---
title: "IndividualFontConfigs"
second_title: "Riferimento API di Aspose.Cells per Java"
description: "Configurazioni dei font per ogni oggetto."
type: docs
url: /it/java/com.aspose.cells/individualfontconfigs/
---

**Inheritance:**
java.lang.Object
```
public class IndividualFontConfigs
```

Configurazioni dei font per ogni oggetto [Workbook](../../com.aspose.cells/workbook).
## Costruttori

| Costruttore | Descrizione |
| --- | --- |
| [IndividualFontConfigs()](#IndividualFontConfigs--) | Ctor. |
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getFontSources()](#getFontSources--) | Restituisce una copia dell'array che contiene l'elenco delle sorgenti |
| [getFontSubstitutes(String originalFontName)](#getFontSubstitutes-java.lang.String-) | Restituisce un array contenente i nomi dei font sostitutivi da utilizzare se il font originale non è presente. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setFontExclusiveSources(FontSourceBase[] exclusiveSources)](#setFontExclusiveSources-com.aspose.cells.FontSourceBase---) | Imposta le font di origine esclusive. |
| [setFontFolder(String fontFolder, boolean recursive)](#setFontFolder-java.lang.String-boolean-) | Imposta la cartella delle font |
| [setFontFolders(String[] fontFolders, boolean recursive)](#setFontFolders-java.lang.String---boolean-) | Imposta le cartelle dei font |
| [setFontSources(FontSourceBase[] sources)](#setFontSources-com.aspose.cells.FontSourceBase---) | Imposta le font di origine. |
| [setFontSubstitutes(String originalFontName, String[] substituteFontNames)](#setFontSubstitutes-java.lang.String-java.lang.String---) | Imposta i nomi dei font sostitutivi per un determinato nome di font originale. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### IndividualFontConfigs() {#IndividualFontConfigs--}
```
public IndividualFontConfigs()
```


Ctor.

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
### getFontSources() {#getFontSources--}
```
public FontSourceBase[] getFontSources()
```


Restituisce una copia dell'array che contiene l'elenco delle sorgenti

**Returns:**
com.aspose.cells.FontSourceBase[] -
### getFontSubstitutes(String originalFontName) {#getFontSubstitutes-java.lang.String-}
```
public String[] getFontSubstitutes(String originalFontName)
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


Imposta le font di origine esclusive. Solo le font nelle origini saranno usate.

**Remarks**

System.setProperty("Aspose.Cells.FontDirExc", "fontExclusiveFolder") verrà ignorato se questo è impostato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| exclusiveSources | [FontSourceBase\[\]](../../com.aspose.cells/fontsourcebase) | Un array di origini che contengono font TrueType. |

### setFontFolder(String fontFolder, boolean recursive) {#setFontFolder-java.lang.String-boolean-}
```
public void setFontFolder(String fontFolder, boolean recursive)
```


Imposta la cartella delle font

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| fontFolder | java.lang.String | La cartella che contiene i font TrueType. |
| recursive | boolean | Determina se eseguire o meno la scansione delle sottocartelle. |

### setFontFolders(String[] fontFolders, boolean recursive) {#setFontFolders-java.lang.String---boolean-}
```
public void setFontFolders(String[] fontFolders, boolean recursive)
```


Imposta le cartelle dei font

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| fontFolders | java.lang.String[] | Le cartelle che contengono i font TrueType. |
| recursive | boolean | Determina se eseguire o meno la scansione delle sottocartelle. |

### setFontSources(FontSourceBase[] sources) {#setFontSources-com.aspose.cells.FontSourceBase---}
```
public void setFontSources(FontSourceBase[] sources)
```


Imposta le font di origine.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| sources | [FontSourceBase\[\]](../../com.aspose.cells/fontsourcebase) | Un array di origini che contengono font TrueType. |

### setFontSubstitutes(String originalFontName, String[] substituteFontNames) {#setFontSubstitutes-java.lang.String-java.lang.String---}
```
public void setFontSubstitutes(String originalFontName, String[] substituteFontNames)
```


Imposta i nomi dei font sostitutivi per un determinato nome di font originale.

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

