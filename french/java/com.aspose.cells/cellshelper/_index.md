---
title: "CellsHelper"
second_title: "Référence API d'Aspose.Cells pour Java"
description: "Fournit des fonctions d'aide."
type: docs
url: /fr/java/com.aspose.cells/cellshelper/
---

**Inheritance:**
java.lang.Object
```
public class CellsHelper
```

Fournit des fonctions d'aide.
## Méthodes

| Méthode | Description |
| --- | --- |
| [addAddInFunction(String function, int minCountOfParameters, int maxCountOfParameters, int[] paramersType, int functionValueType)](#addAddInFunction-java.lang.String-int-int-int---int-) | Ajouter la fonction d'extension. |
| [cellIndexToName(int row, int column)](#cellIndexToName-int-int-) | Obtient le nom de la cellule selon ses indices de ligne et de colonne. |
| [cellNameToIndex(String cellName)](#cellNameToIndex-java.lang.String-) | Obtient les indices de ligne et de colonne de la cellule selon son nom. |
| [columnIndexToName(int column)](#columnIndexToName-int-) | Obtient le nom de la colonne selon l'indice de colonne. |
| [columnNameToIndex(String columnName)](#columnNameToIndex-java.lang.String-) | Obtient l'indice de colonne selon le nom de la colonne. |
| [convertA1FormulaToR1C1(String formula, int row, int column)](#convertA1FormulaToR1C1-java.lang.String-int-int-) | Convertit la formule A1 de la cellule en formule r1c1. |
| [convertR1C1FormulaToA1(String r1c1Formula, int row, int column)](#convertR1C1FormulaToA1-java.lang.String-int-int-) | Convertit la formule r1c1 de la cellule en formule A1. |
| [createSafeSheetName(String nameProposal)](#createSafeSheetName-java.lang.String-) | Vérifie le nom de feuille fourni et crée un nom valide si nécessaire. |
| [createSafeSheetName(String nameProposal, char replaceChar)](#createSafeSheetName-java.lang.String-char-) | Vérifie le nom de feuille fourni et crée un nom valide si nécessaire. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAltStartPath()](#getAltStartPath--) | Obtient le chemin de démarrage alternatif, auquel font référence certaines références de formules externes. |
| [getCacheFolder()](#getCacheFolder--) | Obtient le dossier pour les fichiers temporaires pouvant être utilisés comme cache de données. |
| [getClass()](#getClass--) |  |
| [getCustomImplementationFactory()](#getCustomImplementationFactory--) | Obtient la fabrique pour créer des instances avec une implémentation spéciale. |
| [getDPI()](#getDPI--) | Obtient le DPI de la machine. |
| [getDateTimeFromDouble(double doubleValue, boolean date1904)](#getDateTimeFromDouble-double-boolean-) | Convertit la valeur double en valeur date‑heure. |
| [getDoubleFromDateTime(DateTime dateTime, boolean date1904)](#getDoubleFromDateTime-com.aspose.cells.DateTime-boolean-) | Convertit la date‑heure en valeur double. |
| [getLibraryPath()](#getLibraryPath--) | Obtient le chemin de la bibliothèque auquel font référence certaines références de formules externes. |
| [getSignificantDigits()](#getSignificantDigits--) | Obtient le nombre de chiffres significatifs. |
| [getSignificantDigitsType()](#getSignificantDigitsType--) | Obtient le type par défaut de chiffres significatifs pour la sortie des valeurs numériques. |
| [getStartupPath()](#getStartupPath--) | Obtient le chemin de démarrage auquel font référence certaines références de formules externes. |
| [getTextWidth(String text, Font font, double scaling)](#getTextWidth-java.lang.String-com.aspose.cells.Font-double-) | Obtient la largeur du texte en points. |
| [getUsedColors(Workbook workbook)](#getUsedColors-com.aspose.cells.Workbook-) | Obtient toutes les couleurs utilisées dans le classeur. |
| [getVersion()](#getVersion--) | Obtient la version de publication. |
| [hashCode()](#hashCode--) |  |
| [isCloudPlatform()](#isCloudPlatform--) | Veuillez définir cette propriété sur True lors de l'exécution sur une plateforme cloud, telle que : Azure, AWSLambda, etc, |
| [mergeFiles(String[] files, String cachedFile, String destFile)](#mergeFiles-java.lang.String---java.lang.String-java.lang.String-) | Fusionne plusieurs gros fichiers xls en un fichier xls. |
| [needQuoteInFormula(String sheetName)](#needQuoteInFormula-java.lang.String-) | Indique si le nom de la feuille doit être entouré de guillemets simples |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [rowIndexToName(int row)](#rowIndexToName-int-) | Obtient le nom de la ligne selon l'indice de ligne. |
| [rowNameToIndex(String rowName)](#rowNameToIndex-java.lang.String-) | Obtient l'indice de ligne selon le nom de la ligne. |
| [setAltStartPath(String value)](#setAltStartPath-java.lang.String-) | Définit le chemin de démarrage alternatif, auquel font référence certaines références de formules externes. |
| [setCacheFolder(String cache)](#setCacheFolder-java.lang.String-) | Définit le dossier pour les fichiers temporaires pouvant être utilisés comme cache de données. |
| [setCloudPlatform(boolean value)](#setCloudPlatform-boolean-) | Veuillez définir cette propriété sur True lors de l'exécution sur une plateforme cloud, telle que : Azure, AWSLambda, etc, |
| [setCustomImplementationFactory(CustomImplementationFactory value)](#setCustomImplementationFactory-com.aspose.cells.CustomImplementationFactory-) | Définit la fabrique pour créer des instances avec une implémentation spéciale. |
| [setDPI(double value)](#setDPI-double-) | Obtient le DPI de la machine. |
| [setLibraryPath(String value)](#setLibraryPath-java.lang.String-) | Définit le chemin de la bibliothèque auquel font référence certaines références de formules externes. |
| [setSignificantDigits(int value)](#setSignificantDigits-int-) | Définit le nombre de chiffres significatifs. |
| [setSignificantDigitsType(int value)](#setSignificantDigitsType-int-) | Définit le type par défaut de chiffres significatifs pour la sortie des valeurs numériques. |
| [setStartupPath(String value)](#setStartupPath-java.lang.String-) | Définit le chemin de démarrage, auquel font référence certaines références de formules externes. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### addAddInFunction(String function, int minCountOfParameters, int maxCountOfParameters, int[] paramersType, int functionValueType) {#addAddInFunction-java.lang.String-int-int-int---int-}
```
public static void addAddInFunction(String function, int minCountOfParameters, int maxCountOfParameters, int[] paramersType, int functionValueType)
```


Ajouter la fonction d'extension.

**Remarks**

NOTE : Ce membre est maintenant obsolète. À la place, veuillez utiliser les méthodes WorksheetCollection.RegisterAddInFunction(). Cette méthode sera supprimée 12 mois plus tard, depuis janvier 2022. Aspose s'excuse pour tout désagrément que vous auriez pu rencontrer.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| fonction | java.lang.String | Le nom de la fonction. |
| minCountOfParameters | int | Nombre minimum de paramètres requis par cette fonction |
| maxCountOfParameters | int | Nombre maximum de paramètres autorisés par cette fonction. |
| paramersType | int[] | [ParameterType](../../com.aspose.cells/parametertype). Le type de paramètres attendu de la fonction |
| functionValueType | int | [ParameterType](../../com.aspose.cells/parametertype). Le type de valeur de la fonction. |

### cellIndexToName(int row, int column) {#cellIndexToName-int-int-}
```
public static String cellIndexToName(int row, int column)
```


Obtient le nom de la cellule selon ses indices de ligne et de colonne.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| ligne | int | Indice de ligne. |
| colonne | int | Indice de colonne. |

**Returns:**
java.lang.String - Nom de la cellule.
### cellNameToIndex(String cellName) {#cellNameToIndex-java.lang.String-}
```
public static int[] cellNameToIndex(String cellName)
```


Obtient les indices de ligne et de colonne de la cellule selon son nom.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| cellName | java.lang.String | Nom de la cellule |

**Returns:**
int[] - [0] est l'indice de ligne et [1] est l'indice de colonne.
### columnIndexToName(int column) {#columnIndexToName-int-}
```
public static String columnIndexToName(int column)
```


Obtient le nom de la colonne selon l'indice de colonne.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| colonne | int | Indice de colonne. |

**Returns:**
java.lang.String - Nom de la colonne.
### columnNameToIndex(String columnName) {#columnNameToIndex-java.lang.String-}
```
public static int columnNameToIndex(String columnName)
```


Obtient l'indice de colonne selon le nom de la colonne.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| columnName | java.lang.String | Nom de la colonne. |

**Returns:**
int - Indice de colonne.
### convertA1FormulaToR1C1(String formula, int row, int column) {#convertA1FormulaToR1C1-java.lang.String-int-int-}
```
public static String convertA1FormulaToR1C1(String formula, int row, int column)
```


Convertit la formule A1 de la cellule en formule r1c1.

**Remarks**

NOTE : Ce membre est maintenant obsolète. À la place, veuillez utiliser la méthode Worksheet.ConvertFormulaReferenceStyle(). Cette propriété sera supprimée 12 mois plus tard, depuis août 2023. Aspose s'excuse pour tout désagrément que vous auriez pu rencontrer.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| formula | java.lang.String | La formule A1. |
| ligne | int | L'indice de ligne de la cellule. |
| colonne | int | L'index de colonne de la cellule. |

**Returns:**
java.lang.String - La formule R1C1.
### convertR1C1FormulaToA1(String r1c1Formula, int row, int column) {#convertR1C1FormulaToA1-java.lang.String-int-int-}
```
public static String convertR1C1FormulaToA1(String r1c1Formula, int row, int column)
```


Convertit la formule r1c1 de la cellule en formule A1.

**Remarks**

NOTE : Ce membre est maintenant obsolète. À la place, veuillez utiliser la méthode Worksheet.ConvertFormulaReferenceStyle(). Cette propriété sera supprimée 12 mois plus tard, depuis août 2023. Aspose s'excuse pour tout désagrément que vous auriez pu rencontrer.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| r1c1Formula | java.lang.String | La formule r1c1. |
| ligne | int | L'indice de ligne de la cellule. |
| colonne | int | L'index de colonne de la cellule. |

**Returns:**
java.lang.String - La formule A1.
### createSafeSheetName(String nameProposal) {#createSafeSheetName-java.lang.String-}
```
public static String createSafeSheetName(String nameProposal)
```


Vérifie le nom de feuille fourni et crée un nom valide si nécessaire. Si le nom de feuille fourni respecte les règles de nommage des feuilles Excel, il est renvoyé. Sinon, la chaîne sera tronquée si sa longueur dépasse la limite et les caractères invalides seront remplacés par ' ', puis la valeur de chaîne reconstruite sera renvoyée.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| nameProposal | java.lang.String | nom de feuille à utiliser |

**Returns:**
java.lang.String -
### createSafeSheetName(String nameProposal, char replaceChar) {#createSafeSheetName-java.lang.String-char-}
```
public static String createSafeSheetName(String nameProposal, char replaceChar)
```


Vérifie le nom de feuille fourni et crée un nom valide si nécessaire. Si le nom de feuille fourni respecte les règles de nommage des feuilles Excel, il est renvoyé. Sinon, la chaîne sera tronquée si sa longueur dépasse la limite et les caractères invalides seront remplacés par le caractère fourni, puis la valeur de chaîne reconstruite sera renvoyée.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| nameProposal | java.lang.String | nom de feuille à utiliser |
| replaceChar | char | caractère qui sera utilisé pour remplacer les caractères invalides dans le nom de feuille fourni |

**Returns:**
java.lang.String -
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
### getAltStartPath() {#getAltStartPath--}
```
public static String getAltStartPath()
```


Obtient le chemin de démarrage alternatif, auquel font référence certaines références de formules externes.

**Returns:**
java.lang.String
### getCacheFolder() {#getCacheFolder--}
```
public static String getCacheFolder()
```


Obtient le dossier pour les fichiers temporaires pouvant être utilisés comme cache de données.

**Remarks**

Les fichiers cache sont généralement utilisés pour certaines fonctionnalités afin d'optimiser les performances mémoire, comme l'enregistrement d'un grand ensemble de données dans un fichier xls, ou l'utilisation du mode mémoire avec cache de fichiers pour le modèle de cellules.

**Returns:**
java.lang.String - Dossier pour les fichiers cache qui a été spécifié. S'il n'a pas été spécifié, null sera renvoyé et le chemin temporaire du système sera utilisé si nécessaire.
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getCustomImplementationFactory() {#getCustomImplementationFactory--}
```
public static CustomImplementationFactory getCustomImplementationFactory()
```


Obtient la fabrique pour créer des instances avec une implémentation spéciale.

**Returns:**
[CustomImplementationFactory](../../com.aspose.cells/customimplementationfactory)
### getDPI() {#getDPI--}
```
public static double getDPI()
```


Obtient le DPI de la machine.

**Remarks**

**Returns:**
double
### getDateTimeFromDouble(double doubleValue, boolean date1904) {#getDateTimeFromDouble-double-boolean-}
```
public static DateTime getDateTimeFromDouble(double doubleValue, boolean date1904)
```


Convertit la valeur double en valeur date‑heure.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| doubleValue | double | La valeur double. |
| date1904 | boolean | Système de date 1904. |

**Returns:**
[DateTime](../../com.aspose.cells/datetime) - 
### getDoubleFromDateTime(DateTime dateTime, boolean date1904) {#getDoubleFromDateTime-com.aspose.cells.DateTime-boolean-}
```
public static double getDoubleFromDateTime(DateTime dateTime, boolean date1904)
```


Convertit la date‑heure en valeur double.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| dateTime | [DateTime](../../com.aspose.cells/datetime) | La date et l'heure. |
| date1904 | boolean | Système de date 1904. |

**Returns:**
double -
### getLibraryPath() {#getLibraryPath--}
```
public static String getLibraryPath()
```


Obtient le chemin de la bibliothèque auquel font référence certaines références de formules externes.

**Returns:**
java.lang.String
### getSignificantDigits() {#getSignificantDigits--}
```
public static int getSignificantDigits()
```


Obtient le nombre de chiffres significatifs. La valeur par défaut est 17.

**Remarks**

Ne peut être que 15 ou 17 actuellement. NOTE : Ce membre est maintenant obsolète. À la place, veuillez utiliser [getSignificantDigitsType()](../../com.aspose.cells/cellshelper\#getSignificantDigitsType--). Cette propriété sera supprimée 12 mois plus tard, à partir de juin 2025. Aspose s'excuse pour tout désagrément que vous auriez pu rencontrer.

**Returns:**
int
### getSignificantDigitsType() {#getSignificantDigitsType--}
```
public static int getSignificantDigitsType()
```


Obtient le type par défaut de chiffres significatifs pour la sortie des valeurs numériques. La valeur par défaut est [SignificantDigitsType.G\_17](../../com.aspose.cells/significantdigitstype\#G-17).

Voir [SignificantDigitsType](../../com.aspose.cells/significantdigitstype).

**Returns:**
int
### getStartupPath() {#getStartupPath--}
```
public static String getStartupPath()
```


Obtient le chemin de démarrage auquel font référence certaines références de formules externes.

**Returns:**
java.lang.String
### getTextWidth(String text, Font font, double scaling) {#getTextWidth-java.lang.String-com.aspose.cells.Font-double-}
```
public static double getTextWidth(String text, Font font, double scaling)
```


Obtient la largeur du texte en points.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| texte | java.lang.String | Le texte. |
| font | [Font](../../com.aspose.cells/font) | La police du texte. |
| mise à l'échelle | double | Le redimensionnement du texte. |

**Returns:**
double -
### getUsedColors(Workbook workbook) {#getUsedColors-com.aspose.cells.Workbook-}
```
public static Color[] getUsedColors(Workbook workbook)
```


Obtient toutes les couleurs utilisées dans le classeur.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| workbook | [Workbook](../../com.aspose.cells/workbook) | L'objet classeur. |

**Returns:**
com.aspose.cells.Color[] - Les couleurs utilisées.
### getVersion() {#getVersion--}
```
public static String getVersion()
```


Obtient la version de publication.

**Returns:**
java.lang.String - La version de publication.
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isCloudPlatform() {#isCloudPlatform--}
```
public static boolean isCloudPlatform()
```


Veuillez définir cette propriété sur True lors de l'exécution sur une plateforme cloud, telle que : Azure, AWSLambda, etc,

**Returns:**
boolean
### mergeFiles(String[] files, String cachedFile, String destFile) {#mergeFiles-java.lang.String---java.lang.String-java.lang.String-}
```
public static void mergeFiles(String[] files, String cachedFile, String destFile)
```


Fusionne plusieurs gros fichiers xls en un fichier xls.

**Remarks**

Cette méthode ne prend en charge que la fusion des données, du style et des formules dans le nouveau fichier. Le fichier en cache est utilisé pour stocker certaines données temporaires.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| fichiers | java.lang.String[] | Les fichiers. |
| cachedFile | java.lang.String | Le fichier en cache. |
| destFile | java.lang.String | Le fichier de destination. |

### needQuoteInFormula(String sheetName) {#needQuoteInFormula-java.lang.String-}
```
public static boolean needQuoteInFormula(String sheetName)
```


Indique si le nom de la feuille doit être entouré de guillemets simples

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| sheetName | java.lang.String | Le nom de la feuille |

**Returns:**
boolean -
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### rowIndexToName(int row) {#rowIndexToName-int-}
```
public static String rowIndexToName(int row)
```


Obtient le nom de la ligne selon l'indice de ligne.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| ligne | int | Indice de ligne. |

**Returns:**
java.lang.String - Nom de la ligne.
### rowNameToIndex(String rowName) {#rowNameToIndex-java.lang.String-}
```
public static int rowNameToIndex(String rowName)
```


Obtient l'indice de ligne selon le nom de la ligne.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| rowName | java.lang.String | Nom de la ligne. |

**Returns:**
int - Index de la ligne.
### setAltStartPath(String value) {#setAltStartPath-java.lang.String-}
```
public static void setAltStartPath(String value)
```


Définit le chemin de démarrage alternatif, auquel font référence certaines références de formules externes.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

### setCacheFolder(String cache) {#setCacheFolder-java.lang.String-}
```
public static void setCacheFolder(String cache)
```


Définit le dossier pour les fichiers temporaires pouvant être utilisés comme cache de données.

**Remarks**

Les fichiers cache sont généralement utilisés pour certaines fonctionnalités afin d'optimiser les performances mémoire, comme l'enregistrement d'un grand ensemble de données dans un fichier xls, ou l'utilisation du mode mémoire avec cache de fichiers pour le modèle de cellules.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| cache | java.lang.String | Dossier pour les fichiers temporaires pouvant être utilisés comme cache de données. |

### setCloudPlatform(boolean value) {#setCloudPlatform-boolean-}
```
public static void setCloudPlatform(boolean value)
```


Veuillez définir cette propriété sur True lors de l'exécution sur une plateforme cloud, telle que : Azure, AWSLambda, etc,

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setCustomImplementationFactory(CustomImplementationFactory value) {#setCustomImplementationFactory-com.aspose.cells.CustomImplementationFactory-}
```
public static void setCustomImplementationFactory(CustomImplementationFactory value)
```


Définit la fabrique pour créer des instances avec une implémentation spéciale.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | [CustomImplementationFactory](../../com.aspose.cells/customimplementationfactory) |  |

### setDPI(double value) {#setDPI-double-}
```
public static void setDPI(double value)
```


Obtient le DPI de la machine.

**Remarks**

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | double |  |

### setLibraryPath(String value) {#setLibraryPath-java.lang.String-}
```
public static void setLibraryPath(String value)
```


Définit le chemin de la bibliothèque auquel font référence certaines références de formules externes.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

### setSignificantDigits(int value) {#setSignificantDigits-int-}
```
public static void setSignificantDigits(int value)
```


Définit le nombre de chiffres significatifs. La valeur par défaut est 17.

**Remarks**

Ne peut être que 15 ou 17 actuellement. NOTE : Ce membre est maintenant obsolète. À la place, veuillez utiliser [getSignificantDigitsType()](../../com.aspose.cells/cellshelper\#getSignificantDigitsType--). Cette propriété sera supprimée 12 mois plus tard, à partir de juin 2025. Aspose s'excuse pour tout désagrément que vous auriez pu rencontrer.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setSignificantDigitsType(int value) {#setSignificantDigitsType-int-}
```
public static void setSignificantDigitsType(int value)
```


Définit le type par défaut de chiffres significatifs pour la sortie des valeurs numériques. La valeur par défaut est [SignificantDigitsType.G\_17](../../com.aspose.cells/significantdigitstype\#G-17).

Voir [SignificantDigitsType](../../com.aspose.cells/significantdigitstype).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setStartupPath(String value) {#setStartupPath-java.lang.String-}
```
public static void setStartupPath(String value)
```


Définit le chemin de démarrage, auquel font référence certaines références de formules externes.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

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

