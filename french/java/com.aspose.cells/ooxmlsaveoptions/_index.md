---
title: "OoxmlSaveOptions"
second_title: "Référence API d'Aspose.Cells pour Java"
description: "Représente les options d'enregistrement du fichier Office Open XML."
type: docs
url: /fr/java/com.aspose.cells/ooxmlsaveoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.SaveOptions](../../com.aspose.cells/saveoptions)
```
public class OoxmlSaveOptions extends SaveOptions
```

Représente les options d'enregistrement du fichier Office Open XML.
## Constructeurs

| Constructeur | Description |
| --- | --- |
| [OoxmlSaveOptions()](#OoxmlSaveOptions--) | Crée les options pour enregistrer le fichier Office Open XML. |
| [OoxmlSaveOptions(int saveFormat)](#OoxmlSaveOptions-int-) | Crée les options pour enregistrer le fichier Office Open XML. |
## Méthodes

| Méthode | Description |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAsFlatOpc()](#getAsFlatOpc--) | Indique s'il faut enregistrer en tant que fichier OPC plat qui peut être généré par le SDK Open XML. |
| [getCachedFileFolder()](#getCachedFileFolder--) | Le dossier pour les fichiers temporaires pouvant être utilisés comme cache de données. |
| [getCheckExcelRestriction()](#getCheckExcelRestriction--) | Indique si la vérification des restrictions du fichier Excel est effectuée lorsque l'utilisateur modifie les objets liés aux cellules. |
| [getClass()](#getClass--) |  |
| [getClearData()](#getClearData--) | Rendre le classeur vide après l'enregistrement du fichier. |
| [getCompressionType()](#getCompressionType--) | Obtient le type de compression pour le fichier ooxml. |
| [getCreateDirectory()](#getCreateDirectory--) | Si vrai et que le répertoire n'existe pas, le répertoire sera créé automatiquement avant d'enregistrer le fichier. |
| [getEmbedOoxmlAsOleObject()](#getEmbedOoxmlAsOleObject--) | Indique s'il faut incorporer les fichiers Ooxml d'OleObject en tant qu'objet ole. |
| [getEnableZip64()](#getEnableZip64--) | Utilisez les extensions ZIP64 lors de l'écriture d'archives zip, si nécessaire. |
| [getEncryptDocumentProperties()](#getEncryptDocumentProperties--) | Indique s'il faut chiffrer les propriétés du document lors de l'enregistrement au format .xls. |
| [getExportCellName()](#getExportCellName--) | Indique si le nom de la cellule doit être exporté vers un fichier Excel2007 .xlsx (.xlsm, .xltx, .xltm). |
| [getLightCellsDataProvider()](#getLightCellsDataProvider--) | Le fournisseur de données pour enregistrer le classeur en mode léger. |
| [getMergeAreas()](#getMergeAreas--) | Indique s'il faut fusionner les zones de mise en forme conditionnelle et de validation avant d'enregistrer le fichier. |
| [getRefreshChartCache()](#getRefreshChartCache--) | Indique s'il faut mettre en cache les dernières données du graphique. |
| [getSaveFormat()](#getSaveFormat--) | Obtient le format de fichier d'enregistrement. |
| [getSortExternalNames()](#getSortExternalNames--) | Indique s'il faut trier les noms définis externes avant d'enregistrer le fichier. |
| [getSortNames()](#getSortNames--) | Indique s'il faut trier les noms définis avant d'enregistrer le fichier. |
| [getUpdateSmartArt()](#getUpdateSmartArt--) | Indique s'il faut mettre à jour le paramètre SmartArt. |
| [getUpdateZoom()](#getUpdateZoom--) | Indique s'il faut mettre à jour le facteur d'échelle avant d'enregistrer le fichier si les propriétés PageSetup.FitToPagesWide et PageSetup.FitToPagesTall contrôlent le redimensionnement de la feuille. |
| [getValidateMergedAreas()](#getValidateMergedAreas--) | Indique s'il faut valider les cellules fusionnées avant d'enregistrer le fichier. |
| [getWarningCallback()](#getWarningCallback--) | Obtient le rappel d'avertissement. |
| [getWpsCompatibility()](#getWpsCompatibility--) | Indique s’il faut rendre le xls plus compatible avec WPS. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAsFlatOpc(boolean value)](#setAsFlatOpc-boolean-) | Indique s'il faut enregistrer en tant que fichier OPC plat qui peut être généré par le SDK Open XML. |
| [setCachedFileFolder(String value)](#setCachedFileFolder-java.lang.String-) | Le dossier pour les fichiers temporaires pouvant être utilisés comme cache de données. |
| [setCheckExcelRestriction(boolean value)](#setCheckExcelRestriction-boolean-) | Indique si la vérification des restrictions du fichier Excel est effectuée lorsque l'utilisateur modifie les objets liés aux cellules. |
| [setClearData(boolean value)](#setClearData-boolean-) | Rendre le classeur vide après l'enregistrement du fichier. |
| [setCompressionType(int value)](#setCompressionType-int-) | Définit le type de compression pour le fichier ooxml. |
| [setCreateDirectory(boolean value)](#setCreateDirectory-boolean-) | Si vrai et que le répertoire n'existe pas, le répertoire sera créé automatiquement avant d'enregistrer le fichier. |
| [setEmbedOoxmlAsOleObject(boolean value)](#setEmbedOoxmlAsOleObject-boolean-) | Indique s'il faut incorporer les fichiers Ooxml d'OleObject en tant qu'objet ole. |
| [setEnableZip64(boolean value)](#setEnableZip64-boolean-) | Utilisez les extensions ZIP64 lors de l'écriture d'archives zip, si nécessaire. |
| [setEncryptDocumentProperties(boolean value)](#setEncryptDocumentProperties-boolean-) | Indique s'il faut chiffrer les propriétés du document lors de l'enregistrement au format .xls. |
| [setExportCellName(boolean value)](#setExportCellName-boolean-) | Indique si le nom de la cellule doit être exporté vers un fichier Excel2007 .xlsx (.xlsm, .xltx, .xltm). |
| [setLightCellsDataProvider(LightCellsDataProvider value)](#setLightCellsDataProvider-com.aspose.cells.LightCellsDataProvider-) | Le fournisseur de données pour enregistrer le classeur en mode léger. |
| [setMergeAreas(boolean value)](#setMergeAreas-boolean-) | Indique s'il faut fusionner les zones de mise en forme conditionnelle et de validation avant d'enregistrer le fichier. |
| [setRefreshChartCache(boolean value)](#setRefreshChartCache-boolean-) | Indique s'il faut mettre en cache les dernières données du graphique. |
| [setSortExternalNames(boolean value)](#setSortExternalNames-boolean-) | Indique s'il faut trier les noms définis externes avant d'enregistrer le fichier. |
| [setSortNames(boolean value)](#setSortNames-boolean-) | Indique s'il faut trier les noms définis avant d'enregistrer le fichier. |
| [setUpdateSmartArt(boolean value)](#setUpdateSmartArt-boolean-) | Indique s'il faut mettre à jour le paramètre SmartArt. |
| [setUpdateZoom(boolean value)](#setUpdateZoom-boolean-) | Indique s'il faut mettre à jour le facteur d'échelle avant d'enregistrer le fichier si les propriétés PageSetup.FitToPagesWide et PageSetup.FitToPagesTall contrôlent le redimensionnement de la feuille. |
| [setValidateMergedAreas(boolean value)](#setValidateMergedAreas-boolean-) | Indique s'il faut valider les cellules fusionnées avant d'enregistrer le fichier. |
| [setWarningCallback(IWarningCallback value)](#setWarningCallback-com.aspose.cells.IWarningCallback-) | Définit le rappel d’avertissement. |
| [setWpsCompatibility(boolean value)](#setWpsCompatibility-boolean-) | Indique s’il faut rendre le xls plus compatible avec WPS. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### OoxmlSaveOptions() {#OoxmlSaveOptions--}
```
public OoxmlSaveOptions()
```


Crée les options pour enregistrer le fichier Office Open XML.

### OoxmlSaveOptions(int saveFormat) {#OoxmlSaveOptions-int-}
```
public OoxmlSaveOptions(int saveFormat)
```


Crée les options pour enregistrer le fichier Office Open XML.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| saveFormat | int | [SaveFormat](../../com.aspose.cells/saveformat). Le format de fichier. Il doit être l'un des types suivants : [SaveFormat.XLSX](../../com.aspose.cells/saveformat\#XLSX), [SaveFormat.XLTX](../../com.aspose.cells/saveformat\#XLTX), [SaveFormat.XLAM](../../com.aspose.cells/saveformat\#XLAM), [SaveFormat.XLSM](../../com.aspose.cells/saveformat\#XLSM) ou [SaveFormat.XLTM](../../com.aspose.cells/saveformat\#XLTM), sinon le format enregistré sera automatiquement défini sur [SaveFormat.XLSX](../../com.aspose.cells/saveformat\#XLSX). |

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
### getAsFlatOpc() {#getAsFlatOpc--}
```
public boolean getAsFlatOpc()
```


Indique s'il faut enregistrer en tant que fichier OPC plat qui peut être généré par le SDK Open XML.

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
### getCompressionType() {#getCompressionType--}
```
public int getCompressionType()
```


Obtient le type de compression pour le fichier ooxml.

Voir [OoxmlCompressionType](../../com.aspose.cells/ooxmlcompressiontype).

**Remarks**

La valeur par défaut est OoxmlCompressionType.Level2.

**Returns:**
int
### getCreateDirectory() {#getCreateDirectory--}
```
public boolean getCreateDirectory()
```


Si vrai et que le répertoire n'existe pas, le répertoire sera créé automatiquement avant d'enregistrer le fichier.

**Remarks**

La valeur par défaut est false.

**Returns:**
boolean
### getEmbedOoxmlAsOleObject() {#getEmbedOoxmlAsOleObject--}
```
public boolean getEmbedOoxmlAsOleObject()
```


Indique s'il faut incorporer les fichiers Ooxml d'OleObject en tant qu'objet ole.

**Remarks**

Uniquement pour OleObject.

**Returns:**
boolean
### getEnableZip64() {#getEnableZip64--}
```
public boolean getEnableZip64()
```


Utilisez les extensions ZIP64 lors de l'écriture d'archives zip, si nécessaire.

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
### getExportCellName() {#getExportCellName--}
```
public boolean getExportCellName()
```


Indique si le nom de la cellule doit être exporté vers un fichier Excel2007 .xlsx (.xlsm, .xltx, .xltm). Si le fichier de sortie peut être accédé par SQL Server DTS, cette valeur doit être vraie. Mettre la valeur à false augmentera fortement les performances et réduira la taille du fichier lors de la création de gros fichiers. La valeur par défaut est true.

**Returns:**
boolean
### getLightCellsDataProvider() {#getLightCellsDataProvider--}
```
public LightCellsDataProvider getLightCellsDataProvider()
```


Le fournisseur de données pour enregistrer le classeur en mode léger.

**Returns:**
[LightCellsDataProvider](../../com.aspose.cells/lightcellsdataprovider)
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
### getUpdateZoom() {#getUpdateZoom--}
```
public boolean getUpdateZoom()
```


Indique s'il faut mettre à jour le facteur d'échelle avant d'enregistrer le fichier si les propriétés PageSetup.FitToPagesWide et PageSetup.FitToPagesTall contrôlent le redimensionnement de la feuille.

**Remarks**

La valeur par défaut est false pour les performances.

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
### getWpsCompatibility() {#getWpsCompatibility--}
```
public boolean getWpsCompatibility()
```


Indique s’il faut rendre le xls plus compatible avec WPS.

**Remarks**

NOTE : Ce membre est maintenant obsolète. À la place, veuillez utiliser la propriété WorkbookSetting.WpsCompatibility. Cette méthode sera supprimée 12 mois plus tard à compter de décembre 2025. Aspose s’excuse pour tout désagrément que vous auriez pu rencontrer.

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




### setAsFlatOpc(boolean value) {#setAsFlatOpc-boolean-}
```
public void setAsFlatOpc(boolean value)
```


Indique s'il faut enregistrer en tant que fichier OPC plat qui peut être généré par le SDK Open XML.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

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

### setCompressionType(int value) {#setCompressionType-int-}
```
public void setCompressionType(int value)
```


Définit le type de compression pour le fichier ooxml.

Voir [OoxmlCompressionType](../../com.aspose.cells/ooxmlcompressiontype).

**Remarks**

La valeur par défaut est OoxmlCompressionType.Level2.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

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

### setEmbedOoxmlAsOleObject(boolean value) {#setEmbedOoxmlAsOleObject-boolean-}
```
public void setEmbedOoxmlAsOleObject(boolean value)
```


Indique s'il faut incorporer les fichiers Ooxml d'OleObject en tant qu'objet ole.

**Remarks**

Uniquement pour OleObject.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setEnableZip64(boolean value) {#setEnableZip64-boolean-}
```
public void setEnableZip64(boolean value)
```


Utilisez les extensions ZIP64 lors de l'écriture d'archives zip, si nécessaire.

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

### setExportCellName(boolean value) {#setExportCellName-boolean-}
```
public void setExportCellName(boolean value)
```


Indique si le nom de la cellule doit être exporté vers un fichier Excel2007 .xlsx (.xlsm, .xltx, .xltm). Si le fichier de sortie peut être accédé par SQL Server DTS, cette valeur doit être vraie. Mettre la valeur à false augmentera fortement les performances et réduira la taille du fichier lors de la création de gros fichiers. La valeur par défaut est true.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setLightCellsDataProvider(LightCellsDataProvider value) {#setLightCellsDataProvider-com.aspose.cells.LightCellsDataProvider-}
```
public void setLightCellsDataProvider(LightCellsDataProvider value)
```


Le fournisseur de données pour enregistrer le classeur en mode léger.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | [LightCellsDataProvider](../../com.aspose.cells/lightcellsdataprovider) |  |

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

### setUpdateZoom(boolean value) {#setUpdateZoom-boolean-}
```
public void setUpdateZoom(boolean value)
```


Indique s'il faut mettre à jour le facteur d'échelle avant d'enregistrer le fichier si les propriétés PageSetup.FitToPagesWide et PageSetup.FitToPagesTall contrôlent le redimensionnement de la feuille.

**Remarks**

La valeur par défaut est false pour les performances.

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

### setWpsCompatibility(boolean value) {#setWpsCompatibility-boolean-}
```
public void setWpsCompatibility(boolean value)
```


Indique s’il faut rendre le xls plus compatible avec WPS.

**Remarks**

NOTE : Ce membre est maintenant obsolète. À la place, veuillez utiliser la propriété WorkbookSetting.WpsCompatibility. Cette méthode sera supprimée 12 mois plus tard à compter de décembre 2025. Aspose s’excuse pour tout désagrément que vous auriez pu rencontrer.

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

