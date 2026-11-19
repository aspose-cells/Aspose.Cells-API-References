---
title: "GridHtmlSaveOptions"
second_title: "Référence API d'Aspose.Cells pour Java"
description: "Représente les options d'enregistrement du fichier html."
type: docs
url: /fr/java/com.aspose.gridweb/gridhtmlsaveoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.gridweb.GridSaveOptions](../../com.aspose.gridweb/gridsaveoptions)
```
public class GridHtmlSaveOptions extends GridSaveOptions
```

Représente les options d'enregistrement du fichier html.
## Constructeurs

| Constructeur | Description |
| --- | --- |
| [GridHtmlSaveOptions()](#GridHtmlSaveOptions--) | Crée des options pour enregistrer un fichier html. |
| [GridHtmlSaveOptions(int format)](#GridHtmlSaveOptions-int-) | Crée des options pour enregistrer un fichier htm. |
## Méthodes

| Méthode | Description |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAttachedFilesDirectory()](#getAttachedFilesDirectory--) | Le répertoire où les fichiers joints seront enregistrés. |
| [getAttachedFilesUrlPrefix()](#getAttachedFilesUrlPrefix--) | Spécifie le préfixe d'URL des fichiers joints tels que les images dans le fichier HTML. |
| [getCachedFileFolder()](#getCachedFileFolder--) | Le dossier de fichiers en cache est utilisé pour stocker des données volumineuses. |
| [getClass()](#getClass--) |  |
| [getClearData()](#getClearData--) | Rendre le classeur vide après l'enregistrement du fichier. |
| [getCreateDirectory()](#getCreateDirectory--) | Si vrai et que le répertoire n'existe pas, le répertoire sera créé automatiquement avant d'enregistrer le fichier. |
| [getDefaultFontName()](#getDefaultFontName--) | Spécifie le nom de police par défaut pour l'exportation HTML, la police par défaut sera utilisée lorsque la police du style n'existe pas. Si cette propriété est null, Aspose.Cells utilisera une police universelle ayant la même famille que la police originale, la valeur par défaut est null. |
| [getEncoding()](#getEncoding--) | Si non défini, utilise Encoding.UTF8 comme type d'encodage par défaut. |
| [getExportActiveWorksheetOnly()](#getExportActiveWorksheetOnly--) | Indique si l'exportation du classeur complet vers un fichier html. |
| [getExportArea()](#getExportArea--) | Obtient la zone de cellules (CellArea) exportée de la feuille de calcul active actuelle. |
| [getExportGridLines()](#getExportGridLines--) | Indique si l'exportation des quadrillages. La valeur par défaut est false. |
| [getExportHeadings()](#getExportHeadings--) | Indique si les en-têtes sont exportés lors de l'enregistrement du fichier au format html. La valeur par défaut est false. |
| [getExportHiddenWorksheet()](#getExportHiddenWorksheet--) | Indique si le contenu de la feuille de calcul masqué est exporté. La valeur par défaut est true. |
| [getExportImagesAsBase64()](#getExportImagesAsBase64--) | Spécifie si les images sont enregistrées au format Base64 dans HTML, MHTML ou EPUB. |
| [getExportPrintAreaOnly()](#getExportPrintAreaOnly--) | Indique si seule la zone d'impression est exportée vers le fichier HTML. |
| [getExportSingleTab()](#getExportSingleTab--) | Indique si l'onglet unique est exporté lorsque le fichier ne contient qu'une seule feuille de calcul. |
| [getMergeAreas()](#getMergeAreas--) | Indique s'il faut fusionner les zones de mise en forme conditionnelle et de validation avant d'enregistrer le fichier. |
| [getPageTitle()](#getPageTitle--) | Le titre de la page HTML. |
|  | [getParseHtmlTagInCell()](#getParseHtmlTagInCell--) | Analyser la balise html dans la cellule, comme |

, comme valeur de cellule, ou comme balise html, la valeur par défaut est true |
| [getPresentationPreference()](#getPresentationPreference--) | Indique si le fichier html ou mht est la préférence de présentation. La valeur par défaut est false. Si vous souhaitez obtenir une présentation plus esthétique, veuillez définir la valeur sur true. |
| [getRefreshChartCache()](#getRefreshChartCache--) | Indique si les données du cache du graphique sont rafraîchies. |
| [getSaveFormat()](#getSaveFormat--) | Obtient le format de fichier d'enregistrement. |
| [getSortNames()](#getSortNames--) | Indique s'il faut trier les noms définis avant d'enregistrer le fichier. |
| [getValidateMergedAreas()](#getValidateMergedAreas--) | Indique s'il faut valider les cellules fusionnées avant d'enregistrer le fichier. |
| [hashCode()](#hashCode--) |  |
| [isExportComments()](#isExportComments--) | Indique si les commentaires sont exportés lors de l'enregistrement du fichier en HTML, la valeur par défaut est false. |
| [isFullPathLink()](#isFullPathLink--) | Indication si l'on utilise un lien avec le chemin complet dans sheet00x.htm, filelist.xml et tabstrip.htm. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAttachedFilesDirectory(String value)](#setAttachedFilesDirectory-java.lang.String-) | Le répertoire où les fichiers joints seront enregistrés. |
| [setAttachedFilesUrlPrefix(String value)](#setAttachedFilesUrlPrefix-java.lang.String-) | Spécifie le préfixe d'URL des fichiers joints tels que les images dans le fichier HTML. |
| [setCachedFileFolder(String value)](#setCachedFileFolder-java.lang.String-) | Le dossier de fichiers en cache est utilisé pour stocker des données volumineuses. |
| [setClearData(boolean value)](#setClearData-boolean-) | Rendre le classeur vide après l'enregistrement du fichier. |
| [setCreateDirectory(boolean value)](#setCreateDirectory-boolean-) | Si vrai et que le répertoire n'existe pas, le répertoire sera créé automatiquement avant d'enregistrer le fichier. |
| [setDefaultFontName(String value)](#setDefaultFontName-java.lang.String-) | Spécifie le nom de police par défaut pour l'exportation HTML, la police par défaut sera utilisée lorsque la police du style n'existe pas. Si cette propriété est null, Aspose.Cells utilisera une police universelle ayant la même famille que la police originale, la valeur par défaut est null. |
| [setEncoding(Encoding value)](#setEncoding-com.aspose.gridweb.Encoding-) | Si non défini, utilise Encoding.UTF8 comme type d'encodage par défaut. |
| [setExportActiveWorksheetOnly(boolean value)](#setExportActiveWorksheetOnly-boolean-) | Indique si l'exportation du classeur complet vers un fichier html. |
| [setExportArea(GridCellArea value)](#setExportArea-com.aspose.gridweb.GridCellArea-) | Définit la CellArea d'exportation de la Worksheet active actuelle. |
| [setExportComments(boolean value)](#setExportComments-boolean-) | Indique si les commentaires sont exportés lors de l'enregistrement du fichier en HTML, la valeur par défaut est false. |
| [setExportGridLines(boolean value)](#setExportGridLines-boolean-) | Indique si l'exportation des quadrillages. La valeur par défaut est false. |
| [setExportHeadings(boolean value)](#setExportHeadings-boolean-) | Indique si les en-têtes sont exportés lors de l'enregistrement du fichier au format html. La valeur par défaut est false. |
| [setExportHiddenWorksheet(boolean value)](#setExportHiddenWorksheet-boolean-) | Indique si le contenu de la feuille de calcul masqué est exporté. La valeur par défaut est true. |
| [setExportImagesAsBase64(boolean value)](#setExportImagesAsBase64-boolean-) | Spécifie si les images sont enregistrées au format Base64 dans HTML, MHTML ou EPUB. |
| [setExportPrintAreaOnly(boolean value)](#setExportPrintAreaOnly-boolean-) | Indique si seule la zone d'impression est exportée vers le fichier HTML. |
| [setExportSingleTab(boolean value)](#setExportSingleTab-boolean-) | Indique si l'onglet unique est exporté lorsque le fichier ne contient qu'une seule feuille de calcul. |
| [setFullPathLink(boolean value)](#setFullPathLink-boolean-) | Indication si l'on utilise un lien avec le chemin complet dans sheet00x.htm, filelist.xml et tabstrip.htm. |
| [setMergeAreas(boolean value)](#setMergeAreas-boolean-) | Indique s'il faut fusionner les zones de mise en forme conditionnelle et de validation avant d'enregistrer le fichier. |
| [setPageTitle(String value)](#setPageTitle-java.lang.String-) | Le titre de la page HTML. |
|  | [setParseHtmlTagInCell(boolean value)](#setParseHtmlTagInCell-boolean-) | Analyser la balise html dans la cellule, comme |

, comme valeur de cellule, ou comme balise html, la valeur par défaut est true |
| [setPresentationPreference(boolean value)](#setPresentationPreference-boolean-) | Indique si le fichier html ou mht est la préférence de présentation. La valeur par défaut est false. Si vous souhaitez obtenir une présentation plus esthétique, veuillez définir la valeur sur true. |
| [setRefreshChartCache(boolean value)](#setRefreshChartCache-boolean-) | Indique si les données du cache du graphique sont rafraîchies. |
| [setSortNames(boolean value)](#setSortNames-boolean-) | Indique s'il faut trier les noms définis avant d'enregistrer le fichier. |
| [setValidateMergedAreas(boolean value)](#setValidateMergedAreas-boolean-) | Indique s'il faut valider les cellules fusionnées avant d'enregistrer le fichier. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### GridHtmlSaveOptions() {#GridHtmlSaveOptions--}
```
public GridHtmlSaveOptions()
```


Crée des options pour enregistrer un fichier html.

### GridHtmlSaveOptions(int format) {#GridHtmlSaveOptions-int-}
```
public GridHtmlSaveOptions(int format)
```


Crée des options pour enregistrer un fichier htm.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| format | int | [GridSaveFormat](../../com.aspose.gridweb/gridsaveformat). Le format de fichier d'enregistrement. |

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
### getAttachedFilesDirectory() {#getAttachedFilesDirectory--}
```
public String getAttachedFilesDirectory()
```


Le répertoire où les fichiers joints seront enregistrés. Seulement pour l'enregistrement dans un flux html.

**Returns:**
java.lang.String
### getAttachedFilesUrlPrefix() {#getAttachedFilesUrlPrefix--}
```
public String getAttachedFilesUrlPrefix()
```


Spécifiez le préfixe Url des fichiers joints tels que les images dans le fichier html. Seulement pour l'enregistrement dans un flux html.

**Returns:**
java.lang.String
### getCachedFileFolder() {#getCachedFileFolder--}
```
public String getCachedFileFolder()
```


Le dossier de fichiers en cache est utilisé pour stocker des données volumineuses.

**Returns:**
java.lang.String
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
### getDefaultFontName() {#getDefaultFontName--}
```
public String getDefaultFontName()
```


Spécifie le nom de police par défaut pour l'exportation HTML, la police par défaut sera utilisée lorsque la police du style n'existe pas. Si cette propriété est null, Aspose.Cells utilisera une police universelle ayant la même famille que la police originale, la valeur par défaut est null.

**Returns:**
java.lang.String
### getEncoding() {#getEncoding--}
```
public Encoding getEncoding()
```


Si non défini, utilise Encoding.UTF8 comme type d'encodage par défaut.

**Returns:**
[Encoding](../../com.aspose.gridweb/encoding)
### getExportActiveWorksheetOnly() {#getExportActiveWorksheetOnly--}
```
public boolean getExportActiveWorksheetOnly()
```


Indique si l'exportation du classeur complet vers un fichier html.

**Returns:**
boolean
### getExportArea() {#getExportArea--}
```
public GridCellArea getExportArea()
```


Obtient la CellArea d'exportation de la feuille de calcul active actuelle. Si vous définissez cet attribut, la zone d'impression de la feuille de calcul active actuelle sera omise. Seule la zone spécifiée sera exportée lors de l'enregistrement du fichier au format html.

**Returns:**
[GridCellArea](../../com.aspose.gridweb/gridcellarea)
### getExportGridLines() {#getExportGridLines--}
```
public boolean getExportGridLines()
```


Indique si l'exportation des quadrillages. La valeur par défaut est false.

**Returns:**
boolean
### getExportHeadings() {#getExportHeadings--}
```
public boolean getExportHeadings()
```


Indique si les en-têtes sont exportés lors de l'enregistrement du fichier au format html. La valeur par défaut est false. Si vous souhaitez importer le fichier html dans Excel, veuillez conserver la valeur par défaut.

**Returns:**
boolean
### getExportHiddenWorksheet() {#getExportHiddenWorksheet--}
```
public boolean getExportHiddenWorksheet()
```


Indique si le contenu de la feuille de calcul masqué est exporté. La valeur par défaut est true.

**Returns:**
boolean
### getExportImagesAsBase64() {#getExportImagesAsBase64--}
```
public boolean getExportImagesAsBase64()
```


Spécifie si les images sont enregistrées au format Base64 dans HTML, MHTML ou EPUB.

**Remarks**

Lorsque cette propriété est définie sur true, les données d'image sont exportées directement dans les éléments img et aucun fichier séparé n'est créé.

**Returns:**
boolean
### getExportPrintAreaOnly() {#getExportPrintAreaOnly--}
```
public boolean getExportPrintAreaOnly()
```


Indique si seule la zone d'impression doit être exportée vers le fichier html. La valeur par défaut est false.

**Returns:**
boolean
### getExportSingleTab() {#getExportSingleTab--}
```
public boolean getExportSingleTab()
```


Indique si l'exportation de l'onglet unique doit être effectuée lorsque le fichier ne contient qu'une seule feuille de calcul. La valeur par défaut est false.

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
### getPageTitle() {#getPageTitle--}
```
public String getPageTitle()
```


Le titre de la page html. Uniquement pour l'enregistrement dans un flux html.

**Returns:**
java.lang.String
### getParseHtmlTagInCell() {#getParseHtmlTagInCell--}
```
public boolean getParseHtmlTagInCell()
```


Analyser la balise html dans la cellule, comme

, comme valeur de cellule, ou comme balise html, la valeur par défaut est true

**Returns:**
boolean
### getPresentationPreference() {#getPresentationPreference--}
```
public boolean getPresentationPreference()
```


Indique si le fichier html ou mht est la préférence de présentation. La valeur par défaut est false. Si vous souhaitez obtenir une présentation plus esthétique, veuillez définir la valeur sur true.

**Returns:**
boolean
### getRefreshChartCache() {#getRefreshChartCache--}
```
public boolean getRefreshChartCache()
```


Indique si les données du cache du graphique sont rafraîchies.

**Returns:**
boolean
### getSaveFormat() {#getSaveFormat--}
```
public int getSaveFormat()
```


Obtient le format de fichier d'enregistrement.

Voir [GridSaveFormat](../../com.aspose.gridweb/gridsaveformat).

**Returns:**
int
### getSortNames() {#getSortNames--}
```
public boolean getSortNames()
```


Indique s'il faut trier les noms définis avant d'enregistrer le fichier.

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
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isExportComments() {#isExportComments--}
```
public boolean isExportComments()
```


Indique si les commentaires sont exportés lors de l'enregistrement du fichier en HTML, la valeur par défaut est false.

**Returns:**
boolean
### isFullPathLink() {#isFullPathLink--}
```
public boolean isFullPathLink()
```


Indique si l'on utilise des liens avec le chemin complet dans sheet00x.htm, filelist.xml et tabstrip.htm. La valeur par défaut est false.

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




### setAttachedFilesDirectory(String value) {#setAttachedFilesDirectory-java.lang.String-}
```
public void setAttachedFilesDirectory(String value)
```


Le répertoire où les fichiers joints seront enregistrés. Seulement pour l'enregistrement dans un flux html.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

### setAttachedFilesUrlPrefix(String value) {#setAttachedFilesUrlPrefix-java.lang.String-}
```
public void setAttachedFilesUrlPrefix(String value)
```


Spécifiez le préfixe Url des fichiers joints tels que les images dans le fichier html. Seulement pour l'enregistrement dans un flux html.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

### setCachedFileFolder(String value) {#setCachedFileFolder-java.lang.String-}
```
public void setCachedFileFolder(String value)
```


Le dossier de fichiers en cache est utilisé pour stocker des données volumineuses.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

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

### setDefaultFontName(String value) {#setDefaultFontName-java.lang.String-}
```
public void setDefaultFontName(String value)
```


Spécifie le nom de police par défaut pour l'exportation HTML, la police par défaut sera utilisée lorsque la police du style n'existe pas. Si cette propriété est null, Aspose.Cells utilisera une police universelle ayant la même famille que la police originale, la valeur par défaut est null.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

### setEncoding(Encoding value) {#setEncoding-com.aspose.gridweb.Encoding-}
```
public void setEncoding(Encoding value)
```


Si non défini, utilise Encoding.UTF8 comme type d'encodage par défaut.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | [Encoding](../../com.aspose.gridweb/encoding) |  |

### setExportActiveWorksheetOnly(boolean value) {#setExportActiveWorksheetOnly-boolean-}
```
public void setExportActiveWorksheetOnly(boolean value)
```


Indique si l'exportation du classeur complet vers un fichier html.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setExportArea(GridCellArea value) {#setExportArea-com.aspose.gridweb.GridCellArea-}
```
public void setExportArea(GridCellArea value)
```


Définit la CellArea d'exportation de la feuille de calcul active actuelle. Si vous définissez cet attribut, la zone d'impression de la feuille de calcul active actuelle sera omise. Seule la zone spécifiée sera exportée lors de l'enregistrement du fichier au format html.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | [GridCellArea](../../com.aspose.gridweb/gridcellarea) |  |

### setExportComments(boolean value) {#setExportComments-boolean-}
```
public void setExportComments(boolean value)
```


Indique si les commentaires sont exportés lors de l'enregistrement du fichier en HTML, la valeur par défaut est false.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setExportGridLines(boolean value) {#setExportGridLines-boolean-}
```
public void setExportGridLines(boolean value)
```


Indique si l'exportation des quadrillages. La valeur par défaut est false.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setExportHeadings(boolean value) {#setExportHeadings-boolean-}
```
public void setExportHeadings(boolean value)
```


Indique si les en-têtes sont exportés lors de l'enregistrement du fichier au format html. La valeur par défaut est false. Si vous souhaitez importer le fichier html dans Excel, veuillez conserver la valeur par défaut.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setExportHiddenWorksheet(boolean value) {#setExportHiddenWorksheet-boolean-}
```
public void setExportHiddenWorksheet(boolean value)
```


Indique si le contenu de la feuille de calcul masqué est exporté. La valeur par défaut est true.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setExportImagesAsBase64(boolean value) {#setExportImagesAsBase64-boolean-}
```
public void setExportImagesAsBase64(boolean value)
```


Spécifie si les images sont enregistrées au format Base64 dans HTML, MHTML ou EPUB.

**Remarks**

Lorsque cette propriété est définie sur true, les données d'image sont exportées directement dans les éléments img et aucun fichier séparé n'est créé.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setExportPrintAreaOnly(boolean value) {#setExportPrintAreaOnly-boolean-}
```
public void setExportPrintAreaOnly(boolean value)
```


Indique si seule la zone d'impression doit être exportée vers le fichier html. La valeur par défaut est false.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setExportSingleTab(boolean value) {#setExportSingleTab-boolean-}
```
public void setExportSingleTab(boolean value)
```


Indique si l'exportation de l'onglet unique doit être effectuée lorsque le fichier ne contient qu'une seule feuille de calcul. La valeur par défaut est false.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setFullPathLink(boolean value) {#setFullPathLink-boolean-}
```
public void setFullPathLink(boolean value)
```


Indique si l'on utilise des liens avec le chemin complet dans sheet00x.htm, filelist.xml et tabstrip.htm. La valeur par défaut est false.

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

### setPageTitle(String value) {#setPageTitle-java.lang.String-}
```
public void setPageTitle(String value)
```


Le titre de la page html. Uniquement pour l'enregistrement dans un flux html.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

### setParseHtmlTagInCell(boolean value) {#setParseHtmlTagInCell-boolean-}
```
public void setParseHtmlTagInCell(boolean value)
```


Analyser la balise html dans la cellule, comme

, comme valeur de cellule, ou comme balise html, la valeur par défaut est true

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setPresentationPreference(boolean value) {#setPresentationPreference-boolean-}
```
public void setPresentationPreference(boolean value)
```


Indique si le fichier html ou mht est la préférence de présentation. La valeur par défaut est false. Si vous souhaitez obtenir une présentation plus esthétique, veuillez définir la valeur sur true.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setRefreshChartCache(boolean value) {#setRefreshChartCache-boolean-}
```
public void setRefreshChartCache(boolean value)
```


Indique si les données du cache du graphique sont rafraîchies.

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

