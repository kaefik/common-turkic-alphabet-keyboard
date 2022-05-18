![keyboard map](https://github.com/kaefik/common-turkic-alphabet-keyboard/raw/master/keyboard-US-International.png "Full Keyboard Map")

# Раскладка [Common Turkic Alphabet (Уртак төрки әлифба)](https://en.wikipedia.org/wiki/Common_Turkic_Alphabet) для татарского языка

Является форком проекта (US Keyboard Layout + German + Turkish: 3-in-1!)[https://github.com/billyc/en-de-tr-keyboard].

Данная раскладка полностью повторяет US (английскую) раскладку с добавлением дополнительных символов из Common Turkic Alphabet. Дополнительные символы получаются комбинацией клавиши `right-ALT` и буквы (смотрите ниже в таблице).

Раскладка Common Turkic Alphabet может использоваться при работе с текстами на татарском языке латиницей. Также и с другими родственными языками, подробнее смотоите [здесь](https://en.wikipedia.org/wiki/Common_Turkic_Alphabet).



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


**TODO: нужно проверить и исправить**
```
**About that Turkish `İ`**

^a 
**Circumflex** - 

_EDIT -- this no longer works, ignore this_

Some older Turkish words still use the circumflex `^` e.g. _bekârım_. You can type those by using what's called "dead key" combinations:

- First type `SHIFT`+`RIGHT-ALT`+`6` (the circumflex key) -- nothing will show up on your screen
- Then type the vowel. The letter with the cute little hat will magically appear: â, ô, ê, î
```


# Установка

## 1. Windows  - **TODO: нужно проверить и исправить**
```
The provided setup file should work on Windows 7 and up.

- Download [intl+bc.zip](https://github.com/billyc/en-de-tr-keyboard/raw/master/windows/intl%2Bbc.zip)
- Unzip the contents, and run `setup.exe`.
- Then go to your system _Region & Language_ control panel. Under the English language options, you should be able to add/remove the "US International Alternate + Turkish" keyboard.
- For my own system, I removed the "US Qwerty" keyboard so that Windows always defaults to this layout. Otherwise you may need to choose it from the language icon near your system clock/tray.
```

## 2. Ubuntu

Файлы которые используются ниже вы найдете здесь <https://github.com/kaefik/common-turkic-alphabet-keyboard/linux>


1. Скопировать два файла у казанные места используя `sudo`:

   ```bash
   sudo cp usr-share-x11-xkb-symbols-us /usr/share/X11/xkb/symbols/us
   sudo cp usr-share-x11-xkb-rules-evdev.xml /usr/share/X11/xkb/rules/evdev.xml
   ```

2. Скопируйте файл XCompose в свою домашнюю папку `~/.XCompose`

   ```bash
   cp XCompose ~/.XCompose
   ```

3. Нужно перезайти в пользователя или просто перезагрузить компьютер

4. В Gnome `Settings` (`Настройки`), выбрать `Keyboard` (`Клавиатура`), и раздел `Input Sources` (`Источники ввода`):
   - Нажмите `+`
   - Выберите "English (United States)" ("Английский (Соединенные штаты)")
   - Выберите "English (En/Tatar latin)"
   - Нажмите  `Add` (`Добавить`) и закройте.

Замечание. пункты с 1 по 2 можнов ыполнить запуском скрипта `install_keyboard_common_turk.sh`.
 

### Примечание

Вы можете сделать свою раскладку для своего языка или исправить или дополнить текущую раскладку. Можете использовать бесплатно в различных целях.

Windows: Built with the [Microsoft Keyboard Layout Creator](https://msdn.microsoft.com/en-us/globalization/keyboardlayouts.aspx). Props to [keyboards.jargon-file.org](http://keyboards.jargon-file.org) for the initial KLC file!

Linux: I followed this blog to figure out how to do it: <http://karols.github.io/blog/2013/11/18/creating-custom-keyboard-layouts-for-linux/>
