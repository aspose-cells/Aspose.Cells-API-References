---
title: "MarkdownSaveOptions"
second_title: "Référence API d'Aspose.Cells pour Java"
description: "Représente les options d'enregistrement pour Markdown."
type: docs
url: /fr/java/com.aspose.cells/markdownsaveoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.SaveOptions](../../com.aspose.cells/saveoptions)
```
public class MarkdownSaveOptions extends SaveOptions
```

Représente les options d'enregistrement pour Markdown.
## Constructeurs

| Constructeur | Description |
| --- | --- |
| [MarkdownSaveOptions()](#MarkdownSaveOptions--) | Crée des options pour enregistrer le document markdown |
## Méthodes

| Méthode | Description |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAlignColumnPadding()](#getAlignColumnPadding--) | Indique si l'alignement des colonnes est activé pour les tables Markdown générées. |
| [getCachedFileFolder()](#getCachedFileFolder--) | Le dossier pour les fichiers temporaires pouvant être utilisés comme cache de données. |
| [getCalculateFormula()](#getCalculateFormula--) | Indique s'il faut calculer les formules avant d'enregistrer le fichier markdown. |
| [getCheckExcelRestriction()](#getCheckExcelRestriction--) | Indique si la vérification des restrictions du fichier Excel est effectuée lorsque l'utilisateur modifie les objets liés aux cellules. |
| [getClass()](#getClass--) |  |
| [getClearData()](#getClearData--) | Rendre le classeur vide après l'enregistrement du fichier. |
| [getCreateDirectory()](#getCreateDirectory--) | Si vrai et que le répertoire n'existe pas, le répertoire sera créé automatiquement avant d'enregistrer le fichier. |
| [getEncoding()](#getEncoding--) | Obtient le codage par défaut. |
| [getEncryptDocumentProperties()](#getEncryptDocumentProperties--) | Indique s'il faut chiffrer les propriétés du document lors de l'enregistrement au format .xls. |
| [getExportHyperlinkAsReference()](#getExportHyperlinkAsReference--) | Indique s'il faut exporter le hyperlien en utilisant des définitions de référence au lieu du format en ligne. |
| [getExportImagesAsBase64()](#getExportImagesAsBase64--) | Spécifie si les images sont enregistrées au format Base64 dans le Markdown. |
| [getFormatStrategy()](#getFormatStrategy--) | Obtient la stratégie de format lors de l'exportation de la valeur de la cellule en tant que chaîne. |
| [getImageOptions()](#getImageOptions--) | Obtenez l'objet ImageOrPrintOptions avant l'exportation |
| [getLightCellsDataProvider()](#getLightCellsDataProvider--) | Le fournisseur de données pour fournir les données des cellules lors de l'enregistrement du classeur en mode léger. |
| [getLineSeparator()](#getLineSeparator--) | Obtient le séparateur de ligne. |
| [getMergeAreas()](#getMergeAreas--) | Indique s'il faut fusionner les zones de mise en forme conditionnelle et de validation avant d'enregistrer le fichier. |
| [getOfficeMathOutputType()](#getOfficeMathOutputType--) | Indique comment les objets OfficeMath sont exportés vers le Markdown, la valeur par défaut est Image. |
| [getRefreshChartCache()](#getRefreshChartCache--) | Indique s'il faut mettre en cache les dernières données du graphique. |
| [getSaveFormat()](#getSaveFormat--) | Obtient le format de fichier d'enregistrement. |
| [getSheetSet()](#getSheetSet--) | Obtient les feuilles à rendre. |
| [getSortExternalNames()](#getSortExternalNames--) | Indique s'il faut trier les noms définis externes avant d'enregistrer le fichier. |
| [getSortNames()](#getSortNames--) | Indique s'il faut trier les noms définis avant d'enregistrer le fichier. |
| [getSplitTablesByBlankRow()](#getSplitTablesByBlankRow--) | Indique si les lignes vides de la feuille de calcul doivent être traitées comme des séparateurs de tableau lors de l'exportation vers le Markdown. |
| [getStreamProvider()](#getStreamProvider--) | Obtient le IStreamProvider pour l'exportation des objets. |
| [getTableHeaderType()](#getTableHeaderType--) | Obtient comment définir l'en-tête du tableau. |
| [getUpdateSmartArt()](#getUpdateSmartArt--) | Indique s'il faut mettre à jour le paramètre SmartArt. |
| [getValidateMergedAreas()](#getValidateMergedAreas--) | Indique s'il faut valider les cellules fusionnées avant d'enregistrer le fichier. |
| [getWarningCallback()](#getWarningCallback--) | Obtient le rappel d'avertissement. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAlignColumnPadding(char value)](#setAlignColumnPadding-char-) | Indique si l'alignement des colonnes est activé pour les tables Markdown générées. |
| [setCachedFileFolder(String value)](#setCachedFileFolder-java.lang.String-) | Le dossier pour les fichiers temporaires pouvant être utilisés comme cache de données. |
| [setCalculateFormula(boolean value)](#setCalculateFormula-boolean-) | Indique s'il faut calculer les formules avant d'enregistrer le fichier markdown. |
| [setCheckExcelRestriction(boolean value)](#setCheckExcelRestriction-boolean-) | Indique si la vérification des restrictions du fichier Excel est effectuée lorsque l'utilisateur modifie les objets liés aux cellules. |
| [setClearData(boolean value)](#setClearData-boolean-) | Rendre le classeur vide après l'enregistrement du fichier. |
| [setCreateDirectory(boolean value)](#setCreateDirectory-boolean-) | Si vrai et que le répertoire n'existe pas, le répertoire sera créé automatiquement avant d'enregistrer le fichier. |
| [setEncoding(Encoding value)](#setEncoding-com.aspose.cells.Encoding-) | Définit le codage par défaut. |
| [setEncryptDocumentProperties(boolean value)](#setEncryptDocumentProperties-boolean-) | Indique s'il faut chiffrer les propriétés du document lors de l'enregistrement au format .xls. |
| [setExportHyperlinkAsReference(boolean value)](#setExportHyperlinkAsReference-boolean-) | Indique s'il faut exporter le hyperlien en utilisant des définitions de référence au lieu du format en ligne. |
| [setExportImagesAsBase64(boolean value)](#setExportImagesAsBase64-boolean-) | Spécifie si les images sont enregistrées au format Base64 dans le Markdown. |
| [setFormatStrategy(int value)](#setFormatStrategy-int-) | Définit la stratégie de format lors de l'exportation de la valeur de la cellule en tant que chaîne. |
| [setLightCellsDataProvider(LightCellsDataProvider value)](#setLightCellsDataProvider-com.aspose.cells.LightCellsDataProvider-) | Le fournisseur de données pour fournir les données des cellules lors de l'enregistrement du classeur en mode léger. |
| [setLineSeparator(String value)](#setLineSeparator-java.lang.String-) | Définit le séparateur de ligne. |
| [setMergeAreas(boolean value)](#setMergeAreas-boolean-) | Indique s'il faut fusionner les zones de mise en forme conditionnelle et de validation avant d'enregistrer le fichier. |
| [setOfficeMathOutputType(int value)](#setOfficeMathOutputType-int-) | Indique comment les objets OfficeMath sont exportés vers le Markdown, la valeur par défaut est Image. |
| [setRefreshChartCache(boolean value)](#setRefreshChartCache-boolean-) | Indique s'il faut mettre en cache les dernières données du graphique. |
| [setSheetSet(SheetSet value)](#setSheetSet-com.aspose.cells.SheetSet-) | Définit les feuilles à rendre. |
| [setSortExternalNames(boolean value)](#setSortExternalNames-boolean-) | Indique s'il faut trier les noms définis externes avant d'enregistrer le fichier. |
| [setSortNames(boolean value)](#setSortNames-boolean-) | Indique s'il faut trier les noms définis avant d'enregistrer le fichier. |
| [setSplitTablesByBlankRow(boolean value)](#setSplitTablesByBlankRow-boolean-) | Indique si les lignes vides de la feuille de calcul doivent être traitées comme des séparateurs de tableau lors de l'exportation vers le Markdown. |
| [setStreamProvider(IStreamProvider value)](#setStreamProvider-com.aspose.cells.IStreamProvider-) | Définit le IStreamProvider pour l'exportation des objets. |
| [setTableHeaderType(int value)](#setTableHeaderType-int-) | Définit comment définir l'en-tête du tableau. |
| [setUpdateSmartArt(boolean value)](#setUpdateSmartArt-boolean-) | Indique s'il faut mettre à jour le paramètre SmartArt. |
| [setValidateMergedAreas(boolean value)](#setValidateMergedAreas-boolean-) | Indique s'il faut valider les cellules fusionnées avant d'enregistrer le fichier. |
| [setWarningCallback(IWarningCallback value)](#setWarningCallback-com.aspose.cells.IWarningCallback-) | Définit le rappel d’avertissement. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### MarkdownSaveOptions() {#MarkdownSaveOptions--}
```
public MarkdownSaveOptions()
```


Crée des options pour enregistrer le document markdown

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
### getAlignColumnPadding() {#getAlignColumnPadding--}
```
public char getAlignColumnPadding()
```


Indique si l'alignement des colonnes est activé pour les tables Markdown générées. Lorsqu'il est activé, les colonnes sont alignées en remplissant le contenu des cellules avec le caractère spécifié (généralement ' ' pour les espaces). Définissez à '\\0' pour désactiver l'alignement des colonnes (par défaut).

**Returns:**
char
### getCachedFileFolder() {#getCachedFileFolder--}
```
public String getCachedFileFolder()
```


Le dossier pour les fichiers temporaires pouvant être utilisés comme cache de données.

**Remarks**

Si le dossier n'a pas été spécifié, la valeur par défaut est [CellsHelper.getCacheFolder()](../../com.aspose.cells/cellshelper\#getCacheFolder--). Si sa valeur par défaut est nulle ou vide, ou a été spécifiée comme nulle ou vide, aucun fichier de cache ne sera utilisé lors de l'enregistrement du classeur.

**Returns:**
java.lang.String
### getCalculateFormula() {#getCalculateFormula--}
```
public boolean getCalculateFormula()
```


Indique s'il faut calculer les formules avant d'enregistrer le fichier markdown.

**Remarks**

La valeur par défaut est false.

**Returns:**
boolean
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
### getExportHyperlinkAsReference() {#getExportHyperlinkAsReference--}
```
public boolean getExportHyperlinkAsReference()
```


Indique s'il faut exporter le hyperlien en utilisant des définitions de référence au lieu du format en ligne. La valeur par défaut est false.

**Returns:**
boolean
### getExportImagesAsBase64() {#getExportImagesAsBase64--}
```
public boolean getExportImagesAsBase64()
```


Spécifie si les images sont enregistrées au format Base64 dans le Markdown. La valeur par défaut est true.

**Remarks**

Lorsque cette propriété est définie sur true, les données d'image sont exportées directement dans les éléments img et aucun fichier séparé n'est créé.

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
### getImageOptions() {#getImageOptions--}
```
public ImageOrPrintOptions getImageOptions()
```


Obtenez l'objet ImageOrPrintOptions avant l'exportation

**Returns:**
[ImageOrPrintOptions](../../com.aspose.cells/imageorprintoptions)
### getLightCellsDataProvider() {#getLightCellsDataProvider--}
```
public LightCellsDataProvider getLightCellsDataProvider()
```


Le fournisseur de données pour fournir les données des cellules lors de l'enregistrement du classeur en mode léger.

**Returns:**
[LightCellsDataProvider](../../com.aspose.cells/lightcellsdataprovider)
### getLineSeparator() {#getLineSeparator--}
```
public String getLineSeparator()
```


Obtient le séparateur de ligne.

**Returns:**
java.lang.String
### getMergeAreas() {#getMergeAreas--}
```
public boolean getMergeAreas()
```


Indique s'il faut fusionner les zones de mise en forme conditionnelle et de validation avant d'enregistrer le fichier.

**Remarks**

La valeur par défaut est false.

**Returns:**
boolean
### getOfficeMathOutputType() {#getOfficeMathOutputType--}
```
public int getOfficeMathOutputType()
```


Indique comment les objets OfficeMath sont exportés vers le Markdown, la valeur par défaut est Image.

Voir [HtmlOfficeMathOutputType](../../com.aspose.cells/htmlofficemathoutputtype).

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
### getSheetSet() {#getSheetSet--}
```
public SheetSet getSheetSet()
```


Obtient les feuilles à rendre. Par défaut, toutes les feuilles visibles du classeur : [SheetSet.getActive()](../../com.aspose.cells/sheetset\#getActive--).

**Remarks**

Le paramètre est ignoré lorsqu'il est utilisé dans [SheetRender](../../com.aspose.cells/sheetrender).

**Returns:**
[SheetSet](../../com.aspose.cells/sheetset)
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
### getSplitTablesByBlankRow() {#getSplitTablesByBlankRow--}
```
public boolean getSplitTablesByBlankRow()
```


Indique si les lignes vides de la feuille de calcul doivent être traitées comme des séparateurs de tableau lors de l'exportation vers le Markdown. La valeur par défaut est false.

**Returns:**
boolean
### getStreamProvider() {#getStreamProvider--}
```
public IStreamProvider getStreamProvider()
```


Obtient le IStreamProvider pour l'exportation des objets. Si `null`, les objets exportés seront enregistrés dans le même répertoire que le fichier de sortie.

**Returns:**
[IStreamProvider](../../com.aspose.cells/istreamprovider)
### getTableHeaderType() {#getTableHeaderType--}
```
public int getTableHeaderType()
```


Obtient comment définir l'en-tête du tableau.

Voir [MarkdownTableHeaderType](../../com.aspose.cells/markdowntableheadertype).

**Returns:**
int
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




### setAlignColumnPadding(char value) {#setAlignColumnPadding-char-}
```
public void setAlignColumnPadding(char value)
```


Indique si l'alignement des colonnes est activé pour les tables Markdown générées. Lorsqu'il est activé, les colonnes sont alignées en remplissant le contenu des cellules avec le caractère spécifié (généralement ' ' pour les espaces). Définissez à '\\0' pour désactiver l'alignement des colonnes (par défaut).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | char |  |

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

### setCalculateFormula(boolean value) {#setCalculateFormula-boolean-}
```
public void setCalculateFormula(boolean value)
```


Indique s'il faut calculer les formules avant d'enregistrer le fichier markdown.

**Remarks**

La valeur par défaut est false.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

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

### setExportHyperlinkAsReference(boolean value) {#setExportHyperlinkAsReference-boolean-}
```
public void setExportHyperlinkAsReference(boolean value)
```


Indique s'il faut exporter le hyperlien en utilisant des définitions de référence au lieu du format en ligne. La valeur par défaut est false.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setExportImagesAsBase64(boolean value) {#setExportImagesAsBase64-boolean-}
```
public void setExportImagesAsBase64(boolean value)
```


Spécifie si les images sont enregistrées au format Base64 dans le Markdown. La valeur par défaut est true.

**Remarks**

Lorsque cette propriété est définie sur true, les données d'image sont exportées directement dans les éléments img et aucun fichier séparé n'est créé.

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

### setLightCellsDataProvider(LightCellsDataProvider value) {#setLightCellsDataProvider-com.aspose.cells.LightCellsDataProvider-}
```
public void setLightCellsDataProvider(LightCellsDataProvider value)
```


Le fournisseur de données pour fournir les données des cellules lors de l'enregistrement du classeur en mode léger.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | [LightCellsDataProvider](../../com.aspose.cells/lightcellsdataprovider) |  |

### setLineSeparator(String value) {#setLineSeparator-java.lang.String-}
```
public void setLineSeparator(String value)
```


Définit le séparateur de ligne.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

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

### setOfficeMathOutputType(int value) {#setOfficeMathOutputType-int-}
```
public void setOfficeMathOutputType(int value)
```


Indique comment les objets OfficeMath sont exportés vers le Markdown, la valeur par défaut est Image.

Voir [HtmlOfficeMathOutputType](../../com.aspose.cells/htmlofficemathoutputtype).

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

### setSheetSet(SheetSet value) {#setSheetSet-com.aspose.cells.SheetSet-}
```
public void setSheetSet(SheetSet value)
```


Définit les feuilles à rendre. Par défaut, toutes les feuilles visibles du classeur : [SheetSet.getActive()](../../com.aspose.cells/sheetset\#getActive--).

**Remarks**

Le paramètre est ignoré lorsqu'il est utilisé dans [SheetRender](../../com.aspose.cells/sheetrender).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | [SheetSet](../../com.aspose.cells/sheetset) |  |

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

### setSplitTablesByBlankRow(boolean value) {#setSplitTablesByBlankRow-boolean-}
```
public void setSplitTablesByBlankRow(boolean value)
```


Indique si les lignes vides de la feuille de calcul doivent être traitées comme des séparateurs de tableau lors de l'exportation vers le Markdown. La valeur par défaut est false.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setStreamProvider(IStreamProvider value) {#setStreamProvider-com.aspose.cells.IStreamProvider-}
```
public void setStreamProvider(IStreamProvider value)
```


Définit le IStreamProvider pour l'exportation des objets. Si `null`, les objets exportés seront enregistrés dans le même répertoire que le fichier de sortie.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | [IStreamProvider](../../com.aspose.cells/istreamprovider) |  |

### setTableHeaderType(int value) {#setTableHeaderType-int-}
```
public void setTableHeaderType(int value)
```


Définit comment définir l'en-tête du tableau.

Voir [MarkdownTableHeaderType](../../com.aspose.cells/markdowntableheadertype).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

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

