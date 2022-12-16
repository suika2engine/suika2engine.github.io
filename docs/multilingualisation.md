---
title: Multilingualisation
---

[Return to Table of Contents](home)

Suika2 supports several methods of multilingualisation, each with their own benefits and drawbacks.

# Language Specifiers
Language Specifiers are Suika2's preferred, built-in method of multilingualisation and are based on a user's system locale.

Please see the list of language locales below:

|Language                                          |Abbrev. Name             |
|--------------------------------------------------|-------------------------|
|English                                           |`en`                     |
|French                                            |`fr`                     |
|German                                            |`de`                     |
|Spanish                                           |`es`                     |
|Italian                                           |`it`                     |
|Greek                                             |`el`                     |
|Russian                                           |`ru`                     |
|Simplified Chinese                                |`zh`                     |
|Traditional Chinese                               |`tw`                     |
|Japanese                                          |`ja`                     |
|Other                                             |                         |

Developers may use the `Other` option to specify an alternative or secondary fallback language.

The following scripts provides an English and Japanese message. If the user's locale is set to English, then English will be displayed and Japanese will be hidden. The opposite will take effect if the user's locale is set to Japanese.
```
+en+This is an English Message!
+ja+日本語のメッセージです。
```

Depending on a script's formatting, language specifiers may be omitted for the default display language, however, it is suggested that, if more than one language is used, developers utilise specifiers on all messages.

# Pre-Game Language Selection
Another method of multilingualisation is to provide an option at application start.

This can be achieved with the following inserted at the beginning of the script:
```
@choose ENGLISH "English" JAPANESE "日本語"
:english
@load english-script.txt

:japanese
@load japanese-script.txt
:end
```

# Other Methods
There are a number of approaches not discussed here, such as:
* A seperate game launcher
* Seperate distributions based on language
* Bilingual display
