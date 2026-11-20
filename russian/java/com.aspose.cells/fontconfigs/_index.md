---
title: "FontConfigs"
second_title: "Справочник API Aspose.Cells for Java"
description: "Указывает настройки шрифта"
type: docs
url: /ru/java/com.aspose.cells/fontconfigs/
---

**Inheritance:**
java.lang.Object
```
public class FontConfigs
```

Указывает настройки шрифта
## Конструкторы

| Конструктор | Описание |
| --- | --- |
| [FontConfigs()](#FontConfigs--) |  |
## Методы

| Метод | Описание |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getDefaultFontName()](#getDefaultFontName--) | Возвращает имя шрифта по умолчанию. |
| [getFontFileDataInfo(String fontName, boolean isBold, boolean isItalic, boolean isExactStyle)](#getFontFileDataInfo-java.lang.String-boolean-boolean-boolean-) | Получить информацию о данных файла шрифта. |
| [getFontSources()](#getFontSources--) | Возвращает копию массива, содержащего список источников. |
| [getFontSubstitutes(String originalFontName)](#getFontSubstitutes-java.lang.String-) | Возвращает массив, содержащий имена заменяющих шрифтов, которые будут использоваться, если оригинальный шрифт отсутствует. |
| [hashCode()](#hashCode--) |  |
| [isFontAvailable(String fontName)](#isFontAvailable-java.lang.String-) | Указывает, доступен ли шрифт. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setDefaultFontName(String value)](#setDefaultFontName-java.lang.String-) | Устанавливает имя шрифта по умолчанию. |
| [setFontExclusiveSources(FontSourceBase[] exclusiveSources)](#setFontExclusiveSources-com.aspose.cells.FontSourceBase---) | Устанавливает эксклюзивные источники шрифтов. |
| [setFontFolder(String fontFolder, boolean recursive)](#setFontFolder-java.lang.String-boolean-) | Устанавливает папку шрифтов |
| [setFontFolders(String[] fontFolders, boolean recursive)](#setFontFolders-java.lang.String---boolean-) | Устанавливает папку шрифтов |
| [setFontSources(FontSourceBase[] sources)](#setFontSources-com.aspose.cells.FontSourceBase---) | Устанавливает источники шрифтов. |
| [setFontSubstitutes(String originalFontName, String[] substituteFontNames)](#setFontSubstitutes-java.lang.String-java.lang.String---) | Имена заменяющих шрифтов для заданного оригинального названия шрифта. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### FontConfigs() {#FontConfigs--}
```
public FontConfigs()
```


### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| arg0 | java.lang.Object |  |

**Returns:**
boolean
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getDefaultFontName() {#getDefaultFontName--}
```
public static String getDefaultFontName()
```


Возвращает имя шрифта по умолчанию.

**Returns:**
java.lang.String
### getFontFileDataInfo(String fontName, boolean isBold, boolean isItalic, boolean isExactStyle) {#getFontFileDataInfo-java.lang.String-boolean-boolean-boolean-}
```
public static FontFileDataInfo getFontFileDataInfo(String fontName, boolean isBold, boolean isItalic, boolean isExactStyle)
```


Получить информацию о данных файла шрифта.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| fontName | java.lang.String | название шрифта |
| isBold | boolean | жирный стиль шрифта или нет |
| isItalic | boolean | курсивный стиль шрифта или нет |
| isExactStyle | boolean | нужно ли точно соответствовать заданному жирному/курсивному стилю |

**Returns:**
[FontFileDataInfo](../../com.aspose.cells/fontfiledatainfo) - Data infomation of font file data.
### getFontSources() {#getFontSources--}
```
public static FontSourceBase[] getFontSources()
```


Возвращает копию массива, содержащего список источников.

**Returns:**
com.aspose.cells.FontSourceBase[] -
### getFontSubstitutes(String originalFontName) {#getFontSubstitutes-java.lang.String-}
```
public static String[] getFontSubstitutes(String originalFontName)
```


Возвращает массив, содержащий имена заменяющих шрифтов, которые будут использоваться, если оригинальный шрифт отсутствует.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| originalFontName | java.lang.String | originalFontName |

**Returns:**
java.lang.String[] - Массив, содержащий имена заменяющих шрифтов, которые будут использоваться, если оригинальный шрифт не представлен.
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isFontAvailable(String fontName) {#isFontAvailable-java.lang.String-}
```
public static boolean isFontAvailable(String fontName)
```


Указывает, доступен ли шрифт.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| fontName | java.lang.String | название шрифта |

**Returns:**
boolean - true, если шрифт доступен, иначе false.
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### setDefaultFontName(String value) {#setDefaultFontName-java.lang.String-}
```
public static void setDefaultFontName(String value)
```


Устанавливает имя шрифта по умолчанию.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

### setFontExclusiveSources(FontSourceBase[] exclusiveSources) {#setFontExclusiveSources-com.aspose.cells.FontSourceBase---}
```
public static void setFontExclusiveSources(FontSourceBase[] exclusiveSources)
```


Устанавливает эксклюзивные источники шрифтов. Будут использоваться только шрифты из этих источников.

**Remarks**

System.setProperty("Aspose.Cells.FontDirExc", "fontExclusiveFolder") будет игнорироваться, если это установлено.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| exclusiveSources | [FontSourceBase\[\]](../../com.aspose.cells/fontsourcebase) | Массив источников, содержащих TrueType шрифты. |

### setFontFolder(String fontFolder, boolean recursive) {#setFontFolder-java.lang.String-boolean-}
```
public static void setFontFolder(String fontFolder, boolean recursive)
```


Устанавливает папку шрифтов

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| fontFolder | java.lang.String | Папка, содержащая TrueType шрифты. |
| recursive | boolean | Определяет, сканировать ли подпапки. |

### setFontFolders(String[] fontFolders, boolean recursive) {#setFontFolders-java.lang.String---boolean-}
```
public static void setFontFolders(String[] fontFolders, boolean recursive)
```


Устанавливает папку шрифтов

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| fontFolders | java.lang.String[] | Папки, содержащие TrueType шрифты. |
| recursive | boolean | Определяет, сканировать ли подпапки. |

### setFontSources(FontSourceBase[] sources) {#setFontSources-com.aspose.cells.FontSourceBase---}
```
public static void setFontSources(FontSourceBase[] sources)
```


Устанавливает источники шрифтов.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| sources | [FontSourceBase\[\]](../../com.aspose.cells/fontsourcebase) | Массив источников, содержащих TrueType шрифты. |

### setFontSubstitutes(String originalFontName, String[] substituteFontNames) {#setFontSubstitutes-java.lang.String-java.lang.String---}
```
public static void setFontSubstitutes(String originalFontName, String[] substituteFontNames)
```


Имена заменяющих шрифтов для заданного оригинального названия шрифта.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| originalFontName | java.lang.String | Исходное название шрифта. |
| substituteFontNames | java.lang.String[] | Список имен заменяющих шрифтов, которые будут использоваться, если оригинальный шрифт не представлен. |

### toString() {#toString--}
```
public String toString()
```




**Returns:**
java.lang.String
### wait() {#wait--}
```
public final void wait()
```




### wait(long arg0) {#wait-long-}
```
public final native void wait(long arg0)
```




**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

