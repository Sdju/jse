# JSE - JavaScript Engines (Ru)

> ЭТО ЧЕРНОВИК! Данные будут обновляться для создания в будущем полноценной нормальной базы по движкам. Любые предложения и запросы приветствуются

JSE - сборная солянка для упрощения изучения работы и внутреннего устройства различных движков и рантаймов (в процессе) JS.

## Общее
- JS Engines/Runtimes list
	- https://github.com/errilaz/awesome-js-runtimes
	- https://gist.github.com/guest271314/bd292fc33e1b30dede0643a283fadc6a

- База по движкам 
	- https://www.freecodecamp.org/news/javascript-engine-and-runtime-explained/

- Кладезь информации
	- https://zon8.re/posts/

Способ пощупать многие из перечисленных движков:
- https://github.com/GoogleChromeLabs/jsvu

Еще один хороший способ поизучать кишки движков: это почитать обсуждения под тегами на StackOverflow
- https://stackoverflow.com/questions/tagged/YOUR_ENGINE
	- https://stackoverflow.com/questions/tagged/graalvm
	- https://stackoverflow.com/questions/tagged/javascriptcore
	- https://stackoverflow.com/questions/tagged/v8
	- и тп

## Основные движки
### Spider Monkey
официальная информация:
- https://spidermonkey.dev/blog/

байткод
- https://udn.realityripple.com/docs/Mozilla/Projects/SpiderMonkey/Internals/Bytecode

cli/флаги
- https://udn.realityripple.com/docs/Mozilla/Projects/SpiderMonkey/Introduction_to_the_JavaScript_shell

исходники
- https://searchfox.org/mozilla-central/source/js/src

прочее инфо:
- https://spidermonkey.dev/docs/
- https://firefox-source-docs.mozilla.org/js/index.html
- https://www.youtube.com/@mozhacks/videos
- https://johngrndelwald.medium.com
- https://bugzilla.mozilla.org/buglist.cgi?product=Core&component=MFBT&resolution=---

### JavaScriptCore
официальная информация:
-  https://developer.apple.com/documentation/javascriptcore

байткод
- https://github.com/WebKit/webkit/blob/main/Source/JavaScriptCore/bytecode/Opcode.h

cli/флаги
- https://trac.webkit.org/wiki/JSC

исходники
- https://github.com/WebKit/WebKit/tree/main/Source/JavaScriptCore

прочее инфо:
- https://docs.webkit.org/Deep%20Dive/JSC/JavaScriptCore.html
- https://developer.apple.com/search/?q=JavaScriptCore&type=Videos
- https://webkit.org/?s=javascriptcore
- https://zon8.re/posts/jsc-internals-part1-tracing-js-source-to-bytecode/
- https://ktln2.org/2020/08/25/javascriptcore/
- https://sillycross.github.io/2021/09/12/2021-09-12/
- http://www.filpizlo.com/papers.html

### v8
официальная информация:
-  https://v8.dev/blog

байткод
- https://kuterdinel.com/v8-bytecode-reference.html

cli/флаги
- https://gist.github.com/andrewiggins/68c3165d47769a39eb5ae16e3001d6c6

исходники
- https://chromium.googlesource.com/v8/v8

прочее инфо:
- https://v8docs.nodesource.com/node-20.3/

# Достойные внимания

### Hermes
> JS движок лежащий в основе React Native

официальная информация:
-  https://hermesengine.dev
- https://hermesengine.dev/docs/building-and-running

внутрянка
- https://hermesengine.dev/docs/ir

cli/флаги
- https://github.com/facebook/hermes/blob/55ccdf198078be78ac8c562b0087f561591aa950/npm/hermes-engine-cli/README.md#L4 (очень скудная инфа)
- (буду рад наводкам)

исходники
- https://github.com/facebook/hermes

прочее инфо:
- https://github.com/facebook/hermes/discussions
- https://hermesengine.dev/docs/vm
- https://engineering.fb.com/2019/07/12/android/hermes/
- https://reactnative.dev/blog/2021/10/26/toward-hermes-being-the-default

### XS
> Часть Moddable SDK, цель которого дать возможность гонять JS на IoT устройствах

официальная информация:
-  https://github.com/Moddable-OpenSource/moddable-xst
- https://www.moddable.com
- https://www.moddable.com/documentation/readme

байткод
- явно есть, но пока не сильно погрузился в поиски

cli/флаги
- https://www.moddable.com/documentation/xs/xst

исходники
- https://github.com/Moddable-OpenSource/moddable
- https://github.com/Moddable-OpenSource/moddable/tree/public/xs/sources

прочее инфо:
- https://www.moddable.com/community-call.php

### ChakraCore
> Ранее движок для Edge. Но после ухода Edge на Chromium проект сосредоточен как способ использования JS как встраемого языка

официальная информация:
-  https://github.com/chakra-core/ChakraCore

байткод
- https://github.com/chakra-core/ChakraCore/blob/master/lib/Runtime/ByteCode/OpCodes.h
- https://github.com/chakra-core/ChakraCore/blob/master/lib/Runtime/ByteCode/OpCodesAsmJs.h
- https://github.com/chakra-core/ChakraCore/blob/master/lib/Runtime/ByteCode/OpCodesSimd.h

cli/флаги
- https://github.com/chakra-core/ChakraCore/blob/master/lib/Common/ConfigFlagsList.h
- https://github.com/microsoft/ChakraCore-wiki/blob/master/ch-cli.md

исходники
- https://github.com/chakra-core/ChakraCore

прочее инфо:
- https://github.com/chakra-core/ChakraCore/wiki
- https://github.com/chakra-core/ChakraCore/wiki/Resources
- https://github.com/chakra-core/ChakraCore/wiki/Architecture-Overview

# QuickJS
> Интересная простая реализация JS движка с компилятором
> Имеется актуальный форк Quick.js New Generation https://github.com/quickjs-ng/quickjs
> Однако с 2024 форк и основа взяли курс на объединение

официальная информация:
-  https://bellard.org/quickjs/
- https://bellard.org/quickjs/quickjs.html

байткод
- https://bellard.org/quickjs/quickjs.html#Bytecode

cli/флаги
- https://bellard.org/quickjs/quickjs.html#Command-line-options

исходники
- https://github.com/bellard/quickjs (mirror)

прочее инфо:
- https://www.freelists.org/feed/quickjs-devel

## Java/JVM-based
Иногда движки пишутся и на Java или для JVM конкретно

### Graal.JS (GraalVM JS Support)
> Движок для JS, который собирается под GraalVM
> На данный момент наиболее предпочтительный способ использовать связку Java+JS

официальная информация:
-  https://www.graalvm.org/javascript/
- https://www.graalvm.org/latest/reference-manual/js/

байткод (отсутствует, по факту работает все равно на GraalVM)
cli/флаги
- https://docs.oracle.com/cd/F44923_01/enterprise/19/guide/reference/javascript-nodejs.html

исходники
- https://github.com/oracle/graaljs

прочее инфо:
	https://habr.com/ru/companies/haulmont/articles/433432/
	https://www.youtube.com/watch?v=OUo3BFMwQFo&ab_channel=Devoxx
	https://www.youtube.com/watch?v=a-XEZobXspo&ab_channel=Devoxx
	https://www.youtube.com/watch?v=3SRjPHnWHa0&ab_channel=WixEngineeringTechTalks
	https://www.avisi.nl/blog/an-introduction-to-graalvm-with-examples

### Rhino
> Раньше был частью JDK пока его не сменил Nashorn с Java 8

Судя по активности на Github все еще не заброшен, но **крайне** медленный по отзывам. По факту собирает JS -> JVM bytecode

официальная информация:
-  https://mozilla.github.io/rhino/
- https://javadoc.io/doc/org.mozilla/rhino/latest/index.html

байткод (отсутствует, по факту работает все равно на JVM)
cli/флаги
- https://manpages.ubuntu.com/manpages/jammy/man1/rhino.1.html
- https://www-archive.mozilla.org/rhino/shell

исходники
- https://mozilla.github.io/rhino/

прочее инфо:
- http://web.archive.org/web/20210304081342/https://developer.mozilla.org/en-US/docs/Mozilla/Projects/Rhino/Documentation - архивные записи о Rhino на MDN (более недоступны без машины времени)
- https://mozilla.github.io/rhino/compat/engines.html
- https://habr.com/ru/companies/pvs-studio/articles/688422/

### Nashorn (OpenJDK/Oracle Java)
> стал deprecated с Java 11
> https://openjdk.org/jeps/335
> Причина: ECMAScript слишком быстро развивается, команде стало слишком сложно поддерживать актуальные версии ES

Был частью JDK начиная с Java 8.
инфо
- https://wiki.openjdk.org/display/Nashorn/Main

исходники
- https://github.com/openjdk/nashorn

прочее инфо
- https://wiki.openjdk.org/display/Nashorn/Nashorn%3A+Articles%2C+Documents%2C+Slides+and+Videos
- https://habr.com/ru/articles/195870/
- https://www.oracle.com/technical-resources/articles/java/jf14-nashorn.html
- https://github.com/shekhargulati/java8-the-missing-tutorial/blob/master/10-nashorn.md

### Что нужно дальше?
- Нужно еще больше различных движков
- Нужна еще лучшая структуризация информации
- Нужно еще больше информации о движках
- Нужен перевод на английский (в процессе)
- Нужно еще больше источников с хорошей глубиной
- Перечислить возможные места для обсуждения движков JS
- Дополнить базу знаний рантаймами, бенчмарками и проч
