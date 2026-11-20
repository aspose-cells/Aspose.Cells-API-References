---
title: "IndividualFontConfigs"
second_title: "Справочник API Aspose.Cells for Java"
description: "Конфигурации шрифтов для каждого объекта."
type: docs
url: /ru/java/com.aspose.cells/individualfontconfigs/
---

**Inheritance:**
java.lang.Object
```
public class IndividualFontConfigs
```

Конфигурации шрифтов для каждого объекта [Workbook](../../com.aspose.cells/workbook).
## Конструкторы

| Конструктор | Описание |
| --- | --- |
| [IndividualFontConfigs()](#IndividualFontConfigs--) | Конструктор. |
## Методы

| Метод | Описание |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getFontSources()](#getFontSources--) | Возвращает копию массива, содержащего список источников. |
| [getFontSubstitutes(String originalFontName)](#getFontSubstitutes-java.lang.String-) | Возвращает массив, содержащий имена заменяющих шрифтов, которые будут использоваться, если оригинальный шрифт не представлен. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setFontExclusiveSources(FontSourceBase[] exclusiveSources)](#setFontExclusiveSources-com.aspose.cells.FontSourceBase---) | Устанавливает эксклюзивные источники шрифтов. |
| [setFontFolder(String fontFolder, boolean recursive)](#setFontFolder-java.lang.String-boolean-) | Устанавливает папку шрифтов |
| [setFontFolders(String[] fontFolders, boolean recursive)](#setFontFolders-java.lang.String---boolean-) | Устанавливает папки шрифтов |
| [setFontSources(FontSourceBase[] sources)](#setFontSources-com.aspose.cells.FontSourceBase---) | Устанавливает источники шрифтов. |
| [setFontSubstitutes(String originalFontName, String[] substituteFontNames)](#setFontSubstitutes-java.lang.String-java.lang.String---) | Устанавливает имена заменяющих шрифтов для заданного оригинального имени шрифта. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### IndividualFontConfigs() {#IndividualFontConfigs--}
```
public IndividualFontConfigs()
```


Конструктор.

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
### getFontSources() {#getFontSources--}
```
public FontSourceBase[] getFontSources()
```


Возвращает копию массива, содержащего список источников.

**Returns:**
com.aspose.cells.FontSourceBase[] -
### getFontSubstitutes(String originalFontName) {#getFontSubstitutes-java.lang.String-}
```
public String[] getFontSubstitutes(String originalFontName)
```


Возвращает массив, содержащий имена заменяющих шрифтов, которые будут использоваться, если оригинальный шрифт не представлен.

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
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### setFontExclusiveSources(FontSourceBase[] exclusiveSources) {#setFontExclusiveSources-com.aspose.cells.FontSourceBase---}
```
public void setFontExclusiveSources(FontSourceBase[] exclusiveSources)
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
public void setFontFolder(String fontFolder, boolean recursive)
```


Устанавливает папку шрифтов

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| fontFolder | java.lang.String | Папка, содержащая TrueType шрифты. |
| recursive | boolean | Определяет, сканировать ли подпапки. |

### setFontFolders(String[] fontFolders, boolean recursive) {#setFontFolders-java.lang.String---boolean-}
```
public void setFontFolders(String[] fontFolders, boolean recursive)
```


Устанавливает папки шрифтов

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| fontFolders | java.lang.String[] | Папки, содержащие TrueType шрифты. |
| recursive | boolean | Определяет, сканировать ли подпапки. |

### setFontSources(FontSourceBase[] sources) {#setFontSources-com.aspose.cells.FontSourceBase---}
```
public void setFontSources(FontSourceBase[] sources)
```


Устанавливает источники шрифтов.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| sources | [FontSourceBase\[\]](../../com.aspose.cells/fontsourcebase) | Массив источников, содержащих TrueType шрифты. |

### setFontSubstitutes(String originalFontName, String[] substituteFontNames) {#setFontSubstitutes-java.lang.String-java.lang.String---}
```
public void setFontSubstitutes(String originalFontName, String[] substituteFontNames)
```


Устанавливает имена заменяющих шрифтов для заданного оригинального имени шрифта.

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

