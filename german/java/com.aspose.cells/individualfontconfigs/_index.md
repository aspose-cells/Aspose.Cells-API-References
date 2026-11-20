---
title: "IndividualFontConfigs"
second_title: "Aspose.Cells for Java API-Referenz"
description: "Schriftkonfigurationen für jedes Objekt."
type: docs
url: /de/java/com.aspose.cells/individualfontconfigs/
---

**Inheritance:**
java.lang.Object
```
public class IndividualFontConfigs
```

Schriftkonfigurationen für jedes [Workbook](../../com.aspose.cells/workbook)-Objekt.
## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [IndividualFontConfigs()](#IndividualFontConfigs--) | Konstruktor. |
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getFontSources()](#getFontSources--) | Liefert eine Kopie des Arrays, das die Liste der Quellen enthält. |
| [getFontSubstitutes(String originalFontName)](#getFontSubstitutes-java.lang.String-) | Gibt ein Array mit Schriftart-Ersatznamen zurück, die verwendet werden, wenn die Originalschriftart nicht vorhanden ist. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setFontExclusiveSources(FontSourceBase[] exclusiveSources)](#setFontExclusiveSources-com.aspose.cells.FontSourceBase---) | Legt die exklusiven Quellen der Schriftarten fest. |
| [setFontFolder(String fontFolder, boolean recursive)](#setFontFolder-java.lang.String-boolean-) | Legt den Schriftarten-Ordner fest |
| [setFontFolders(String[] fontFolders, boolean recursive)](#setFontFolders-java.lang.String---boolean-) | Legt die Schriftordner fest |
| [setFontSources(FontSourceBase[] sources)](#setFontSources-com.aspose.cells.FontSourceBase---) | Legt die Schriftart-Quellen fest. |
| [setFontSubstitutes(String originalFontName, String[] substituteFontNames)](#setFontSubstitutes-java.lang.String-java.lang.String---) | Legt Schriftart-Ersatznamen für einen angegebenen Originalschriftartnamen fest. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### IndividualFontConfigs() {#IndividualFontConfigs--}
```
public IndividualFontConfigs()
```


Konstruktor.

### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| Parameter | Typ | Beschreibung |
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


Liefert eine Kopie des Arrays, das die Liste der Quellen enthält.

**Returns:**
com.aspose.cells.FontSourceBase[] -
### getFontSubstitutes(String originalFontName) {#getFontSubstitutes-java.lang.String-}
```
public String[] getFontSubstitutes(String originalFontName)
```


Gibt ein Array mit Schriftart-Ersatznamen zurück, die verwendet werden, wenn die Originalschriftart nicht vorhanden ist.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| originalFontName | java.lang.String | originalFontName |

**Returns:**
java.lang.String[] - Ein Array, das Schriftart-Ersatznamen enthält, die verwendet werden, wenn die Originalschriftart nicht vorhanden ist.
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


Legt die exklusiven Quellen der Schriftarten fest. Nur Schriftarten in den Quellen werden verwendet.

**Remarks**

System.setProperty(\"Aspose.Cells.FontDirExc\", \"fontExclusiveFolder\") wird ignoriert, wenn dies gesetzt ist.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| exclusiveSources | [FontSourceBase\[\]](../../com.aspose.cells/fontsourcebase) | Ein Array von Quellen, die TrueType-Schriftarten enthalten. |

### setFontFolder(String fontFolder, boolean recursive) {#setFontFolder-java.lang.String-boolean-}
```
public void setFontFolder(String fontFolder, boolean recursive)
```


Legt den Schriftarten-Ordner fest

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| fontFolder | java.lang.String | Der Ordner, der TrueType-Schriftarten enthält. |
| rekursiv | boolean | Bestimmt, ob Unterordner gescannt werden sollen oder nicht. |

### setFontFolders(String[] fontFolders, boolean recursive) {#setFontFolders-java.lang.String---boolean-}
```
public void setFontFolders(String[] fontFolders, boolean recursive)
```


Legt die Schriftordner fest

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| fontFolders | java.lang.String[] | Die Ordner, die TrueType-Schriften enthalten. |
| rekursiv | boolean | Bestimmt, ob Unterordner gescannt werden sollen oder nicht. |

### setFontSources(FontSourceBase[] sources) {#setFontSources-com.aspose.cells.FontSourceBase---}
```
public void setFontSources(FontSourceBase[] sources)
```


Legt die Schriftart-Quellen fest.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| sources | [FontSourceBase\[\]](../../com.aspose.cells/fontsourcebase) | Ein Array von Quellen, die TrueType-Schriftarten enthalten. |

### setFontSubstitutes(String originalFontName, String[] substituteFontNames) {#setFontSubstitutes-java.lang.String-java.lang.String---}
```
public void setFontSubstitutes(String originalFontName, String[] substituteFontNames)
```


Legt Schriftart-Ersatznamen für einen angegebenen Originalschriftartnamen fest.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| originalFontName | java.lang.String | Ursprünglicher Schriftname. |
| substituteFontNames | java.lang.String[] | Liste von Ersatzschriftartnamen, die verwendet werden, wenn die ursprüngliche Schrift nicht vorhanden ist. |

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
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

