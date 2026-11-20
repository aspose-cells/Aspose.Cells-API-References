---
title: "FontConfigs"
second_title: "Riferimento API di Aspose.Cells per Java"
description: "Specifica le impostazioni del font"
type: docs
url: /it/java/com.aspose.cells/fontconfigs/
---

**Inheritance:**
java.lang.Object
```
public class FontConfigs
```

Specifica le impostazioni del font
## Costruttori

| Costruttore | Descrizione |
| --- | --- |
| [FontConfigs()](#FontConfigs--) |  |
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getDefaultFontName()](#getDefaultFontName--) | Restituisce il nome del font predefinito. |
| [getFontFileDataInfo(String fontName, boolean isBold, boolean isItalic, boolean isExactStyle)](#getFontFileDataInfo-java.lang.String-boolean-boolean-boolean-) | Ottieni le informazioni sui dati del file del font. |
| [getFontSources()](#getFontSources--) | Restituisce una copia dell'array che contiene l'elenco delle sorgenti |
| [getFontSubstitutes(String originalFontName)](#getFontSubstitutes-java.lang.String-) | Restituisce un array contenente i nomi dei font sostitutivi da utilizzare se il font originale non è presente. |
| [hashCode()](#hashCode--) |  |
| [isFontAvailable(String fontName)](#isFontAvailable-java.lang.String-) | Indica se il font è disponibile. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setDefaultFontName(String value)](#setDefaultFontName-java.lang.String-) | Imposta il nome del font predefinito. |
| [setFontExclusiveSources(FontSourceBase[] exclusiveSources)](#setFontExclusiveSources-com.aspose.cells.FontSourceBase---) | Imposta le font di origine esclusive. |
| [setFontFolder(String fontFolder, boolean recursive)](#setFontFolder-java.lang.String-boolean-) | Imposta la cartella delle font |
| [setFontFolders(String[] fontFolders, boolean recursive)](#setFontFolders-java.lang.String---boolean-) | Imposta la cartella delle font |
| [setFontSources(FontSourceBase[] sources)](#setFontSources-com.aspose.cells.FontSourceBase---) | Imposta le font di origine. |
| [setFontSubstitutes(String originalFontName, String[] substituteFontNames)](#setFontSubstitutes-java.lang.String-java.lang.String---) | Nomi di sostituzione dei font per il nome del font originale fornito. |
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
| Parametro | Tipo | Descrizione |
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


Restituisce il nome del font predefinito.

**Returns:**
java.lang.String
### getFontFileDataInfo(String fontName, boolean isBold, boolean isItalic, boolean isExactStyle) {#getFontFileDataInfo-java.lang.String-boolean-boolean-boolean-}
```
public static FontFileDataInfo getFontFileDataInfo(String fontName, boolean isBold, boolean isItalic, boolean isExactStyle)
```


Ottieni le informazioni sui dati del file del font.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| fontName | java.lang.String | nome del font |
| isBold | boolean | lo stile del font è in grassetto o meno |
| isItalic | boolean | lo stile del font è in corsivo o meno |
| isExactStyle | boolean | se corrispondere esattamente allo stile grassetto/corsivo fornito |

**Returns:**
[FontFileDataInfo](../../com.aspose.cells/fontfiledatainfo) - Data infomation of font file data.
### getFontSources() {#getFontSources--}
```
public static FontSourceBase[] getFontSources()
```


Restituisce una copia dell'array che contiene l'elenco delle sorgenti

**Returns:**
com.aspose.cells.FontSourceBase[] -
### getFontSubstitutes(String originalFontName) {#getFontSubstitutes-java.lang.String-}
```
public static String[] getFontSubstitutes(String originalFontName)
```


Restituisce un array contenente i nomi dei font sostitutivi da utilizzare se il font originale non è presente.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| originalFontName | java.lang.String | originalFontName |

**Returns:**
java.lang.String[] - Un array contenente i nomi di sostituzione dei font da utilizzare se il font originale non è presente.
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


Indica se il font è disponibile.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| fontName | java.lang.String | nome del font |

**Returns:**
boolean - true se il font è disponibile, altrimenti false.
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


Imposta il nome del font predefinito.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

### setFontExclusiveSources(FontSourceBase[] exclusiveSources) {#setFontExclusiveSources-com.aspose.cells.FontSourceBase---}
```
public static void setFontExclusiveSources(FontSourceBase[] exclusiveSources)
```


Imposta le font di origine esclusive. Solo le font nelle origini saranno usate.

**Remarks**

System.setProperty("Aspose.Cells.FontDirExc", "fontExclusiveFolder") verrà ignorato se questo è impostato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| exclusiveSources | [FontSourceBase\[\]](../../com.aspose.cells/fontsourcebase) | Un array di origini che contengono font TrueType. |

### setFontFolder(String fontFolder, boolean recursive) {#setFontFolder-java.lang.String-boolean-}
```
public static void setFontFolder(String fontFolder, boolean recursive)
```


Imposta la cartella delle font

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| fontFolder | java.lang.String | La cartella che contiene i font TrueType. |
| recursive | boolean | Determina se eseguire o meno la scansione delle sottocartelle. |

### setFontFolders(String[] fontFolders, boolean recursive) {#setFontFolders-java.lang.String---boolean-}
```
public static void setFontFolders(String[] fontFolders, boolean recursive)
```


Imposta la cartella delle font

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| fontFolders | java.lang.String[] | Le cartelle che contengono i font TrueType. |
| recursive | boolean | Determina se eseguire o meno la scansione delle sottocartelle. |

### setFontSources(FontSourceBase[] sources) {#setFontSources-com.aspose.cells.FontSourceBase---}
```
public static void setFontSources(FontSourceBase[] sources)
```


Imposta le font di origine.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| sources | [FontSourceBase\[\]](../../com.aspose.cells/fontsourcebase) | Un array di origini che contengono font TrueType. |

### setFontSubstitutes(String originalFontName, String[] substituteFontNames) {#setFontSubstitutes-java.lang.String-java.lang.String---}
```
public static void setFontSubstitutes(String originalFontName, String[] substituteFontNames)
```


Nomi di sostituzione dei font per il nome del font originale fornito.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| originalFontName | java.lang.String | Nome del font originale. |
| substituteFontNames | java.lang.String[] | Elenco dei nomi dei font sostitutivi da utilizzare se il font originale non è presente. |

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
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

