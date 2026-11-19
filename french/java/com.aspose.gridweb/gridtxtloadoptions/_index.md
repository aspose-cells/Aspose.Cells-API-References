---
title: "GridTxtLoadOptions"
second_title: "Référence API d'Aspose.Cells pour Java"
description: "Représente les options de chargement du fichier texte."
type: docs
url: /fr/java/com.aspose.gridweb/gridtxtloadoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.gridweb.GridLoadOptions](../../com.aspose.gridweb/gridloadoptions)
```
public class GridTxtLoadOptions extends GridLoadOptions
```

Représente les options de chargement du fichier texte.
## Constructeurs

| Constructeur | Description |
| --- | --- |
| [GridTxtLoadOptions()](#GridTxtLoadOptions--) | Crée les options pour charger un fichier texte. |
## Méthodes

| Méthode | Description |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAutoFilter()](#getAutoFilter--) | Indique si le filtrage automatique des données est effectué lors du chargement des fichiers. |
| [getCheckDataValid()](#getCheckDataValid--) | Vérifie si les données sont valides dans le fichier modèle. |
| [getCheckExcelRestriction()](#getCheckExcelRestriction--) | Indique si la vérification des restrictions du fichier Excel est effectuée lorsque l'utilisateur modifie les objets liés aux cellules. |
| [getClass()](#getClass--) |  |
| [getConvertDateTimeData()](#getConvertDateTimeData--) | Obtient une valeur qui indique si la chaîne dans le fichier texte est convertie en données de date. |
| [getConvertNumericData()](#getConvertNumericData--) | Obtient une valeur qui indique si la chaîne dans le fichier texte est convertie en données numériques. |
| [getEncoding()](#getEncoding--) | Obtient le codage par défaut. |
| [getExtendToNextSheet()](#getExtendToNextSheet--) | Indique si les données sont étendues à la feuille suivante lorsque les lignes ou colonnes dépassent la limite. |
| [getIgnoreNotPrinted()](#getIgnoreNotPrinted--) | Ignore les données qui ne sont pas imprimées lors de l'impression directe du fichier |
| [getKeepPrecision()](#getKeepPrecision--) | Indique s'il ne faut pas analyser une valeur de chaîne si la longueur est de 15. |
| [getKeepUnparsedData()](#getKeepUnparsedData--) | Indique si les données non analysées sont conservées en mémoire pour le classeur lorsqu'il est chargé à partir du fichier modèle. |
| [getOnlyAuto()](#getOnlyAuto--) | Indique si seules les lignes dont la hauteur n'est pas personnalisée sont ajustées. |
| [getParsingFormulaOnOpen()](#getParsingFormulaOnOpen--) | Indique si la formule est analysée lors de la lecture du fichier. |
| [getParsingPivotCachedRecords()](#getParsingPivotCachedRecords--) | Indique si les enregistrements mis en cache du tableau croisé dynamique sont analysés lors du chargement du fichier. |
| [getPassword()](#getPassword--) | Obtient le mot de passe du classeur. |
| [getPreservePaddingSpacesInFormula()](#getPreservePaddingSpacesInFormula--) | Indique s'il faut préserver les espaces et les sauts de ligne insérés entre les jetons de formule lors de l'obtention et de la définition des formules. |
| [getSeparator()](#getSeparator--) | Obtient le séparateur de caractères du fichier texte. |
| [getSeparatorString()](#getSeparatorString--) | Obtient une valeur chaîne comme séparateur. |
| [getTextQualifier()](#getTextQualifier--) | Spécifie le qualificateur de texte pour les valeurs des cellules. |
| [getTreatConsecutiveDelimitersAsOne()](#getTreatConsecutiveDelimitersAsOne--) | Indique si les délimiteurs consécutifs doivent être traités comme un seul. |
| [getTreatQuotePrefixAsValue()](#getTreatQuotePrefixAsValue--) | Indique si le signe de guillemet simple en début doit être considéré comme faisant partie de la valeur d’une cellule. |
| [hasFormula()](#hasFormula--) | Indique si le texte est une formule s'il commence par "=". |
| [hasTextQualifier()](#hasTextQualifier--) | Indique s’il existe un qualificateur de texte pour la valeur d’une cellule. |
| [hashCode()](#hashCode--) |  |
| [isMultiEncoded()](#isMultiEncoded--) | Vrai signifie que le fichier contient plusieurs encodages. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAutoFilter(boolean value)](#setAutoFilter-boolean-) | Indique si le filtrage automatique des données est effectué lors du chargement des fichiers. |
| [setCheckDataValid(boolean value)](#setCheckDataValid-boolean-) | Vérifie si les données sont valides dans le fichier modèle. |
| [setCheckExcelRestriction(boolean value)](#setCheckExcelRestriction-boolean-) | Indique si la vérification des restrictions du fichier Excel est effectuée lorsque l'utilisateur modifie les objets liés aux cellules. |
| [setConvertDateTimeData(boolean value)](#setConvertDateTimeData-boolean-) | Définit une valeur qui indique si la chaîne du fichier texte est convertie en données de date. |
| [setConvertNumericData(boolean value)](#setConvertNumericData-boolean-) | Définit une valeur qui indique si la chaîne du fichier texte est convertie en données numériques. |
| [setEncoding(Encoding value)](#setEncoding-com.aspose.gridweb.Encoding-) | Définit le codage par défaut. |
| [setExtendToNextSheet(boolean value)](#setExtendToNextSheet-boolean-) | Indique si les données sont étendues à la feuille suivante lorsque les lignes ou colonnes dépassent la limite. |
| [setHasFormula(boolean value)](#setHasFormula-boolean-) | Indique si le texte est une formule s'il commence par "=". |
| [setHasTextQualifier(boolean value)](#setHasTextQualifier-boolean-) | Indique s’il existe un qualificateur de texte pour la valeur d’une cellule. |
| [setIgnoreNotPrinted(boolean value)](#setIgnoreNotPrinted-boolean-) | Ignore les données qui ne sont pas imprimées lors de l'impression directe du fichier |
| [setKeepPrecision(boolean value)](#setKeepPrecision-boolean-) | Indique s'il ne faut pas analyser une valeur de chaîne si la longueur est de 15. |
| [setKeepUnparsedData(boolean value)](#setKeepUnparsedData-boolean-) | Indique si les données non analysées sont conservées en mémoire pour le classeur lorsqu'il est chargé à partir du fichier modèle. |
| [setMultiEncoded(boolean value)](#setMultiEncoded-boolean-) | Vrai signifie que le fichier contient plusieurs encodages. |
| [setOnlyAuto(boolean value)](#setOnlyAuto-boolean-) | Indique si seules les lignes dont la hauteur n'est pas personnalisée sont ajustées. |
| [setParsingFormulaOnOpen(boolean value)](#setParsingFormulaOnOpen-boolean-) | Indique si la formule est analysée lors de la lecture du fichier. |
| [setParsingPivotCachedRecords(boolean value)](#setParsingPivotCachedRecords-boolean-) | Indique si les enregistrements mis en cache du tableau croisé dynamique sont analysés lors du chargement du fichier. |
| [setPassword(String value)](#setPassword-java.lang.String-) | Définit le mot de passe du classeur. |
| [setPreservePaddingSpacesInFormula(boolean value)](#setPreservePaddingSpacesInFormula-boolean-) | Indique s'il faut préserver les espaces et les sauts de ligne insérés entre les jetons de formule lors de l'obtention et de la définition des formules. |
| [setSeparator(char value)](#setSeparator-char-) | Définit le séparateur de caractères du fichier texte. |
| [setSeparatorString(String value)](#setSeparatorString-java.lang.String-) | Définit une valeur chaîne comme séparateur. |
| [setTextQualifier(char value)](#setTextQualifier-char-) | Spécifie le qualificateur de texte pour les valeurs des cellules. |
| [setTreatConsecutiveDelimitersAsOne(boolean value)](#setTreatConsecutiveDelimitersAsOne-boolean-) | Indique si les délimiteurs consécutifs doivent être traités comme un seul. |
| [setTreatQuotePrefixAsValue(boolean value)](#setTreatQuotePrefixAsValue-boolean-) | Indique si le signe de guillemet simple en début doit être considéré comme faisant partie de la valeur d’une cellule. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### GridTxtLoadOptions() {#GridTxtLoadOptions--}
```
public GridTxtLoadOptions()
```


Crée les options pour charger un fichier texte.

**Remarks**

Le type de fichier chargé par défaut est CSV.

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
### getAutoFilter() {#getAutoFilter--}
```
public boolean getAutoFilter()
```


Indique si le filtrage automatique des données est effectué lors du chargement des fichiers.

**Remarks**

Parfois, même si le filtre automatique est activé, les lignes correspondantes ne sont pas masquées dans le fichier. Fonctionne désormais uniquement pour le fichier SpreadSheetML.

**Returns:**
boolean
### getCheckDataValid() {#getCheckDataValid--}
```
public boolean getCheckDataValid()
```


Vérifie si les données sont valides dans le fichier modèle.

**Returns:**
boolean
### getCheckExcelRestriction() {#getCheckExcelRestriction--}
```
public boolean getCheckExcelRestriction()
```


Indique s’il faut vérifier les restrictions du fichier Excel lorsque l’utilisateur modifie des objets liés aux cellules. Par exemple, Excel n’autorise pas la saisie d’une chaîne de caractères supérieure à 32 K. Lorsque vous saisissez une valeur supérieure à 32 K, par exemple avec Cell.PutValue(string), si cette propriété est vraie, vous obtiendrez une exception. Si cette propriété est fausse, nous accepterons votre chaîne saisie comme valeur de la cellule afin que vous puissiez ensuite exporter la chaîne complète vers d’autres formats de fichier tels que CSV. Cependant, si vous avez défini une valeur qui n’est pas valide pour le format de fichier Excel, vous ne devez pas enregistrer le classeur au format Excel ultérieurement. Sinon, il peut y avoir des erreurs inattendues dans le fichier Excel généré.

**Returns:**
boolean
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getConvertDateTimeData() {#getConvertDateTimeData--}
```
public boolean getConvertDateTimeData()
```


Obtient une valeur qui indique si la chaîne dans le fichier texte est convertie en données de date.

**Returns:**
boolean
### getConvertNumericData() {#getConvertNumericData--}
```
public boolean getConvertNumericData()
```


Obtient une valeur qui indique si la chaîne dans le fichier texte est convertie en données numériques.

**Returns:**
boolean
### getEncoding() {#getEncoding--}
```
public Encoding getEncoding()
```


Obtient le codage par défaut. S'applique uniquement aux fichiers csv.

**Returns:**
[Encoding](../../com.aspose.gridweb/encoding)
### getExtendToNextSheet() {#getExtendToNextSheet--}
```
public boolean getExtendToNextSheet()
```


Indique si les données sont étendues à la feuille suivante lorsque les lignes ou colonnes des données dépassent la limite. Si cette propriété est vraie, les données supplémentaires seront étendues à la feuille suivante derrière la feuille actuelle (si la feuille actuelle est la dernière, une nouvelle feuille sera ajoutée au classeur actuel). Si cette propriété est fausse, les données dépassant la limite seront ignorées. La valeur par défaut est false;

**Returns:**
boolean
### getIgnoreNotPrinted() {#getIgnoreNotPrinted--}
```
public boolean getIgnoreNotPrinted()
```


Ignore les données qui ne sont pas imprimées lors de l'impression directe du fichier

**Remarks**

Uniquement pour le fichier xlsx.

**Returns:**
boolean
### getKeepPrecision() {#getKeepPrecision--}
```
public boolean getKeepPrecision()
```


Indique s'il ne faut pas analyser une valeur de chaîne si la longueur est de 15.

**Returns:**
boolean
### getKeepUnparsedData() {#getKeepUnparsedData--}
```
public boolean getKeepUnparsedData()
```


Indique s’il faut conserver les données non analysées en mémoire pour le Workbook lorsqu’il est chargé depuis un fichier modèle. La valeur par défaut est vraie.

**Remarks**

Dans les scénarios où l’utilisateur n’a besoin que de lire certains contenus du fichier modèle et n’a pas besoin d’enregistrer à nouveau le classeur, définir cette propriété à false peut améliorer les performances, notamment lorsqu’elle est utilisée conjointement avec un certain type de LoadFilter,

**Returns:**
boolean
### getOnlyAuto() {#getOnlyAuto--}
```
public boolean getOnlyAuto()
```


Indique si seules les lignes dont la hauteur n'est pas personnalisée sont ajustées.

**Returns:**
boolean
### getParsingFormulaOnOpen() {#getParsingFormulaOnOpen--}
```
public boolean getParsingFormulaOnOpen()
```


Indique si la formule est analysée lors de la lecture du fichier.

**Remarks**

S’applique uniquement aux fichiers Excel Xlsx, Xltx, Xltm et Xlsm car les formules dans ces fichiers sont stockées sous forme de chaîne de caractères.

**Returns:**
boolean
### getParsingPivotCachedRecords() {#getParsingPivotCachedRecords--}
```
public boolean getParsingPivotCachedRecords()
```


Indique s’il faut analyser les enregistrements mis en cache du tableau croisé dynamique lors du chargement du fichier. La valeur par défaut est false.

**Remarks**

S’applique uniquement aux fichiers Excel Xlsx, Xltx, Xltm, Xlsm et xlsb.

**Returns:**
boolean
### getPassword() {#getPassword--}
```
public String getPassword()
```


Obtient le mot de passe du classeur.

**Returns:**
java.lang.String
### getPreservePaddingSpacesInFormula() {#getPreservePaddingSpacesInFormula--}
```
public boolean getPreservePaddingSpacesInFormula()
```


Indique s'il faut conserver les espaces et les sauts de ligne qui sont remplis entre les jetons de formule lors de la lecture et de l'écriture des formules. La valeur par défaut est false.

**Remarks**

Après le chargement du classeur à partir d'un fichier modèle avec cette option, [GridWorkbookSettings.getPreservePaddingSpaces()](../../com.aspose.gridweb/gridworkbooksettings\\#getPreservePaddingSpaces--) sera défini sur la même valeur que cette propriété.

**Returns:**
boolean
### getSeparator() {#getSeparator--}
```
public char getSeparator()
```


Obtient le séparateur de caractères du fichier texte.

**Returns:**
char
### getSeparatorString() {#getSeparatorString--}
```
public String getSeparatorString()
```


Obtient une valeur chaîne comme séparateur.

**Returns:**
java.lang.String
### getTextQualifier() {#getTextQualifier--}
```
public char getTextQualifier()
```


Spécifie le qualificateur de texte pour les valeurs des cellules. Le qualificateur par défaut est '\"'.

**Remarks**

Lors de la définition de cette propriété, [hasTextQualifier()](../../com.aspose.gridweb/gridtxtloadoptions\#hasTextQualifier--) deviendra true automatiquement.

**Returns:**
char
### getTreatConsecutiveDelimitersAsOne() {#getTreatConsecutiveDelimitersAsOne--}
```
public boolean getTreatConsecutiveDelimitersAsOne()
```


Indique si les délimiteurs consécutifs doivent être traités comme un seul.

**Returns:**
boolean
### getTreatQuotePrefixAsValue() {#getTreatQuotePrefixAsValue--}
```
public boolean getTreatQuotePrefixAsValue()
```


Indique si le signe de guillemet simple initial doit être considéré comme faisant partie de la valeur d'une cellule. La valeur par défaut est true. Si elle est false, le guillemet simple initial sera supprimé de la valeur de la cellule correspondante et [GridTableItemStyle.getQuotePrefix()](../../com.aspose.gridweb/gridtableitemstyle\#getQuotePrefix--) sera défini sur true pour la cellule.

**Returns:**
boolean
### hasFormula() {#hasFormula--}
```
public boolean hasFormula()
```


Indique si le texte est une formule s'il commence par "=".

**Returns:**
boolean
### hasTextQualifier() {#hasTextQualifier--}
```
public boolean hasTextQualifier()
```


Indique s’il existe un qualificateur de texte pour la valeur d’une cellule. La valeur par défaut est true.

**Returns:**
boolean
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isMultiEncoded() {#isMultiEncoded--}
```
public boolean isMultiEncoded()
```


Vrai signifie que le fichier contient plusieurs encodages.

**Returns:**
boolean
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### setAutoFilter(boolean value) {#setAutoFilter-boolean-}
```
public void setAutoFilter(boolean value)
```


Indique si le filtrage automatique des données est effectué lors du chargement des fichiers.

**Remarks**

Parfois, même si le filtre automatique est activé, les lignes correspondantes ne sont pas masquées dans le fichier. Fonctionne désormais uniquement pour le fichier SpreadSheetML.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setCheckDataValid(boolean value) {#setCheckDataValid-boolean-}
```
public void setCheckDataValid(boolean value)
```


Vérifie si les données sont valides dans le fichier modèle.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setCheckExcelRestriction(boolean value) {#setCheckExcelRestriction-boolean-}
```
public void setCheckExcelRestriction(boolean value)
```


Indique s’il faut vérifier les restrictions du fichier Excel lorsque l’utilisateur modifie des objets liés aux cellules. Par exemple, Excel n’autorise pas la saisie d’une chaîne de caractères supérieure à 32 K. Lorsque vous saisissez une valeur supérieure à 32 K, par exemple avec Cell.PutValue(string), si cette propriété est vraie, vous obtiendrez une exception. Si cette propriété est fausse, nous accepterons votre chaîne saisie comme valeur de la cellule afin que vous puissiez ensuite exporter la chaîne complète vers d’autres formats de fichier tels que CSV. Cependant, si vous avez défini une valeur qui n’est pas valide pour le format de fichier Excel, vous ne devez pas enregistrer le classeur au format Excel ultérieurement. Sinon, il peut y avoir des erreurs inattendues dans le fichier Excel généré.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setConvertDateTimeData(boolean value) {#setConvertDateTimeData-boolean-}
```
public void setConvertDateTimeData(boolean value)
```


Définit une valeur qui indique si la chaîne du fichier texte est convertie en données de date.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setConvertNumericData(boolean value) {#setConvertNumericData-boolean-}
```
public void setConvertNumericData(boolean value)
```


Définit une valeur qui indique si la chaîne du fichier texte est convertie en données numériques.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setEncoding(Encoding value) {#setEncoding-com.aspose.gridweb.Encoding-}
```
public void setEncoding(Encoding value)
```


Définit l’encodage par défaut. S’applique uniquement aux fichiers csv.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | [Encoding](../../com.aspose.gridweb/encoding) |  |

### setExtendToNextSheet(boolean value) {#setExtendToNextSheet-boolean-}
```
public void setExtendToNextSheet(boolean value)
```


Indique si les données sont étendues à la feuille suivante lorsque les lignes ou colonnes des données dépassent la limite. Si cette propriété est vraie, les données supplémentaires seront étendues à la feuille suivante derrière la feuille actuelle (si la feuille actuelle est la dernière, une nouvelle feuille sera ajoutée au classeur actuel). Si cette propriété est fausse, les données dépassant la limite seront ignorées. La valeur par défaut est false;

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setHasFormula(boolean value) {#setHasFormula-boolean-}
```
public void setHasFormula(boolean value)
```


Indique si le texte est une formule s'il commence par "=".

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setHasTextQualifier(boolean value) {#setHasTextQualifier-boolean-}
```
public void setHasTextQualifier(boolean value)
```


Indique s’il existe un qualificateur de texte pour la valeur d’une cellule. La valeur par défaut est true.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setIgnoreNotPrinted(boolean value) {#setIgnoreNotPrinted-boolean-}
```
public void setIgnoreNotPrinted(boolean value)
```


Ignore les données qui ne sont pas imprimées lors de l'impression directe du fichier

**Remarks**

Uniquement pour le fichier xlsx.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setKeepPrecision(boolean value) {#setKeepPrecision-boolean-}
```
public void setKeepPrecision(boolean value)
```


Indique s'il ne faut pas analyser une valeur de chaîne si la longueur est de 15.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setKeepUnparsedData(boolean value) {#setKeepUnparsedData-boolean-}
```
public void setKeepUnparsedData(boolean value)
```


Indique s’il faut conserver les données non analysées en mémoire pour le Workbook lorsqu’il est chargé depuis un fichier modèle. La valeur par défaut est vraie.

**Remarks**

Dans les scénarios où l’utilisateur n’a besoin que de lire certains contenus du fichier modèle et n’a pas besoin d’enregistrer à nouveau le classeur, définir cette propriété à false peut améliorer les performances, notamment lorsqu’elle est utilisée conjointement avec un certain type de LoadFilter,

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setMultiEncoded(boolean value) {#setMultiEncoded-boolean-}
```
public void setMultiEncoded(boolean value)
```


Vrai signifie que le fichier contient plusieurs encodages.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setOnlyAuto(boolean value) {#setOnlyAuto-boolean-}
```
public void setOnlyAuto(boolean value)
```


Indique si seules les lignes dont la hauteur n'est pas personnalisée sont ajustées.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setParsingFormulaOnOpen(boolean value) {#setParsingFormulaOnOpen-boolean-}
```
public void setParsingFormulaOnOpen(boolean value)
```


Indique si la formule est analysée lors de la lecture du fichier.

**Remarks**

S’applique uniquement aux fichiers Excel Xlsx, Xltx, Xltm et Xlsm car les formules dans ces fichiers sont stockées sous forme de chaîne de caractères.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setParsingPivotCachedRecords(boolean value) {#setParsingPivotCachedRecords-boolean-}
```
public void setParsingPivotCachedRecords(boolean value)
```


Indique s’il faut analyser les enregistrements mis en cache du tableau croisé dynamique lors du chargement du fichier. La valeur par défaut est false.

**Remarks**

S’applique uniquement aux fichiers Excel Xlsx, Xltx, Xltm, Xlsm et xlsb.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setPassword(String value) {#setPassword-java.lang.String-}
```
public void setPassword(String value)
```


Définit le mot de passe du classeur.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

### setPreservePaddingSpacesInFormula(boolean value) {#setPreservePaddingSpacesInFormula-boolean-}
```
public void setPreservePaddingSpacesInFormula(boolean value)
```


Indique s'il faut conserver les espaces et les sauts de ligne qui sont remplis entre les jetons de formule lors de la lecture et de l'écriture des formules. La valeur par défaut est false.

**Remarks**

Après le chargement du classeur à partir d'un fichier modèle avec cette option, [GridWorkbookSettings.getPreservePaddingSpaces()](../../com.aspose.gridweb/gridworkbooksettings\\#getPreservePaddingSpaces--) sera défini sur la même valeur que cette propriété.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setSeparator(char value) {#setSeparator-char-}
```
public void setSeparator(char value)
```


Définit le séparateur de caractères du fichier texte.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | char |  |

### setSeparatorString(String value) {#setSeparatorString-java.lang.String-}
```
public void setSeparatorString(String value)
```


Définit une valeur chaîne comme séparateur.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

### setTextQualifier(char value) {#setTextQualifier-char-}
```
public void setTextQualifier(char value)
```


Spécifie le qualificateur de texte pour les valeurs des cellules. Le qualificateur par défaut est '\"'.

**Remarks**

Lors de la définition de cette propriété, [hasTextQualifier()](../../com.aspose.gridweb/gridtxtloadoptions\#hasTextQualifier--) deviendra true automatiquement.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | char |  |

### setTreatConsecutiveDelimitersAsOne(boolean value) {#setTreatConsecutiveDelimitersAsOne-boolean-}
```
public void setTreatConsecutiveDelimitersAsOne(boolean value)
```


Indique si les délimiteurs consécutifs doivent être traités comme un seul.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setTreatQuotePrefixAsValue(boolean value) {#setTreatQuotePrefixAsValue-boolean-}
```
public void setTreatQuotePrefixAsValue(boolean value)
```


Indique si le signe de guillemet simple initial doit être considéré comme faisant partie de la valeur d'une cellule. La valeur par défaut est true. Si elle est false, le guillemet simple initial sera supprimé de la valeur de la cellule correspondante et [GridTableItemStyle.getQuotePrefix()](../../com.aspose.gridweb/gridtableitemstyle\#getQuotePrefix--) sera défini sur true pour la cellule.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

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

