---
title: "TxtSaveOptions"
second_title: "Référence API d'Aspose.Cells pour Java"
description: "Représente les options d'enregistrement pour le format csv/à tabulation/d'autres formats texte."
type: docs
url: /fr/java/com.aspose.cells/txtsaveoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.SaveOptions](../../com.aspose.cells/saveoptions)
```
public class TxtSaveOptions extends SaveOptions
```

Représente les options d'enregistrement pour le format csv/à tabulation/d'autres formats texte.
## Constructeurs

| Constructeur | Description |
| --- | --- |
| [TxtSaveOptions()](#TxtSaveOptions--) | Crée des options d'enregistrement de fichier texte. |
| [TxtSaveOptions(int saveFormat)](#TxtSaveOptions-int-) | Crée des options d'enregistrement de fichier texte. |
## Méthodes

| Méthode | Description |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAlwaysQuoted()](#getAlwaysQuoted--) | Indique si l'ajout du caractère '\\"' est toujours effectué pour chaque champ. |
| [getCachedFileFolder()](#getCachedFileFolder--) | Le dossier pour les fichiers temporaires pouvant être utilisés comme cache de données. |
| [getCheckExcelRestriction()](#getCheckExcelRestriction--) | Indique si la vérification des restrictions du fichier Excel est effectuée lorsque l'utilisateur modifie les objets liés aux cellules. |
| [getClass()](#getClass--) |  |
| [getClearData()](#getClearData--) | Rendre le classeur vide après l'enregistrement du fichier. |
| [getCreateDirectory()](#getCreateDirectory--) | Si vrai et que le répertoire n'existe pas, le répertoire sera créé automatiquement avant d'enregistrer le fichier. |
| [getEncoding()](#getEncoding--) | Obtient le codage par défaut. |
| [getEncryptDocumentProperties()](#getEncryptDocumentProperties--) | Indique s'il faut chiffrer les propriétés du document lors de l'enregistrement au format .xls. |
| [getExportAllSheets()](#getExportAllSheets--) | Indique si toutes les feuilles sont exportées vers le fichier texte. |
| [getExportArea()](#getExportArea--) | La plage de cellules à exporter. |
| [getExportQuotePrefix()](#getExportQuotePrefix--) | Indique si le signe d'apostrophe simple doit être exporté comme faisant partie de la valeur d'une cellule lorsque [Style.getQuotePrefix()](../../com.aspose.cells/style\\#getQuotePrefix--) est vrai pour celle-ci. |
| [getFormatStrategy()](#getFormatStrategy--) | Obtient la stratégie de format lors de l'exportation de la valeur de la cellule en tant que chaîne. |
| [getKeepSeparatorsForBlankRow()](#getKeepSeparatorsForBlankRow--) | Indique si les séparateurs doivent être générés pour une ligne vide. |
| [getLightCellsDataProvider()](#getLightCellsDataProvider--) | Le fournisseur de données pour enregistrer le classeur en mode léger. |
| [getMergeAreas()](#getMergeAreas--) | Indique s'il faut fusionner les zones de mise en forme conditionnelle et de validation avant d'enregistrer le fichier. |
| [getQuoteType()](#getQuoteType--) | Obtient la façon de citer les valeurs dans le fichier texte exporté. |
| [getRefreshChartCache()](#getRefreshChartCache--) | Indique s'il faut mettre en cache les dernières données du graphique. |
| [getSaveFormat()](#getSaveFormat--) | Obtient le format de fichier d'enregistrement. |
| [getSeparator()](#getSeparator--) | Obtient le caractère délimiteur du fichier texte. |
| [getSeparatorString()](#getSeparatorString--) | Obtient une valeur chaîne comme séparateur. |
| [getSortExternalNames()](#getSortExternalNames--) | Indique s'il faut trier les noms définis externes avant d'enregistrer le fichier. |
| [getSortNames()](#getSortNames--) | Indique s'il faut trier les noms définis avant d'enregistrer le fichier. |
| [getTrimLeadingBlankRowAndColumn()](#getTrimLeadingBlankRowAndColumn--) | Indique si les lignes et colonnes vides en tête doivent être supprimées comme le fait MS Excel. |
| [getTrimTailingBlankCells()](#getTrimTailingBlankCells--) | Indique si les cellules vides en fin de ligne doivent être supprimées. |
| [getUpdateSmartArt()](#getUpdateSmartArt--) | Indique s'il faut mettre à jour le paramètre SmartArt. |
| [getValidateMergedAreas()](#getValidateMergedAreas--) | Indique s'il faut valider les cellules fusionnées avant d'enregistrer le fichier. |
| [getWarningCallback()](#getWarningCallback--) | Obtient le rappel d'avertissement. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAlwaysQuoted(boolean value)](#setAlwaysQuoted-boolean-) | Indique si l'ajout du caractère '\\"' est toujours effectué pour chaque champ. |
| [setCachedFileFolder(String value)](#setCachedFileFolder-java.lang.String-) | Le dossier pour les fichiers temporaires pouvant être utilisés comme cache de données. |
| [setCheckExcelRestriction(boolean value)](#setCheckExcelRestriction-boolean-) | Indique si la vérification des restrictions du fichier Excel est effectuée lorsque l'utilisateur modifie les objets liés aux cellules. |
| [setClearData(boolean value)](#setClearData-boolean-) | Rendre le classeur vide après l'enregistrement du fichier. |
| [setCreateDirectory(boolean value)](#setCreateDirectory-boolean-) | Si vrai et que le répertoire n'existe pas, le répertoire sera créé automatiquement avant d'enregistrer le fichier. |
| [setEncoding(Encoding value)](#setEncoding-com.aspose.cells.Encoding-) | Définit le codage par défaut. |
| [setEncryptDocumentProperties(boolean value)](#setEncryptDocumentProperties-boolean-) | Indique s'il faut chiffrer les propriétés du document lors de l'enregistrement au format .xls. |
| [setExportAllSheets(boolean value)](#setExportAllSheets-boolean-) | Indique si toutes les feuilles sont exportées vers le fichier texte. |
| [setExportArea(CellArea value)](#setExportArea-com.aspose.cells.CellArea-) | La plage de cellules à exporter. |
| [setExportQuotePrefix(boolean value)](#setExportQuotePrefix-boolean-) | Indique si le signe d'apostrophe simple doit être exporté comme faisant partie de la valeur d'une cellule lorsque [Style.getQuotePrefix()](../../com.aspose.cells/style\\#getQuotePrefix--) est vrai pour celle-ci. |
| [setFormatStrategy(int value)](#setFormatStrategy-int-) | Définit la stratégie de format lors de l'exportation de la valeur de la cellule en tant que chaîne. |
| [setKeepSeparatorsForBlankRow(boolean value)](#setKeepSeparatorsForBlankRow-boolean-) | Indique si les séparateurs doivent être générés pour une ligne vide. |
| [setLightCellsDataProvider(LightCellsDataProvider value)](#setLightCellsDataProvider-com.aspose.cells.LightCellsDataProvider-) | Le fournisseur de données pour enregistrer le classeur en mode léger. |
| [setMergeAreas(boolean value)](#setMergeAreas-boolean-) | Indique s'il faut fusionner les zones de mise en forme conditionnelle et de validation avant d'enregistrer le fichier. |
| [setQuoteType(int value)](#setQuoteType-int-) | Définit la façon de citer les valeurs dans le fichier texte exporté. |
| [setRefreshChartCache(boolean value)](#setRefreshChartCache-boolean-) | Indique s'il faut mettre en cache les dernières données du graphique. |
| [setSeparator(char value)](#setSeparator-char-) | Définit le caractère délimiteur du fichier texte. |
| [setSeparatorString(String value)](#setSeparatorString-java.lang.String-) | Définit une valeur chaîne comme séparateur. |
| [setSortExternalNames(boolean value)](#setSortExternalNames-boolean-) | Indique s'il faut trier les noms définis externes avant d'enregistrer le fichier. |
| [setSortNames(boolean value)](#setSortNames-boolean-) | Indique s'il faut trier les noms définis avant d'enregistrer le fichier. |
| [setTrimLeadingBlankRowAndColumn(boolean value)](#setTrimLeadingBlankRowAndColumn-boolean-) | Indique si les lignes et colonnes vides en tête doivent être supprimées comme le fait MS Excel. |
| [setTrimTailingBlankCells(boolean value)](#setTrimTailingBlankCells-boolean-) | Indique si les cellules vides en fin de ligne doivent être supprimées. |
| [setUpdateSmartArt(boolean value)](#setUpdateSmartArt-boolean-) | Indique s'il faut mettre à jour le paramètre SmartArt. |
| [setValidateMergedAreas(boolean value)](#setValidateMergedAreas-boolean-) | Indique s'il faut valider les cellules fusionnées avant d'enregistrer le fichier. |
| [setWarningCallback(IWarningCallback value)](#setWarningCallback-com.aspose.cells.IWarningCallback-) | Définit le rappel d’avertissement. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### TxtSaveOptions() {#TxtSaveOptions--}
```
public TxtSaveOptions()
```


Crée des options d'enregistrement de fichier texte.

### TxtSaveOptions(int saveFormat) {#TxtSaveOptions-int-}
```
public TxtSaveOptions(int saveFormat)
```


Crée des options d'enregistrement de fichier texte.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| saveFormat | int | [SaveFormat](../../com.aspose.cells/saveformat). Le format de fichier. Il doit être [SaveFormat.CSV](../../com.aspose.cells/saveformat\\#CSV) ou [SaveFormat.TSV](../../com.aspose.cells/saveformat\\#TSV), sinon le format enregistré sera automatiquement défini sur [SaveFormat.CSV](../../com.aspose.cells/saveformat\\#CSV). |

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
### getAlwaysQuoted() {#getAlwaysQuoted--}
```
public boolean getAlwaysQuoted()
```


Indique si l'ajout du caractère '\\"' est toujours effectué pour chaque champ. Si vrai, toutes les valeurs seront entre guillemets ; si faux, les valeurs ne seront entre guillemets que lorsque cela est nécessaire (par exemple, lorsque les valeurs contiennent des caractères spéciaux tels que '\\"', '\\n' ou le caractère séparateur). La valeur par défaut est false.

**Remarks**

NOTE : Ce membre est maintenant obsolète. À la place, veuillez utiliser la propriété QuoteType. Cette propriété sera supprimée 12 mois plus tard depuis août 2012. Aspose s'excuse pour tout désagrément que vous avez pu rencontrer.

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
### getEncoding() {#getEncoding--}
```
public Encoding getEncoding()
```


Obtient le codage par défaut.

**Returns:**
[Encoding](../../com.aspose.cells/encoding)
### getEncryptDocumentProperties() {#getEncryptDocumentProperties--}
```
public boolean getEncryptDocumentProperties()
```


Indique si les propriétés du document sont chiffrées lors de l'enregistrement au format .xls. La valeur par défaut est true.

**Remarks**

Uniquement pour les fichiers .xls, .xlsx, .xlsb et .xlsm.

**Returns:**
boolean
### getExportAllSheets() {#getExportAllSheets--}
```
public boolean getExportAllSheets()
```


Indique si toutes les feuilles sont exportées vers le fichier texte. Si false, seule la feuille active est exportée, comme le fait MS Excel.

**Remarks**

La valeur par défaut est false.

**Returns:**
boolean
### getExportArea() {#getExportArea--}
```
public CellArea getExportArea()
```


La plage de cellules à exporter.

**Remarks**

Si la zone exportée a été spécifiée, [getTrimLeadingBlankRowAndColumn()](../../com.aspose.cells/txtsaveoptions\#getTrimLeadingBlankRowAndColumn--) ne prendra aucun effet.

**Returns:**
[CellArea](../../com.aspose.cells/cellarea)
### getExportQuotePrefix() {#getExportQuotePrefix--}
```
public boolean getExportQuotePrefix()
```


Indique si le signe d'apostrophe doit être exporté comme partie de la valeur d'une cellule lorsque [Style.getQuotePrefix()](../../com.aspose.cells/style\#getQuotePrefix--) est vrai pour celle-ci. La valeur par défaut est false.

**Returns:**
boolean
### getFormatStrategy() {#getFormatStrategy--}
```
public int getFormatStrategy()
```


Obtient la stratégie de format lors de l'exportation de la valeur de la cellule en tant que chaîne.

Voir [CellValueFormatStrategy](../../com.aspose.cells/cellvalueformatstrategy).

**Returns:**
int
### getKeepSeparatorsForBlankRow() {#getKeepSeparatorsForBlankRow--}
```
public boolean getKeepSeparatorsForBlankRow()
```


Indique si des séparateurs doivent être générés pour une ligne vide. La valeur par défaut est false, ainsi le contenu d'une ligne vide sera vide par défaut.

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
### getQuoteType() {#getQuoteType--}
```
public int getQuoteType()
```


Obtient la façon de citer les valeurs dans le fichier texte exporté.

Voir [TxtValueQuoteType](../../com.aspose.cells/txtvaluequotetype).

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
### getSeparator() {#getSeparator--}
```
public char getSeparator()
```


Obtient le caractère délimiteur du fichier texte.

**Returns:**
char
### getSeparatorString() {#getSeparatorString--}
```
public String getSeparatorString()
```


Obtient une valeur chaîne comme séparateur.

**Returns:**
java.lang.String
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
### getTrimLeadingBlankRowAndColumn() {#getTrimLeadingBlankRowAndColumn--}
```
public boolean getTrimLeadingBlankRowAndColumn()
```


Indique si les lignes et colonnes vides en début doivent être supprimées comme le fait ms excel. La valeur par défaut est true.

**Remarks**

Même règle que dans ms excel, une ligne/colonne ne sera pas considérée comme vide si elle possède un style personnalisé, même si elle ne contient aucune donnée de cellule. Lors de l'enregistrement en mode LightCells, cette option n'a aucun effet. L'utilisateur doit contrôler la plage de sortie via l'implémentation de [getLightCellsDataProvider()](../../com.aspose.cells/txtsaveoptions\#getLightCellsDataProvider--) ou en spécifiant [getExportArea()](../../com.aspose.cells/txtsaveoptions\#getExportArea--).

**Returns:**
boolean
### getTrimTailingBlankCells() {#getTrimTailingBlankCells--}
```
public boolean getTrimTailingBlankCells()
```


Indique si les cellules vides en fin de ligne doivent être supprimées. La valeur par défaut est false.

**Remarks**

Lors de l'enregistrement en mode LightCells et si [getExportArea()](../../com.aspose.cells/txtsaveoptions\#getExportArea--) n'a pas été spécifié, cette option n'a aucun effet et une ligne sera étendue jusqu'à la dernière cellule fournie par l'implémentation [getLightCellsDataProvider()](../../com.aspose.cells/txtsaveoptions\#getLightCellsDataProvider--).

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
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### setAlwaysQuoted(boolean value) {#setAlwaysQuoted-boolean-}
```
public void setAlwaysQuoted(boolean value)
```


Indique si l'ajout du caractère '\\"' est toujours effectué pour chaque champ. Si vrai, toutes les valeurs seront entre guillemets ; si faux, les valeurs ne seront entre guillemets que lorsque cela est nécessaire (par exemple, lorsque les valeurs contiennent des caractères spéciaux tels que '\\"', '\\n' ou le caractère séparateur). La valeur par défaut est false.

**Remarks**

NOTE : Ce membre est maintenant obsolète. À la place, veuillez utiliser la propriété QuoteType. Cette propriété sera supprimée 12 mois plus tard depuis août 2012. Aspose s'excuse pour tout désagrément que vous avez pu rencontrer.

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

### setEncoding(Encoding value) {#setEncoding-com.aspose.cells.Encoding-}
```
public void setEncoding(Encoding value)
```


Définit le codage par défaut.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | [Encoding](../../com.aspose.cells/encoding) |  |

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

### setExportAllSheets(boolean value) {#setExportAllSheets-boolean-}
```
public void setExportAllSheets(boolean value)
```


Indique si toutes les feuilles sont exportées vers le fichier texte. Si false, seule la feuille active est exportée, comme le fait MS Excel.

**Remarks**

La valeur par défaut est false.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setExportArea(CellArea value) {#setExportArea-com.aspose.cells.CellArea-}
```
public void setExportArea(CellArea value)
```


La plage de cellules à exporter.

**Remarks**

Si la zone exportée a été spécifiée, [getTrimLeadingBlankRowAndColumn()](../../com.aspose.cells/txtsaveoptions\#getTrimLeadingBlankRowAndColumn--) ne prendra aucun effet.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | [CellArea](../../com.aspose.cells/cellarea) |  |

### setExportQuotePrefix(boolean value) {#setExportQuotePrefix-boolean-}
```
public void setExportQuotePrefix(boolean value)
```


Indique si le signe d'apostrophe doit être exporté comme partie de la valeur d'une cellule lorsque [Style.getQuotePrefix()](../../com.aspose.cells/style\#getQuotePrefix--) est vrai pour celle-ci. La valeur par défaut est false.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setFormatStrategy(int value) {#setFormatStrategy-int-}
```
public void setFormatStrategy(int value)
```


Définit la stratégie de format lors de l'exportation de la valeur de la cellule en tant que chaîne.

Voir [CellValueFormatStrategy](../../com.aspose.cells/cellvalueformatstrategy).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setKeepSeparatorsForBlankRow(boolean value) {#setKeepSeparatorsForBlankRow-boolean-}
```
public void setKeepSeparatorsForBlankRow(boolean value)
```


Indique si des séparateurs doivent être générés pour une ligne vide. La valeur par défaut est false, ainsi le contenu d'une ligne vide sera vide par défaut.

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

### setQuoteType(int value) {#setQuoteType-int-}
```
public void setQuoteType(int value)
```


Définit la façon de citer les valeurs dans le fichier texte exporté.

Voir [TxtValueQuoteType](../../com.aspose.cells/txtvaluequotetype).

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

### setSeparator(char value) {#setSeparator-char-}
```
public void setSeparator(char value)
```


Définit le caractère délimiteur du fichier texte.

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

### setTrimLeadingBlankRowAndColumn(boolean value) {#setTrimLeadingBlankRowAndColumn-boolean-}
```
public void setTrimLeadingBlankRowAndColumn(boolean value)
```


Indique si les lignes et colonnes vides en début doivent être supprimées comme le fait ms excel. La valeur par défaut est true.

**Remarks**

Même règle que dans ms excel, une ligne/colonne ne sera pas considérée comme vide si elle possède un style personnalisé, même si elle ne contient aucune donnée de cellule. Lors de l'enregistrement en mode LightCells, cette option n'a aucun effet. L'utilisateur doit contrôler la plage de sortie via l'implémentation de [getLightCellsDataProvider()](../../com.aspose.cells/txtsaveoptions\#getLightCellsDataProvider--) ou en spécifiant [getExportArea()](../../com.aspose.cells/txtsaveoptions\#getExportArea--).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setTrimTailingBlankCells(boolean value) {#setTrimTailingBlankCells-boolean-}
```
public void setTrimTailingBlankCells(boolean value)
```


Indique si les cellules vides en fin de ligne doivent être supprimées. La valeur par défaut est false.

**Remarks**

Lors de l'enregistrement en mode LightCells et si [getExportArea()](../../com.aspose.cells/txtsaveoptions\#getExportArea--) n'a pas été spécifié, cette option n'a aucun effet et une ligne sera étendue jusqu'à la dernière cellule fournie par l'implémentation [getLightCellsDataProvider()](../../com.aspose.cells/txtsaveoptions\#getLightCellsDataProvider--).

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

