---
title: "FontConfigs"
second_title: "Aspose.Cells för Java API-referens"
description: "Specificerar typsnittsinställningar."
type: docs
url: /sv/java/com.aspose.cells/fontconfigs/
---

**Inheritance:**
java.lang.Object
```
public class FontConfigs
```

Specificerar typsnittsinställningar.
## Konstruktörer

| Konstruktör | Beskrivning |
| --- | --- |
| [FontConfigs()](#FontConfigs--) |  |
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getDefaultFontName()](#getDefaultFontName--) | Hämtar standardtypsnittets namn. |
| [getFontFileDataInfo(String fontName, boolean isBold, boolean isItalic, boolean isExactStyle)](#getFontFileDataInfo-java.lang.String-boolean-boolean-boolean-) | Hämta datainformation för typsnittsfilens data. |
| [getFontSources()](#getFontSources--) | Hämtar en kopia av arrayen som innehåller listan över källor |
| [getFontSubstitutes(String originalFontName)](#getFontSubstitutes-java.lang.String-) | Returnerar en array som innehåller namn på typsnittssubstitut som ska användas om originaltypsnittet inte finns. |
| [hashCode()](#hashCode--) |  |
| [isFontAvailable(String fontName)](#isFontAvailable-java.lang.String-) | Ange om teckensnittet är tillgängligt. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setDefaultFontName(String value)](#setDefaultFontName-java.lang.String-) | Ställer in standardteckensnittets namn. |
| [setFontExclusiveSources(FontSourceBase[] exclusiveSources)](#setFontExclusiveSources-com.aspose.cells.FontSourceBase---) | Ställer in teckensnittens exklusiva källor. |
| [setFontFolder(String fontFolder, boolean recursive)](#setFontFolder-java.lang.String-boolean-) | Ställer in teckensnittsmappen |
| [setFontFolders(String[] fontFolders, boolean recursive)](#setFontFolders-java.lang.String---boolean-) | Ställer in teckensnittsmappen |
| [setFontSources(FontSourceBase[] sources)](#setFontSources-com.aspose.cells.FontSourceBase---) | Ställer in teckensnittskällorna. |
| [setFontSubstitutes(String originalFontName, String[] substituteFontNames)](#setFontSubstitutes-java.lang.String-java.lang.String---) | Ersättningsnamn för teckensnitt för givet originalteckensnitt. |
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
### getDefaultFontName() {#getDefaultFontName--}
```
public static String getDefaultFontName()
```


Hämtar standardtypsnittets namn.

**Returns:**
java.lang.String
### getFontFileDataInfo(String fontName, boolean isBold, boolean isItalic, boolean isExactStyle) {#getFontFileDataInfo-java.lang.String-boolean-boolean-boolean-}
```
public static FontFileDataInfo getFontFileDataInfo(String fontName, boolean isBold, boolean isItalic, boolean isExactStyle)
```


Hämta datainformation för typsnittsfilens data.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| fontName | java.lang.String | teckensnittsnamn |
| isBold | boolean | teckensnittsstilen är fet eller inte |
| isItalic | boolean | teckensnittsstilen är kursiv eller inte |
| isExactStyle | boolean | om den givna fet/kursiv-stilen ska matchas exakt |

**Returns:**
[FontFileDataInfo](../../com.aspose.cells/fontfiledatainfo) - Data infomation of font file data.
### getFontSources() {#getFontSources--}
```
public static FontSourceBase[] getFontSources()
```


Hämtar en kopia av arrayen som innehåller listan över källor

**Returns:**
com.aspose.cells.FontSourceBase[] -
### getFontSubstitutes(String originalFontName) {#getFontSubstitutes-java.lang.String-}
```
public static String[] getFontSubstitutes(String originalFontName)
```


Returnerar en array som innehåller namn på typsnittssubstitut som ska användas om originaltypsnittet inte finns.

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
### isFontAvailable(String fontName) {#isFontAvailable-java.lang.String-}
```
public static boolean isFontAvailable(String fontName)
```


Ange om teckensnittet är tillgängligt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| fontName | java.lang.String | teckensnittsnamn |

**Returns:**
boolean - true om teckensnittet är tillgängligt, annars false.
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


Ställer in standardteckensnittets namn.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

### setFontExclusiveSources(FontSourceBase[] exclusiveSources) {#setFontExclusiveSources-com.aspose.cells.FontSourceBase---}
```
public static void setFontExclusiveSources(FontSourceBase[] exclusiveSources)
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
public static void setFontFolder(String fontFolder, boolean recursive)
```


Ställer in teckensnittsmappen

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| fontFolder | java.lang.String | Mappen som innehåller TrueType-teckensnitt. |
| rekursiv | boolean | Bestämmer om underkataloger ska genomsökas eller inte. |

### setFontFolders(String[] fontFolders, boolean recursive) {#setFontFolders-java.lang.String---boolean-}
```
public static void setFontFolders(String[] fontFolders, boolean recursive)
```


Ställer in teckensnittsmappen

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| fontFolders | java.lang.String[] | Mapparna som innehåller TrueType-teckensnitt. |
| rekursiv | boolean | Bestämmer om underkataloger ska genomsökas eller inte. |

### setFontSources(FontSourceBase[] sources) {#setFontSources-com.aspose.cells.FontSourceBase---}
```
public static void setFontSources(FontSourceBase[] sources)
```


Ställer in teckensnittskällorna.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| sources | [FontSourceBase\[\]](../../com.aspose.cells/fontsourcebase) | En array av källor som innehåller TrueType-teckensnitt. |

### setFontSubstitutes(String originalFontName, String[] substituteFontNames) {#setFontSubstitutes-java.lang.String-java.lang.String---}
```
public static void setFontSubstitutes(String originalFontName, String[] substituteFontNames)
```


Ersättningsnamn för teckensnitt för givet originalteckensnitt.

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

