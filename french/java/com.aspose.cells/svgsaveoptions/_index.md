---
title: "SvgSaveOptions"
second_title: "Référence API d'Aspose.Cells pour Java"
description: "Représente les options d'enregistrement Svg."
type: docs
url: /fr/java/com.aspose.cells/svgsaveoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.SaveOptions](../../com.aspose.cells/saveoptions), [com.aspose.cells.ImageSaveOptions](../../com.aspose.cells/imagesaveoptions)
```
public class SvgSaveOptions extends ImageSaveOptions
```

Représente les options d'enregistrement Svg. Pour une utilisation avancée, veuillez utiliser [WorkbookRender](../../com.aspose.cells/workbookrender) ou [SheetRender](../../com.aspose.cells/sheetrender).

**Remarks**

NOTE: Cette classe est maintenant obsolète. À la place, veuillez utiliser la classe ImageSaveOptions. Cette propriété sera supprimée 12 mois plus tard, depuis mars 2023. Aspose s'excuse pour tout désagrément que vous auriez pu rencontrer.
## Constructeurs

| Constructeur | Description |
| --- | --- |
| [SvgSaveOptions()](#SvgSaveOptions--) | Crée les options pour enregistrer un fichier svg. |
| [SvgSaveOptions(int saveFormat)](#SvgSaveOptions-int-) | Crée les options pour enregistrer un fichier svg. |
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
| [getImageOrPrintOptions()](#getImageOrPrintOptions--) | Options supplémentaires de création d'image. |
| [getMergeAreas()](#getMergeAreas--) | Indique s'il faut fusionner les zones de mise en forme conditionnelle et de validation avant d'enregistrer le fichier. |
| [getRefreshChartCache()](#getRefreshChartCache--) | Indique s'il faut mettre en cache les dernières données du graphique. |
| [getSaveFormat()](#getSaveFormat--) | Obtient le format de fichier d'enregistrement. |
| [getSheetIndex()](#getSheetIndex--) | Obtient quelle feuille de calcul doit être exportée. |
| [getSortExternalNames()](#getSortExternalNames--) | Indique s'il faut trier les noms définis externes avant d'enregistrer le fichier. |
| [getSortNames()](#getSortNames--) | Indique s'il faut trier les noms définis avant d'enregistrer le fichier. |
| [getStreamProvider()](#getStreamProvider--) | Obtient le IStreamProvider pour l'exportation des objets. |
| [getUpdateSmartArt()](#getUpdateSmartArt--) | Indique s'il faut mettre à jour le paramètre SmartArt. |
| [getValidateMergedAreas()](#getValidateMergedAreas--) | Indique s'il faut valider les cellules fusionnées avant d'enregistrer le fichier. |
| [getWarningCallback()](#getWarningCallback--) | Obtient le rappel d'avertissement. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setCachedFileFolder(String value)](#setCachedFileFolder-java.lang.String-) | Le dossier pour les fichiers temporaires pouvant être utilisés comme cache de données. |
| [setCheckExcelRestriction(boolean value)](#setCheckExcelRestriction-boolean-) | Indique si la vérification des restrictions du fichier Excel est effectuée lorsque l'utilisateur modifie les objets liés aux cellules. |
| [setClearData(boolean value)](#setClearData-boolean-) | Rendre le classeur vide après l'enregistrement du fichier. |
| [setCreateDirectory(boolean value)](#setCreateDirectory-boolean-) | Si vrai et que le répertoire n'existe pas, le répertoire sera créé automatiquement avant d'enregistrer le fichier. |
| [setEncryptDocumentProperties(boolean value)](#setEncryptDocumentProperties-boolean-) | Indique s'il faut chiffrer les propriétés du document lors de l'enregistrement au format .xls. |
| [setMergeAreas(boolean value)](#setMergeAreas-boolean-) | Indique s'il faut fusionner les zones de mise en forme conditionnelle et de validation avant d'enregistrer le fichier. |
| [setRefreshChartCache(boolean value)](#setRefreshChartCache-boolean-) | Indique s'il faut mettre en cache les dernières données du graphique. |
| [setSheetIndex(int value)](#setSheetIndex-int-) | Définit quelle feuille de calcul doit être exportée. |
| [setSortExternalNames(boolean value)](#setSortExternalNames-boolean-) | Indique s'il faut trier les noms définis externes avant d'enregistrer le fichier. |
| [setSortNames(boolean value)](#setSortNames-boolean-) | Indique s'il faut trier les noms définis avant d'enregistrer le fichier. |
| [setStreamProvider(IStreamProvider value)](#setStreamProvider-com.aspose.cells.IStreamProvider-) | Définit le IStreamProvider pour l'exportation des objets. |
| [setUpdateSmartArt(boolean value)](#setUpdateSmartArt-boolean-) | Indique s'il faut mettre à jour le paramètre SmartArt. |
| [setValidateMergedAreas(boolean value)](#setValidateMergedAreas-boolean-) | Indique s'il faut valider les cellules fusionnées avant d'enregistrer le fichier. |
| [setWarningCallback(IWarningCallback value)](#setWarningCallback-com.aspose.cells.IWarningCallback-) | Définit le rappel d’avertissement. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### SvgSaveOptions() {#SvgSaveOptions--}
```
public SvgSaveOptions()
```


Crée les options pour enregistrer un fichier svg.

**Remarks**

NOTE: Cette classe est maintenant obsolète. À la place, veuillez utiliser la classe ImageSaveOptions. Cette propriété sera supprimée 12 mois plus tard, depuis mars 2023. Aspose s'excuse pour tout désagrément que vous auriez pu rencontrer.

### SvgSaveOptions(int saveFormat) {#SvgSaveOptions-int-}
```
public SvgSaveOptions(int saveFormat)
```


Crée les options pour enregistrer un fichier svg.

**Remarks**

NOTE: Ce constructeur est maintenant obsolète. À la place, veuillez utiliser le constructeur SvgSaveOptions(). Cette propriété sera supprimée 12 mois plus tard, depuis août 2022. Aspose s'excuse pour tout désagrément que vous auriez pu rencontrer.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| saveFormat | int | [SaveFormat](../../com.aspose.cells/saveformat). Le format de fichier. Il doit être svg. |

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
### getImageOrPrintOptions() {#getImageOrPrintOptions--}
```
public ImageOrPrintOptions getImageOrPrintOptions()
```


Options supplémentaires de création d'image.

**Remarks**

Pour une utilisation avancée, veuillez utiliser [WorkbookRender](../../com.aspose.cells/workbookrender) ou [SheetRender](../../com.aspose.cells/sheetrender).

**Returns:**
[ImageOrPrintOptions](../../com.aspose.cells/imageorprintoptions)
### getMergeAreas() {#getMergeAreas--}
```
public boolean getMergeAreas()
```


Indique s'il faut fusionner les zones de mise en forme conditionnelle et de validation avant d'enregistrer le fichier.

**Remarks**

La valeur par défaut est false.

**Returns:**
boolean
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
### getSheetIndex() {#getSheetIndex--}
```
public int getSheetIndex()
```


Obtient quelle feuille de calcul doit être exportée. Si la valeur est -1, la feuille de calcul active sera exportée.

**Remarks**

NOTE: Cette classe est maintenant obsolète. À la place, veuillez utiliser la classe ImageSaveOptions. Cette propriété sera supprimée 12 mois plus tard, depuis mars 2023. Aspose s'excuse pour tout désagrément que vous auriez pu rencontrer.

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
### getStreamProvider() {#getStreamProvider--}
```
public IStreamProvider getStreamProvider()
```


Obtient le IStreamProvider pour l'exportation des objets.

**Remarks**

Si l'enregistrement se fait au format Tiff, cette propriété est ignorée. Sinon, si plusieurs images doivent être enregistrées, nous écrirons les autres images avec celle-ci. Pour une utilisation avancée, veuillez utiliser [WorkbookRender](../../com.aspose.cells/workbookrender) ou [SheetRender](../../com.aspose.cells/sheetrender).

**Returns:**
[IStreamProvider](../../com.aspose.cells/istreamprovider)
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

### setRefreshChartCache(boolean value) {#setRefreshChartCache-boolean-}
```
public void setRefreshChartCache(boolean value)
```


Indique s'il faut mettre en cache les dernières données du graphique.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setSheetIndex(int value) {#setSheetIndex-int-}
```
public void setSheetIndex(int value)
```


Définit quelle feuille de calcul doit être exportée. Si la valeur est -1, la feuille de calcul active sera exportée.

**Remarks**

NOTE: Cette classe est maintenant obsolète. À la place, veuillez utiliser la classe ImageSaveOptions. Cette propriété sera supprimée 12 mois plus tard, depuis mars 2023. Aspose s'excuse pour tout désagrément que vous auriez pu rencontrer.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

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

### setStreamProvider(IStreamProvider value) {#setStreamProvider-com.aspose.cells.IStreamProvider-}
```
public void setStreamProvider(IStreamProvider value)
```


Définit le IStreamProvider pour l'exportation des objets.

**Remarks**

Si l'enregistrement se fait au format Tiff, cette propriété est ignorée. Sinon, si plusieurs images doivent être enregistrées, nous écrirons les autres images avec celle-ci. Pour une utilisation avancée, veuillez utiliser [WorkbookRender](../../com.aspose.cells/workbookrender) ou [SheetRender](../../com.aspose.cells/sheetrender).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | [IStreamProvider](../../com.aspose.cells/istreamprovider) |  |

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

