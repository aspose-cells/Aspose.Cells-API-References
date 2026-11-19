---
title: "OdsSaveOptions"
second_title: "Référence API d'Aspose.Cells pour Java"
description: "Représente les options d'enregistrement du fichier ods."
type: docs
url: /fr/java/com.aspose.cells/odssaveoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.SaveOptions](../../com.aspose.cells/saveoptions)
```
public class OdsSaveOptions extends SaveOptions
```

Représente les options d'enregistrement du fichier ods.
## Constructeurs

| Constructeur | Description |
| --- | --- |
| [OdsSaveOptions()](#OdsSaveOptions--) | Crée les options d'enregistrement du fichier ods. |
| [OdsSaveOptions(int saveFormat)](#OdsSaveOptions-int-) | Crée les options d'enregistrement du fichier ods. |
## Méthodes

| Méthode | Description |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getCachedFileFolder()](#getCachedFileFolder--) | Le dossier pour les fichiers temporaires pouvant être utilisés comme cache de données. |
| [getCheckExcelRestriction()](#getCheckExcelRestriction--) | Indique si la vérification des restrictions du fichier Excel est effectuée lorsque l'utilisateur modifie les objets liés aux cellules. |
| [getClass()](#getClass--) |  |
| [getClearData()](#getClearData--) | Rendre le classeur vide après l'enregistrement du fichier. |
| [getCreateDirectory()](#getCreateDirectory--) | Si vrai et que le répertoire n'existe pas, le répertoire sera créé automatiquement avant d'enregistrer le fichier. |
| [getEncryptDocumentProperties()](#getEncryptDocumentProperties--) | Indique s'il faut chiffrer les propriétés du document lors de l'enregistrement au format .xls. |
| [getGeneratorType()](#getGeneratorType--) | Obtient le générateur du fichier ods. |
| [getIgnorePivotTables()](#getIgnorePivotTables--) | Indique s'il faut enregistrer les tableaux croisés dynamiques. |
| [getMergeAreas()](#getMergeAreas--) | Indique s'il faut fusionner les zones de mise en forme conditionnelle et de validation avant d'enregistrer le fichier. |
| [getOdfStrictVersion()](#getOdfStrictVersion--) | Obtient la version ODF. |
| [getRefreshChartCache()](#getRefreshChartCache--) | Indique s'il faut mettre en cache les dernières données du graphique. |
| [getSaveFormat()](#getSaveFormat--) | Obtient le format de fichier d'enregistrement. |
| [getSortExternalNames()](#getSortExternalNames--) | Indique s'il faut trier les noms définis externes avant d'enregistrer le fichier. |
| [getSortNames()](#getSortNames--) | Indique s'il faut trier les noms définis avant d'enregistrer le fichier. |
| [getUpdateSmartArt()](#getUpdateSmartArt--) | Indique s'il faut mettre à jour le paramètre SmartArt. |
| [getValidateMergedAreas()](#getValidateMergedAreas--) | Indique s'il faut valider les cellules fusionnées avant d'enregistrer le fichier. |
| [getWarningCallback()](#getWarningCallback--) | Obtient le rappel d'avertissement. |
| [hashCode()](#hashCode--) |  |
| [isStrictSchema11()](#isStrictSchema11--) | Indique si le fichier ods doit être enregistré au format ODF version 1.1. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setCachedFileFolder(String value)](#setCachedFileFolder-java.lang.String-) | Le dossier pour les fichiers temporaires pouvant être utilisés comme cache de données. |
| [setCheckExcelRestriction(boolean value)](#setCheckExcelRestriction-boolean-) | Indique si la vérification des restrictions du fichier Excel est effectuée lorsque l'utilisateur modifie les objets liés aux cellules. |
| [setClearData(boolean value)](#setClearData-boolean-) | Rendre le classeur vide après l'enregistrement du fichier. |
| [setCreateDirectory(boolean value)](#setCreateDirectory-boolean-) | Si vrai et que le répertoire n'existe pas, le répertoire sera créé automatiquement avant d'enregistrer le fichier. |
| [setEncryptDocumentProperties(boolean value)](#setEncryptDocumentProperties-boolean-) | Indique s'il faut chiffrer les propriétés du document lors de l'enregistrement au format .xls. |
| [setGeneratorType(int value)](#setGeneratorType-int-) | Définit le générateur du fichier ods. |
| [setIgnorePivotTables(boolean value)](#setIgnorePivotTables-boolean-) | Indique s'il faut enregistrer les tableaux croisés dynamiques. |
| [setMergeAreas(boolean value)](#setMergeAreas-boolean-) | Indique s'il faut fusionner les zones de mise en forme conditionnelle et de validation avant d'enregistrer le fichier. |
| [setOdfStrictVersion(int value)](#setOdfStrictVersion-int-) | Définit la version ODF. |
| [setRefreshChartCache(boolean value)](#setRefreshChartCache-boolean-) | Indique s'il faut mettre en cache les dernières données du graphique. |
| [setSortExternalNames(boolean value)](#setSortExternalNames-boolean-) | Indique s'il faut trier les noms définis externes avant d'enregistrer le fichier. |
| [setSortNames(boolean value)](#setSortNames-boolean-) | Indique s'il faut trier les noms définis avant d'enregistrer le fichier. |
| [setStrictSchema11(boolean value)](#setStrictSchema11-boolean-) | Indique si le fichier ods doit être enregistré au format ODF version 1.1. |
| [setUpdateSmartArt(boolean value)](#setUpdateSmartArt-boolean-) | Indique s'il faut mettre à jour le paramètre SmartArt. |
| [setValidateMergedAreas(boolean value)](#setValidateMergedAreas-boolean-) | Indique s'il faut valider les cellules fusionnées avant d'enregistrer le fichier. |
| [setWarningCallback(IWarningCallback value)](#setWarningCallback-com.aspose.cells.IWarningCallback-) | Définit le rappel d’avertissement. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### OdsSaveOptions() {#OdsSaveOptions--}
```
public OdsSaveOptions()
```


Crée les options d'enregistrement du fichier ods.

### OdsSaveOptions(int saveFormat) {#OdsSaveOptions-int-}
```
public OdsSaveOptions(int saveFormat)
```


Crée les options d'enregistrement du fichier ods.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| saveFormat | int | [SaveFormat](../../com.aspose.cells/saveformat). Le format de fichier. Il doit être [SaveFormat.ODS](../../com.aspose.cells/saveformat\#ODS), [SaveFormat.OTS](../../com.aspose.cells/saveformat\#OTS), [SaveFormat.FODS](../../com.aspose.cells/saveformat\#FODS) ou [SaveFormat.SXC](../../com.aspose.cells/saveformat\#SXC), sinon le format enregistré sera automatiquement défini sur [SaveFormat.ODS](../../com.aspose.cells/saveformat\#ODS). |

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
### getCachedFileFolder() {#getCachedFileFolder--}
```
public String getCachedFileFolder()
```


Le dossier pour les fichiers temporaires pouvant être utilisés comme cache de données.

**Remarks**

Si le dossier n'a pas été spécifié, la valeur par défaut est [CellsHelper.getCacheFolder()](../../com.aspose.cells/cellshelper\#getCacheFolder--). Si sa valeur par défaut est nulle ou vide, ou a été spécifiée comme nulle ou vide, aucun fichier de cache ne sera utilisé lors de l'enregistrement du classeur.

**Returns:**
java.lang.String
### getCheckExcelRestriction() {#getCheckExcelRestriction--}
```
public boolean getCheckExcelRestriction()
```


Vérifie la restriction du fichier Excel lorsque l'utilisateur modifie des objets liés aux cellules. Par exemple, Excel n'autorise pas la saisie d'une chaîne de caractères supérieure à 32 K. Lorsque vous saisissez une valeur supérieure à 32 K, elle sera tronquée.

**Returns:**
boolean
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getClearData() {#getClearData--}
```
public boolean getClearData()
```


Rendre le classeur vide après l'enregistrement du fichier.

**Returns:**
boolean
### getCreateDirectory() {#getCreateDirectory--}
```
public boolean getCreateDirectory()
```


Si vrai et que le répertoire n'existe pas, le répertoire sera créé automatiquement avant d'enregistrer le fichier.

**Remarks**

La valeur par défaut est false.

**Returns:**
boolean
### getEncryptDocumentProperties() {#getEncryptDocumentProperties--}
```
public boolean getEncryptDocumentProperties()
```


Indique si les propriétés du document sont chiffrées lors de l'enregistrement au format .xls. La valeur par défaut est true.

**Remarks**

Uniquement pour les fichiers .xls, .xlsx, .xlsb et .xlsm.

**Returns:**
boolean
### getGeneratorType() {#getGeneratorType--}
```
public int getGeneratorType()
```


Obtient le générateur du fichier ods.

Voir [OdsGeneratorType](../../com.aspose.cells/odsgeneratortype).

**Returns:**
int
### getIgnorePivotTables() {#getIgnorePivotTables--}
```
public boolean getIgnorePivotTables()
```


Indique s'il faut enregistrer les tableaux croisés dynamiques.

**Remarks**

La fonctionnalité de tableau croisé dynamique d'OpenOffice possède moins de paramètres comparée à Excel, ce qui entraîne de nombreuses différences dans les résultats des tableaux croisés dynamiques. Parfois, il est préférable d'ignorer ces tableaux croisés dynamiques lors de l'enregistrement du fichier .ods.

**Returns:**
boolean
### getMergeAreas() {#getMergeAreas--}
```
public boolean getMergeAreas()
```


Indique s'il faut fusionner les zones de mise en forme conditionnelle et de validation avant d'enregistrer le fichier.

**Remarks**

La valeur par défaut est false.

**Returns:**
boolean
### getOdfStrictVersion() {#getOdfStrictVersion--}
```
public int getOdfStrictVersion()
```


Obtient la version ODF.

Voir [OpenDocumentFormatVersionType](../../com.aspose.cells/opendocumentformatversiontype).

**Returns:**
int
### getRefreshChartCache() {#getRefreshChartCache--}
```
public boolean getRefreshChartCache()
```


Indique s'il faut mettre en cache les dernières données du graphique.

**Returns:**
boolean
### getSaveFormat() {#getSaveFormat--}
```
public int getSaveFormat()
```


Obtient le format de fichier d'enregistrement.

Voir [SaveFormat](../../com.aspose.cells/saveformat).

**Returns:**
int
### getSortExternalNames() {#getSortExternalNames--}
```
public boolean getSortExternalNames()
```


Indique s'il faut trier les noms définis externes avant d'enregistrer le fichier.

**Returns:**
boolean
### getSortNames() {#getSortNames--}
```
public boolean getSortNames()
```


Indique s'il faut trier les noms définis avant d'enregistrer le fichier.

**Returns:**
boolean
### getUpdateSmartArt() {#getUpdateSmartArt--}
```
public boolean getUpdateSmartArt()
```


Indique si la mise à jour du paramètre smart art est activée. La valeur par défaut est false.

**Remarks**

N'affecte que après l'appel de la méthode Shape.GetResultOfSmartArt() et lorsque les formes mises en cache existent dans le fichier modèle.

**Returns:**
boolean
### getValidateMergedAreas() {#getValidateMergedAreas--}
```
public boolean getValidateMergedAreas()
```


Indique s'il faut valider les cellules fusionnées avant d'enregistrer le fichier.

**Remarks**

La valeur par défaut est false.

**Returns:**
boolean
### getWarningCallback() {#getWarningCallback--}
```
public IWarningCallback getWarningCallback()
```


Obtient le rappel d'avertissement.

**Returns:**
[IWarningCallback](../../com.aspose.cells/iwarningcallback)
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isStrictSchema11() {#isStrictSchema11--}
```
public boolean isStrictSchema11()
```


Indique si le fichier ods doit être enregistré au format ODF version 1.1. La valeur par défaut est false.

**Remarks**

NOTE : Ce membre est désormais obsolète. Veuillez plutôt utiliser la propriété OdsSaveOptions.OdfStrictVersion. Cette méthode sera supprimée 12 mois après février 2024. Aspose s'excuse pour tout désagrément que vous auriez pu rencontrer.

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




### setCachedFileFolder(String value) {#setCachedFileFolder-java.lang.String-}
```
public void setCachedFileFolder(String value)
```


Le dossier pour les fichiers temporaires pouvant être utilisés comme cache de données.

**Remarks**

Si le dossier n'a pas été spécifié, la valeur par défaut est [CellsHelper.getCacheFolder()](../../com.aspose.cells/cellshelper\#getCacheFolder--). Si sa valeur par défaut est nulle ou vide, ou a été spécifiée comme nulle ou vide, aucun fichier de cache ne sera utilisé lors de l'enregistrement du classeur.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

### setCheckExcelRestriction(boolean value) {#setCheckExcelRestriction-boolean-}
```
public void setCheckExcelRestriction(boolean value)
```


Vérifie la restriction du fichier Excel lorsque l'utilisateur modifie des objets liés aux cellules. Par exemple, Excel n'autorise pas la saisie d'une chaîne de caractères supérieure à 32 K. Lorsque vous saisissez une valeur supérieure à 32 K, elle sera tronquée.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setClearData(boolean value) {#setClearData-boolean-}
```
public void setClearData(boolean value)
```


Rendre le classeur vide après l'enregistrement du fichier.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setCreateDirectory(boolean value) {#setCreateDirectory-boolean-}
```
public void setCreateDirectory(boolean value)
```


Si vrai et que le répertoire n'existe pas, le répertoire sera créé automatiquement avant d'enregistrer le fichier.

**Remarks**

La valeur par défaut est false.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setEncryptDocumentProperties(boolean value) {#setEncryptDocumentProperties-boolean-}
```
public void setEncryptDocumentProperties(boolean value)
```


Indique si les propriétés du document sont chiffrées lors de l'enregistrement au format .xls. La valeur par défaut est true.

**Remarks**

Uniquement pour les fichiers .xls, .xlsx, .xlsb et .xlsm.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setGeneratorType(int value) {#setGeneratorType-int-}
```
public void setGeneratorType(int value)
```


Définit le générateur du fichier ods.

Voir [OdsGeneratorType](../../com.aspose.cells/odsgeneratortype).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setIgnorePivotTables(boolean value) {#setIgnorePivotTables-boolean-}
```
public void setIgnorePivotTables(boolean value)
```


Indique s'il faut enregistrer les tableaux croisés dynamiques.

**Remarks**

La fonctionnalité de tableau croisé dynamique d'OpenOffice possède moins de paramètres comparée à Excel, ce qui entraîne de nombreuses différences dans les résultats des tableaux croisés dynamiques. Parfois, il est préférable d'ignorer ces tableaux croisés dynamiques lors de l'enregistrement du fichier .ods.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setMergeAreas(boolean value) {#setMergeAreas-boolean-}
```
public void setMergeAreas(boolean value)
```


Indique s'il faut fusionner les zones de mise en forme conditionnelle et de validation avant d'enregistrer le fichier.

**Remarks**

La valeur par défaut est false.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setOdfStrictVersion(int value) {#setOdfStrictVersion-int-}
```
public void setOdfStrictVersion(int value)
```


Définit la version ODF.

Voir [OpenDocumentFormatVersionType](../../com.aspose.cells/opendocumentformatversiontype).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setRefreshChartCache(boolean value) {#setRefreshChartCache-boolean-}
```
public void setRefreshChartCache(boolean value)
```


Indique s'il faut mettre en cache les dernières données du graphique.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setSortExternalNames(boolean value) {#setSortExternalNames-boolean-}
```
public void setSortExternalNames(boolean value)
```


Indique s'il faut trier les noms définis externes avant d'enregistrer le fichier.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setSortNames(boolean value) {#setSortNames-boolean-}
```
public void setSortNames(boolean value)
```


Indique s'il faut trier les noms définis avant d'enregistrer le fichier.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setStrictSchema11(boolean value) {#setStrictSchema11-boolean-}
```
public void setStrictSchema11(boolean value)
```


Indique si le fichier ods doit être enregistré au format ODF version 1.1. La valeur par défaut est false.

**Remarks**

NOTE : Ce membre est désormais obsolète. Veuillez plutôt utiliser la propriété OdsSaveOptions.OdfStrictVersion. Cette méthode sera supprimée 12 mois après février 2024. Aspose s'excuse pour tout désagrément que vous auriez pu rencontrer.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setUpdateSmartArt(boolean value) {#setUpdateSmartArt-boolean-}
```
public void setUpdateSmartArt(boolean value)
```


Indique si la mise à jour du paramètre smart art est activée. La valeur par défaut est false.

**Remarks**

N'affecte que après l'appel de la méthode Shape.GetResultOfSmartArt() et lorsque les formes mises en cache existent dans le fichier modèle.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setValidateMergedAreas(boolean value) {#setValidateMergedAreas-boolean-}
```
public void setValidateMergedAreas(boolean value)
```


Indique s'il faut valider les cellules fusionnées avant d'enregistrer le fichier.

**Remarks**

La valeur par défaut est false.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setWarningCallback(IWarningCallback value) {#setWarningCallback-com.aspose.cells.IWarningCallback-}
```
public void setWarningCallback(IWarningCallback value)
```


Définit le rappel d’avertissement.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | [IWarningCallback](../../com.aspose.cells/iwarningcallback) |  |

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

