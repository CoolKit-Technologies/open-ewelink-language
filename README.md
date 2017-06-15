# open-ewelink-language
We created this project to support translation for eWelink

---
# IOS翻译注意事项

## 翻译文件：
	country-all.js : 国家码名称翻译
	locale-da.json : 丹麦翻译
	locale-en.json : 英文翻译
	locale-it.json : 意大利翻译
	locale-pl.json : 葡萄牙翻译
	locale-ru.json : 俄语翻译
	locale-zh.json : 简体中文翻译
	locale-zh_HK.json : 繁体中文（香港）翻译
	locale-zh_TW.json : 繁体中文 （台湾）翻译
	locale-fr.json : 法语翻译
	locale-de.json : 德语翻译
	locale-es.json : 西班牙语翻译
	ios/locale-bg.json : 保加利亚语
	ios/locale-el.json : 希腊语
	ios/locale-sk.json : 斯洛伐克语
	ios/locale-tr.json : 土耳其语

## 翻译规则：
	国家码翻译：对国家名称的国际化，使用JSON格式来描述一个国家，如果需要新增国家，请新增一个JSON格式
	属性格式为：国家名称缩写+"_name"+":"+"具体国际化国家名称"，
	例如 :
	        {
            	zh_name: '中国',
            	en_name: 'China',
            	ru_name: 'Китай',
            	da_name: 'China',
            	prefix: '+86'
        	}

    其他部分翻译：对具体app文字的，
    属性格式为："App标识符（仅用于app本身唯一性描述与使用，本身无意义"+":"+“具体国际化翻译”；
    例如：
	    locale-zh.json :
		    {
	  			"ABOUTE_WELINK": "关于易微联",
		    }
		locale-en.json :
			{
				 "ABOUTE_WELINK": "About eWeLink",
			}
		local-zh_HT.js :
			{
				  "ABOUTE_WELINK": "關於易微联",
			}	

*注意：仅需对 ”具体国际化国家名称“与”具体国际化翻译“翻译，即 ":" 后面的内容翻译即可；*

---

---
# IOS Translation Notes

## Translation File:
  country-all.js :  country code translation
  locale-da.json :  Danish translation
  locale-en.json :  English translation
  locale-it.json :  Italian translation
  locale-pl.json :  Portuguese translation
  locale-ru.json :  Russian translation
  locale-zh.json :  Simplified Chinese translation
  locale-zh_HK.json : Traditional Chinese (HK) translation
  locale-zh_TW.json : Traditional Chinese (Taiwan) translation
  locale-fr.json : French translator
  locale-de.json : German translator
  locale-es.json : Spanish translator
  locale-bg.json : Bulgarian translator
  locale-el.json : Greek translator
  locale-sk.json : Slovakia translator
  locale-tr.json : Turkic translator

## Translation rules：

	Country code translation: the name of a country or location should be described in JSON format. To add a new country or location, please add a country name in JSON format first.
	The attribute format should be: country name abbreviation + "_ name" + ":" + "specific internationalized country name"

	For example:
	          {
	              zh_name: '中国',
	              en_name: 'China',
	              ru_name: 'Китай',
	              da_name: 'China',
	              prefix: '+86'
	          }

	Other translation: for all other description and prompt words,
	The attribute format should be: "App identifier (only for the app itself to distinguish among different descriptions, it does not have any meaning)" + ":" + "specific international translation";
	For example:
	      locale-zh.json :
	        {
	          "ABOUTE_WELINK": "关于易微联",
	        }
	    locale-en.json :
	      {
	         "ABOUTE_WELINK": "About eWeLink",
	      }
	    local-zh_HT.js :
	      {
	          "ABOUTE_WELINK": "關於易微联",
	      }  

	* Note: it only needs to translate "specific internationalized country name" and "specific internationalized translation", which is the content behind the ":" *

---
# Android翻译注意事项

## 翻译文件：
	values:英语
	values-da-rDK:丹麦语
	values-it-rIT:意大利语
	values-pl-rPL:波兰语
	values-ru-rRU:俄语
	values-zh-rCN:简体中文
	values-zh-rTW:繁体中文
	values-bg-rBG:保加利亚语
	values-tr-rTR:土耳其语
	values-sk-rSK:斯洛伐克语
	values-fr-rFR:法语
	values-eu-rES:西班牙语
	values-el-rGR:希腊语
	values-de-rDE:德语
	
	

## 翻译规则：
    例如:
	1.<string-array name="phone_managers">
	内容无需翻译.	
	</string-array>

	2.<string-array name="country_code1">
		<item>xxx+yy</item>  
	只需要翻译"+"之前的内容	
	</string-array>

	3.<string name="xxxxx">yyyyy</string>
	只需要翻译yyyyy.

	4.<string name="xxxxx">yyyyy%1$s</string>
	只需要翻译yyyyy, "%1$s"不做修改.

	5.<string name="xxxxx">yyyyy\n%1$s</string>
	只需要翻译yyyyy, "\n%1$s"不做修改.

	6.<string name="xxxxx">(timer: %1$sdays %2$shours %3$sminutes xx)</string>
	只需要翻译timer: days  hours minutes xx
	"%1$s","%2$s","%3$s"不做修改

	7.<string name="xxxxx">yy\tzz</string>
	只需要翻译yy,zz, "\t"不做修改.

	8.<string name="xxxxx">yy\n\nzz</string>
	只需要翻译yy,zz, "\n\n"不做修改.
	
	---
# Android Translation Notes

## Translation File:
	values: English
	values-da-rDK: Danish
	values-it-rIT: Italian
	values-pl-rPL: Polish
	values-ru-rRU: Russian
	values-zh-rCN: Simplified Chinese
	values-zh-rTW: Traditional Chinese
	values-bg-rBG: Bulgarian
	values-tr-rTR: Turkish
	values-sk-rSK: Slovakian
	values-fr-rFR: French
	values-eu-rES: Spanish
	values-el-rGR: Greek
	values-de-rDE: German

## Translation rules：
    For example:
	1.<string-array name="phone_managers">
	 No need to translate.	
	</string-array>

	2.<string-array name="country_code1">
		<item>xxx+yy</item>  
	Please translate the content before "+".
	</string-array>

	3.<string name="xxxxx">yyyyy</string>
	Only need to translate yyyyy.

	4.<string name="xxxxx">yyyyy%1$s</string>
	Only need to translate yyyyy. Keep "%1$s" unchanged.

	5.<string name="xxxxx">yyyyy\n%1$s</string>
	Only need to translate yyyyy. Keep "\n%1$s" unchanged.

	6.<string name="xxxxx">(timer: %1$sdays %2$shours %3$sminutes xx)</string>
	Only need to translate timer: days  hours minutes xx
	Keep "%1$s","%2$s","%3$s" unchanged.

	7.<string name="xxxxx">yy\tzz</string>
	Only need to translate yy,zz. Keep "\t" unchanged.


	8.<string name="xxxxx">yy\n\nzz</string>
	Only need to translate yy,zz. Keep "\n\n" unchanged.
	
