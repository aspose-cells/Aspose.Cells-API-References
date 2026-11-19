---
title: "IndividualFontConfigs"
second_title: "Référence API d'Aspose.Cells pour Java"
description: "Configurations de police pour chaque objet."
type: docs
url: /fr/java/com.aspose.cells/individualfontconfigs/
---

**Inheritance:**
java.lang.Object
```
public class IndividualFontConfigs
```

Configurations de police pour chaque objet [Workbook](../../com.aspose.cells/workbook).
## Constructeurs

| Constructeur | Description |
| --- | --- |
| [IndividualFontConfigs()](#IndividualFontConfigs--) | Ctor. |
## Méthodes

| Méthode | Description |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getFontSources()](#getFontSources--) | Obtient une copie du tableau qui contient la liste des sources |
| [getFontSubstitutes(String originalFontName)](#getFontSubstitutes-java.lang.String-) | Renvoie un tableau contenant les noms de polices de substitution à utiliser si la police d'origine n'est pas disponible. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setFontExclusiveSources(FontSourceBase[] exclusiveSources)](#setFontExclusiveSources-com.aspose.cells.FontSourceBase---) | Définit les sources exclusives des polices. |
| [setFontFolder(String fontFolder, boolean recursive)](#setFontFolder-java.lang.String-boolean-) | Définit le dossier des polices |
| [setFontFolders(String[] fontFolders, boolean recursive)](#setFontFolders-java.lang.String---boolean-) | Définit les dossiers de polices |
| [setFontSources(FontSourceBase[] sources)](#setFontSources-com.aspose.cells.FontSourceBase---) | Définit les sources des polices. |
| [setFontSubstitutes(String originalFontName, String[] substituteFontNames)](#setFontSubstitutes-java.lang.String-java.lang.String---) | Définit les noms de polices de substitution pour un nom de police d'origine donné. |
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
| Paramètre | Type | Description |
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


Obtient une copie du tableau qui contient la liste des sources

**Returns:**
com.aspose.cells.FontSourceBase[] -
### getFontSubstitutes(String originalFontName) {#getFontSubstitutes-java.lang.String-}
```
public String[] getFontSubstitutes(String originalFontName)
```


Renvoie un tableau contenant les noms de polices de substitution à utiliser si la police d'origine n'est pas disponible.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| originalFontName | java.lang.String | originalFontName |

**Returns:**
java.lang.String[] - Un tableau contenant les noms de substitution de police à utiliser si la police originale n'est pas présentée.
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


Définit les sources exclusives des polices. Seules les polices présentes dans les sources seront utilisées.

**Remarks**

System.setProperty("Aspose.Cells.FontDirExc", "fontExclusiveFolder") sera ignoré si cela est défini.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| exclusiveSources | [FontSourceBase\[\]](../../com.aspose.cells/fontsourcebase) | Un tableau de sources contenant des polices TrueType. |

### setFontFolder(String fontFolder, boolean recursive) {#setFontFolder-java.lang.String-boolean-}
```
public void setFontFolder(String fontFolder, boolean recursive)
```


Définit le dossier des polices

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| fontFolder | java.lang.String | Le dossier contenant des polices TrueType. |
| recursive | boolean | Détermine s’il faut ou non analyser les sous‑dossiers. |

### setFontFolders(String[] fontFolders, boolean recursive) {#setFontFolders-java.lang.String---boolean-}
```
public void setFontFolders(String[] fontFolders, boolean recursive)
```


Définit les dossiers de polices

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| fontFolders | java.lang.String[] | Les dossiers contenant des polices TrueType. |
| recursive | boolean | Détermine s’il faut ou non analyser les sous‑dossiers. |

### setFontSources(FontSourceBase[] sources) {#setFontSources-com.aspose.cells.FontSourceBase---}
```
public void setFontSources(FontSourceBase[] sources)
```


Définit les sources des polices.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| sources | [FontSourceBase\[\]](../../com.aspose.cells/fontsourcebase) | Un tableau de sources contenant des polices TrueType. |

### setFontSubstitutes(String originalFontName, String[] substituteFontNames) {#setFontSubstitutes-java.lang.String-java.lang.String---}
```
public void setFontSubstitutes(String originalFontName, String[] substituteFontNames)
```


Définit les noms de polices de substitution pour un nom de police d'origine donné.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| originalFontName | java.lang.String | Nom de police original. |
| substituteFontNames | java.lang.String[] | Liste des noms de polices de substitution à utiliser si la police d'origine n'est pas présentée. |

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
| Paramètre | Type | Description |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

