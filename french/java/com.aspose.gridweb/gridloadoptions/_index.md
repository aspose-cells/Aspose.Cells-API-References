---
title: "GridLoadOptions"
second_title: "Référence API d'Aspose.Cells pour Java"
description: "Représente les options de chargement du fichier."
type: docs
url: /fr/java/com.aspose.gridweb/gridloadoptions/
---

**Inheritance:**
java.lang.Object
```
public class GridLoadOptions
```

Représente les options de chargement du fichier. [Obsolete(\"This class will be obsoleted after stand alone dll usage of cells public api,instead you can use Aspose.Cells.LodOptions \")]
## Constructeurs

| Constructeur | Description |
| --- | --- |
| [GridLoadOptions()](#GridLoadOptions--) | Crée une option de chargement du fichier. |
## Méthodes

| Méthode | Description |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAutoFilter()](#getAutoFilter--) | Indique si le filtrage automatique des données est effectué lors du chargement des fichiers. |
| [getCheckDataValid()](#getCheckDataValid--) | Vérifie si les données sont valides dans le fichier modèle. |
| [getCheckExcelRestriction()](#getCheckExcelRestriction--) | Indique si la vérification des restrictions du fichier Excel est effectuée lorsque l'utilisateur modifie les objets liés aux cellules. |
| [getClass()](#getClass--) |  |
| [getIgnoreNotPrinted()](#getIgnoreNotPrinted--) | Ignore les données qui ne sont pas imprimées lors de l'impression directe du fichier |
| [getKeepUnparsedData()](#getKeepUnparsedData--) | Indique si les données non analysées sont conservées en mémoire pour le classeur lorsqu'il est chargé à partir du fichier modèle. |
| [getOnlyAuto()](#getOnlyAuto--) | Indique si seules les lignes dont la hauteur n'est pas personnalisée sont ajustées. |
| [getParsingFormulaOnOpen()](#getParsingFormulaOnOpen--) | Indique si la formule est analysée lors de la lecture du fichier. |
| [getParsingPivotCachedRecords()](#getParsingPivotCachedRecords--) | Indique si les enregistrements mis en cache du tableau croisé dynamique sont analysés lors du chargement du fichier. |
| [getPassword()](#getPassword--) | Obtient le mot de passe du classeur. |
| [getPreservePaddingSpacesInFormula()](#getPreservePaddingSpacesInFormula--) | Indique s'il faut préserver les espaces et les sauts de ligne insérés entre les jetons de formule lors de l'obtention et de la définition des formules. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAutoFilter(boolean value)](#setAutoFilter-boolean-) | Indique si le filtrage automatique des données est effectué lors du chargement des fichiers. |
| [setCheckDataValid(boolean value)](#setCheckDataValid-boolean-) | Vérifie si les données sont valides dans le fichier modèle. |
| [setCheckExcelRestriction(boolean value)](#setCheckExcelRestriction-boolean-) | Indique si la vérification des restrictions du fichier Excel est effectuée lorsque l'utilisateur modifie les objets liés aux cellules. |
| [setIgnoreNotPrinted(boolean value)](#setIgnoreNotPrinted-boolean-) | Ignore les données qui ne sont pas imprimées lors de l'impression directe du fichier |
| [setKeepUnparsedData(boolean value)](#setKeepUnparsedData-boolean-) | Indique si les données non analysées sont conservées en mémoire pour le classeur lorsqu'il est chargé à partir du fichier modèle. |
| [setOnlyAuto(boolean value)](#setOnlyAuto-boolean-) | Indique si seules les lignes dont la hauteur n'est pas personnalisée sont ajustées. |
| [setParsingFormulaOnOpen(boolean value)](#setParsingFormulaOnOpen-boolean-) | Indique si la formule est analysée lors de la lecture du fichier. |
| [setParsingPivotCachedRecords(boolean value)](#setParsingPivotCachedRecords-boolean-) | Indique si les enregistrements mis en cache du tableau croisé dynamique sont analysés lors du chargement du fichier. |
| [setPassword(String value)](#setPassword-java.lang.String-) | Définit le mot de passe du classeur. |
| [setPreservePaddingSpacesInFormula(boolean value)](#setPreservePaddingSpacesInFormula-boolean-) | Indique s'il faut préserver les espaces et les sauts de ligne insérés entre les jetons de formule lors de l'obtention et de la définition des formules. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### GridLoadOptions() {#GridLoadOptions--}
```
public GridLoadOptions()
```


Crée une option de chargement du fichier.

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
### getIgnoreNotPrinted() {#getIgnoreNotPrinted--}
```
public boolean getIgnoreNotPrinted()
```


Ignore les données qui ne sont pas imprimées lors de l'impression directe du fichier

**Remarks**

Uniquement pour le fichier xlsx.

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

