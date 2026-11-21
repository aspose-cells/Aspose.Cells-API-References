---
title: "IndividualFontConfigs"
second_title: "Aspose.Cells för Java API-referens"
description: "Teckensnittskonfigurationer för varje objekt."
type: docs
url: /sv/java/com.aspose.cells/individualfontconfigs/
---

**Inheritance:**
java.lang.Object
```
public class IndividualFontConfigs
```

Typsnittskonfigurationer för varje [Workbook](../../com.aspose.cells/workbook) objekt.
## Konstruktörer

| Konstruktör | Beskrivning |
| --- | --- |
| [IndividualFontConfigs()](#IndividualFontConfigs--) | Konstruktor. |
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getFontSources()](#getFontSources--) | Hämtar en kopia av arrayen som innehåller listan över källor |
| [getFontSubstitutes(String originalFontName)](#getFontSubstitutes-java.lang.String-) | Returnerar en array som innehåller namn på typsnittsersättningar som ska användas om originaltypsnittet inte finns. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setFontExclusiveSources(FontSourceBase[] exclusiveSources)](#setFontExclusiveSources-com.aspose.cells.FontSourceBase---) | Ställer in teckensnittens exklusiva källor. |
| [setFontFolder(String fontFolder, boolean recursive)](#setFontFolder-java.lang.String-boolean-) | Ställer in teckensnittsmappen |
| [setFontFolders(String[] fontFolders, boolean recursive)](#setFontFolders-java.lang.String---boolean-) | Ställer in typsnittsmapparna |
| [setFontSources(FontSourceBase[] sources)](#setFontSources-com.aspose.cells.FontSourceBase---) | Ställer in teckensnittskällorna. |
| [setFontSubstitutes(String originalFontName, String[] substituteFontNames)](#setFontSubstitutes-java.lang.String-java.lang.String---) | Ställer in namn på typsnittsersättningar för ett givet originaltypsnitt. |
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
| Parameter | Typ | Beskrivning |
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


Hämtar en kopia av arrayen som innehåller listan över källor

**Returns:**
com.aspose.cells.FontSourceBase[] -
### getFontSubstitutes(String originalFontName) {#getFontSubstitutes-java.lang.String-}
```
public String[] getFontSubstitutes(String originalFontName)
```


Returnerar en array som innehåller namn på typsnittsersättningar som ska användas om originaltypsnittet inte finns.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| originalFontName | java.lang.String | originalFontName |

**Returns:**
java.lang.String[] - En array som innehåller ersättningsnamn för teckensnitt som ska användas om originalteckensnittet inte finns.
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


Ställer in teckensnittens exklusiva källor. Endast teckensnitt i källorna kommer att användas.

**Remarks**

System.setProperty("Aspose.Cells.FontDirExc", "fontExclusiveFolder") kommer att ignoreras om detta är inställt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| exclusiveSources | [FontSourceBase\[\]](../../com.aspose.cells/fontsourcebase) | En array av källor som innehåller TrueType-teckensnitt. |

### setFontFolder(String fontFolder, boolean recursive) {#setFontFolder-java.lang.String-boolean-}
```
public void setFontFolder(String fontFolder, boolean recursive)
```


Ställer in teckensnittsmappen

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| fontFolder | java.lang.String | Mappen som innehåller TrueType-teckensnitt. |
| rekursiv | boolean | Bestämmer om underkataloger ska genomsökas eller inte. |

### setFontFolders(String[] fontFolders, boolean recursive) {#setFontFolders-java.lang.String---boolean-}
```
public void setFontFolders(String[] fontFolders, boolean recursive)
```


Ställer in typsnittsmapparna

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| fontFolders | java.lang.String[] | Mapparna som innehåller TrueType-teckensnitt. |
| rekursiv | boolean | Bestämmer om underkataloger ska genomsökas eller inte. |

### setFontSources(FontSourceBase[] sources) {#setFontSources-com.aspose.cells.FontSourceBase---}
```
public void setFontSources(FontSourceBase[] sources)
```


Ställer in teckensnittskällorna.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| sources | [FontSourceBase\[\]](../../com.aspose.cells/fontsourcebase) | En array av källor som innehåller TrueType-teckensnitt. |

### setFontSubstitutes(String originalFontName, String[] substituteFontNames) {#setFontSubstitutes-java.lang.String-java.lang.String---}
```
public void setFontSubstitutes(String originalFontName, String[] substituteFontNames)
```


Ställer in namn på typsnittsersättningar för ett givet originaltypsnitt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| originalFontName | java.lang.String | Ursprungligt teckensnittsnamn. |
| substituteFontNames | java.lang.String[] | Lista med teckensnittssubstitutionsnamn som ska användas om det ursprungliga teckensnittet inte finns. |

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
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

