![keyboard map](https://github.com/kaefik/common-turkic-alphabet-keyboard/raw/master/keyboard-US-International.png "Full Keyboard Map")

# Раскладка [Common Turkic Alphabet (Уртак төрки әлифба)](https://en.wikipedia.org/wiki/Common_Turkic_Alphabet) для татарского языка

Является форком проекта [US Keyboard Layout + German + Turkish: 3-in-1!](https://github.com/billyc/en-de-tr-keyboard)

Данная раскладка полностью повторяет US (английскую) раскладку с добавлением дополнительных символов из Common Turkic Alphabet. Дополнительные символы получаются комбинацией клавиши `right-ALT` и буквы (смотрите ниже в таблице).

Раскладка Common Turkic Alphabet может использоваться при работе с текстами на татарском языке латиницей. Также и с другими родственными языками, подробнее смотрите [здесь](https://en.wikipedia.org/wiki/Common_Turkic_Alphabet).



## Комбинации клавиш специфичных для Common Turkic Alphabet

На английской клавиатуре клавиша `AltGr` - это клавиша **ALT** с правой стороны от клавиши пробел.

Чтобы напечатать:
   * строчную букву зажимаете `RIGHT-ALT` и нажимаете букву.
   * прописную букву зажимаете две клавиши `SHIFT` and `RIGHT-ALT` и затем нажимаете букву.


| Буква  | Как получить букву|
| ------ | ----------------- |
| `ö`    | `RIGHT-ALT` + `O` |
| `ü`    | `RIGHT-ALT` + `U` |
| `ä`    | `RIGHT-ALT` + `A` |
| `ş`    | `RIGHT-ALT` + `S` |
| `ç`    | `RIGHT-ALT` + `C` |
| `ğ`    | `RIGHT-ALT` + `G` |
| `ı/İ`  | `RIGHT-ALT` + `I` |


# Установка

## 1. Windows

Установка клавиатуры работает ОС WIndows 7 и выше.

1. скачать [tatlat](https://github.com/kaefik/common-turkic-alphabet-keyboard/blob/master/windows/tatlat.zip)

2. распакуйте архив и запустите `setup.exe`.

3. На вашей системе

   * WIndows 7 и Windows 8.1

     зайдите в `Control Panel (Панель управления)` -> раздел `Clock, Language and Region` -> выбрать `Add a language` -> выбрать язык `English (United States)` -> выбрать `Options (Настройки)`

   * Windows 10

     * выберите `Settings (Настройки)` -> `Time & Language (Время & Язык)`  -> `Language (Язык)`-> кликнуть на `English (United States)` -> выбрать `Options (Настройки)` увидите что установлен Tatar latin

4. удалите "US Qwerty" (Английский язык) чтобы был один United States (Tatar latin) в системе.

## 2. Ubuntu

Файлы которые используются ниже вы найдете здесь <https://github.com/kaefik/common-turkic-alphabet-keyboard/linux>


1. Скопировать два файла у казанные места используя `sudo`:

   ```bash
   sudo cp usr-share-x11-xkb-symbols-us /usr/share/X11/xkb/symbols/us
   sudo cp usr-share-x11-xkb-rules-evdev.xml /usr/share/X11/xkb/rules/evdev.xml
   ```

3. Нужно перезайти в пользователя или  перезагрузить компьютер

4. В Gnome `Settings` (`Настройки`), выбрать `Keyboard` (`Клавиатура`), и раздел `Input Sources` (`Источники ввода`):
   - Нажмите `+`
   - Выберите "English (United States)" ("Английский (Соединенные штаты)")
   - Выберите "English (En/Tatar latin)"
   - Нажмите  `Add` (`Добавить`) и закройте.

**Замечание.** пункты с 1 по 2 можно выполнить запуском скрипта `install_keyboard_common_turk.sh`.


### Примечание

Вы можете сделать свою раскладку для своего языка или исправить или дополнить текущую раскладку. Можете использовать бесплатно в различных целях.

Можно скачать [Microsoft Keyboard Layout Creator](https://github.com/kaefik/common-turkic-alphabet-keyboard/blob/master/windows/MSKLC.exe) и файл раскладки  [us-tatar_latin.klc](https://github.com/kaefik/common-turkic-alphabet-keyboard/blob/master/windows/us-tatar_latin.klc)

#### Другое

Windows: Built with the [Microsoft Keyboard Layout Creator](https://www.microsoft.com/en-us/download/details.aspx?id=102134). Props to [keyboards.jargon-file.org](http://keyboards.jargon-file.org) for the initial KLC file!

Linux: I followed this blog to figure out how to do it: <http://karols.github.io/blog/2013/11/18/creating-custom-keyboard-layouts-for-linux/>
