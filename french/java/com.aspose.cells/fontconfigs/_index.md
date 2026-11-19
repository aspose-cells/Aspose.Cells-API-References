---
title: "FontConfigs"
second_title: "Référence API d'Aspose.Cells pour Java"
description: "Spécifie les paramètres de police"
type: docs
url: /fr/java/com.aspose.cells/fontconfigs/
---

**Inheritance:**
java.lang.Object
```
public class FontConfigs
```

Spécifie les paramètres de police
## Constructeurs

| Constructeur | Description |
| --- | --- |
| [FontConfigs()](#FontConfigs--) |  |
## Méthodes

| Méthode | Description |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getDefaultFontName()](#getDefaultFontName--) | Obtient le nom de police par défaut. |
| [getFontFileDataInfo(String fontName, boolean isBold, boolean isItalic, boolean isExactStyle)](#getFontFileDataInfo-java.lang.String-boolean-boolean-boolean-) | Obtenir les informations de données du fichier de police. |
| [getFontSources()](#getFontSources--) | Obtient une copie du tableau qui contient la liste des sources |
| [getFontSubstitutes(String originalFontName)](#getFontSubstitutes-java.lang.String-) | Renvoie un tableau contenant les noms de substitution de police à utiliser si la police originale n'est pas présente. |
| [hashCode()](#hashCode--) |  |
| [isFontAvailable(String fontName)](#isFontAvailable-java.lang.String-) | Indique si la police est disponible. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setDefaultFontName(String value)](#setDefaultFontName-java.lang.String-) | Définit le nom de police par défaut. |
| [setFontExclusiveSources(FontSourceBase[] exclusiveSources)](#setFontExclusiveSources-com.aspose.cells.FontSourceBase---) | Définit les sources exclusives des polices. |
| [setFontFolder(String fontFolder, boolean recursive)](#setFontFolder-java.lang.String-boolean-) | Définit le dossier des polices |
| [setFontFolders(String[] fontFolders, boolean recursive)](#setFontFolders-java.lang.String---boolean-) | Définit le dossier des polices |
| [setFontSources(FontSourceBase[] sources)](#setFontSources-com.aspose.cells.FontSourceBase---) | Définit les sources des polices. |
| [setFontSubstitutes(String originalFontName, String[] substituteFontNames)](#setFontSubstitutes-java.lang.String-java.lang.String---) | Noms de substitution de police pour le nom de police original donné. |
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
### getDefaultFontName() {#getDefaultFontName--}
```
public static String getDefaultFontName()
```


Obtient le nom de police par défaut.

**Returns:**
java.lang.String
### getFontFileDataInfo(String fontName, boolean isBold, boolean isItalic, boolean isExactStyle) {#getFontFileDataInfo-java.lang.String-boolean-boolean-boolean-}
```
public static FontFileDataInfo getFontFileDataInfo(String fontName, boolean isBold, boolean isItalic, boolean isExactStyle)
```


Obtenir les informations de données du fichier de police.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| fontName | java.lang.String | nom de police |
| isBold | boolean | le style de police est gras ou non |
| isItalic | boolean | le style de police est italique ou non |
| isExactStyle | boolean | si l’on doit correspondre exactement au style gras/italique donné |

**Returns:**
[FontFileDataInfo](../../com.aspose.cells/fontfiledatainfo) - Data infomation of font file data.
### getFontSources() {#getFontSources--}
```
public static FontSourceBase[] getFontSources()
```


Obtient une copie du tableau qui contient la liste des sources

**Returns:**
com.aspose.cells.FontSourceBase[] -
### getFontSubstitutes(String originalFontName) {#getFontSubstitutes-java.lang.String-}
```
public static String[] getFontSubstitutes(String originalFontName)
```


Renvoie un tableau contenant les noms de substitution de police à utiliser si la police originale n'est pas présente.

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
### isFontAvailable(String fontName) {#isFontAvailable-java.lang.String-}
```
public static boolean isFontAvailable(String fontName)
```


Indique si la police est disponible.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| fontName | java.lang.String | nom de police |

**Returns:**
boolean - vrai si la police est disponible, sinon faux.
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


Définit le nom de police par défaut.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

### setFontExclusiveSources(FontSourceBase[] exclusiveSources) {#setFontExclusiveSources-com.aspose.cells.FontSourceBase---}
```
public static void setFontExclusiveSources(FontSourceBase[] exclusiveSources)
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
public static void setFontFolder(String fontFolder, boolean recursive)
```


Définit le dossier des polices

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| fontFolder | java.lang.String | Le dossier contenant des polices TrueType. |
| recursive | boolean | Détermine s’il faut ou non analyser les sous‑dossiers. |

### setFontFolders(String[] fontFolders, boolean recursive) {#setFontFolders-java.lang.String---boolean-}
```
public static void setFontFolders(String[] fontFolders, boolean recursive)
```


Définit le dossier des polices

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| fontFolders | java.lang.String[] | Les dossiers contenant des polices TrueType. |
| recursive | boolean | Détermine s’il faut ou non analyser les sous‑dossiers. |

### setFontSources(FontSourceBase[] sources) {#setFontSources-com.aspose.cells.FontSourceBase---}
```
public static void setFontSources(FontSourceBase[] sources)
```


Définit les sources des polices.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| sources | [FontSourceBase\[\]](../../com.aspose.cells/fontsourcebase) | Un tableau de sources contenant des polices TrueType. |

### setFontSubstitutes(String originalFontName, String[] substituteFontNames) {#setFontSubstitutes-java.lang.String-java.lang.String---}
```
public static void setFontSubstitutes(String originalFontName, String[] substituteFontNames)
```


Noms de substitution de police pour le nom de police original donné.

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

