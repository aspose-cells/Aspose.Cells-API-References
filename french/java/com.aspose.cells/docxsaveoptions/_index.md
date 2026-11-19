---
title: "DocxSaveOptions"
second_title: "Référence API d'Aspose.Cells pour Java"
description: "Représente les options d'enregistrement du fichier .docx."
type: docs
url: /fr/java/com.aspose.cells/docxsaveoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.SaveOptions](../../com.aspose.cells/saveoptions), [com.aspose.cells.PaginatedSaveOptions](../../com.aspose.cells/paginatedsaveoptions)
```
public class DocxSaveOptions extends PaginatedSaveOptions
```

Représente les options d'enregistrement du fichier .docx.
## Constructeurs

| Constructeur | Description |
| --- | --- |
| [DocxSaveOptions()](#DocxSaveOptions--) | Représente les options d'enregistrement du fichier .docx. |
| [DocxSaveOptions(boolean saveAsImage)](#DocxSaveOptions-boolean-) | Représente les options d'enregistrement du fichier .docx. |
## Méthodes

| Méthode | Description |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAllColumnsInOnePagePerSheet()](#getAllColumnsInOnePagePerSheet--) | Si AllColumnsInOnePagePerSheet est true, tout le contenu des colonnes d’une feuille sera généré sur une seule page dans le résultat. |
| [getAsFlatOpc()](#getAsFlatOpc--) | Indique si l'enregistrement se fait sous forme de fichier OPC plat qui peut être généré par Open XML SDK. |
| [getAsNormalView()](#getAsNormalView--) | Exportation du fichier Excel vers docx fiel en vue normale. |
| [getCachedFileFolder()](#getCachedFileFolder--) | Le dossier pour les fichiers temporaires pouvant être utilisés comme cache de données. |
| [getCheckExcelRestriction()](#getCheckExcelRestriction--) | Indique si la vérification des restrictions du fichier Excel est effectuée lorsque l'utilisateur modifie les objets liés aux cellules. |
| [getCheckFontCompatibility()](#getCheckFontCompatibility--) | Indique s’il faut vérifier la compatibilité des polices pour chaque caractère du texte. |
| [getCheckWorkbookDefaultFont()](#getCheckWorkbookDefaultFont--) | Lorsque les caractères dans Excel sont Unicode et ne sont pas définis avec la police correcte dans le style de cellule, ils peuvent apparaître sous forme de blocs dans le pdf, l’image. |
| [getClass()](#getClass--) |  |
| [getClearData()](#getClearData--) | Rendre le classeur vide après l'enregistrement du fichier. |
| [getCreateDirectory()](#getCreateDirectory--) | Si vrai et que le répertoire n'existe pas, le répertoire sera créé automatiquement avant d'enregistrer le fichier. |
| [getCustomRenderSettings()](#getCustomRenderSettings--) | Obtient les paramètres personnalisés pendant le rendu. |
| [getDefaultEditLanguage()](#getDefaultEditLanguage--) | Obtient la langue d’édition par défaut. |
| [getDefaultFont()](#getDefaultFont--) | Lorsque les caractères dans Excel sont Unicode et ne sont pas définis avec la police correcte dans le style de cellule, ils peuvent apparaître sous forme de blocs dans le pdf, l’image. |
| [getDrawObjectEventHandler()](#getDrawObjectEventHandler--) | Implémentez cette interface pour obtenir DrawObject et Bound lors du rendu. |
| [getEmbedXlsxAsChartDataSource()](#getEmbedXlsxAsChartDataSource--) | Indique si l'intégration d'un fichier xlsx comme source de données du graphique. |
| [getEmfRenderSetting()](#getEmfRenderSetting--) | Paramètre pour le rendu du métafichier Emf. |
| [getEncryptDocumentProperties()](#getEncryptDocumentProperties--) | Indique s'il faut chiffrer les propriétés du document lors de l'enregistrement au format .xls. |
| [getGridlineColor()](#getGridlineColor--) | Obtient la couleur des lignes de grille. |
| [getGridlineType()](#getGridlineType--) | Obtient le type des lignes de grille. |
| [getIgnoreError()](#getIgnoreError--) | Indique si vous devez masquer l’erreur lors du rendu. |
| [getMergeAreas()](#getMergeAreas--) | Indique s'il faut fusionner les zones de mise en forme conditionnelle et de validation avant d'enregistrer le fichier. |
| [getOnePagePerSheet()](#getOnePagePerSheet--) | Si OnePagePerSheet est true, tout le contenu d’une feuille sera généré sur une seule page dans le résultat. |
| [getOutputBlankPageWhenNothingToPrint()](#getOutputBlankPageWhenNothingToPrint--) | Indique s’il faut générer une page blanche lorsqu’il n’y a rien à imprimer. |
| [getPageCount()](#getPageCount--) | Obtient le nombre de pages à enregistrer. |
| [getPageIndex()](#getPageIndex--) | Obtient l’indice basé sur zéro de la première page à enregistrer. |
| [getPageSavingCallback()](#getPageSavingCallback--) | Contrôle/Indique la progression du processus d'enregistrement de la page. |
| [getPrintingPageType()](#getPrintingPageType--) | Indique quelles pages ne seront pas imprimées. |
| [getRefreshChartCache()](#getRefreshChartCache--) | Indique s'il faut mettre en cache les dernières données du graphique. |
| [getRenderingBehavior()](#getRenderingBehavior--) | Obtient les comportements de rendu spécifiques à Excel à appliquer. |
| [getSaveAsEditableShapes()](#getSaveAsEditableShapes--) | Enregistrez tous les objets de dessin en tant que formes modifiables dans le fichier Word, afin de pouvoir les modifier dans Word. |
| [getSaveAsEditableShaps()](#getSaveAsEditableShaps--) | Enregistrez tous les objets de dessin objecgts en tant que formes modifiables dans le fichier Word. Ainsi, vous pouvez les modifier dans Word. |
| [getSaveElementType()](#getSaveElementType--) | Indique quels éléments doivent être enregistrés. |
| [getSaveFormat()](#getSaveFormat--) | Obtient le format de fichier d'enregistrement. |
| [getSheetSet()](#getSheetSet--) | Obtient les feuilles à rendre. |
| [getSortExternalNames()](#getSortExternalNames--) | Indique s'il faut trier les noms définis externes avant d'enregistrer le fichier. |
| [getSortNames()](#getSortNames--) | Indique s'il faut trier les noms définis avant d'enregistrer le fichier. |
| [getTextCrossType()](#getTextCrossType--) | Obtient le type d'affichage du texte lorsque la largeur du texte est supérieure à la largeur de la cellule. |
| [getUpdateSmartArt()](#getUpdateSmartArt--) | Indique s'il faut mettre à jour le paramètre SmartArt. |
| [getValidateMergedAreas()](#getValidateMergedAreas--) | Indique s'il faut valider les cellules fusionnées avant d'enregistrer le fichier. |
| [getWarningCallback()](#getWarningCallback--) | Obtient le rappel d'avertissement. |
| [hashCode()](#hashCode--) |  |
| [isFontSubstitutionCharGranularity()](#isFontSubstitutionCharGranularity--) | Indique s'il faut uniquement substituer la police du caractère lorsque la police de la cellule n'est pas compatible. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAllColumnsInOnePagePerSheet(boolean value)](#setAllColumnsInOnePagePerSheet-boolean-) | Si AllColumnsInOnePagePerSheet est true, tout le contenu des colonnes d’une feuille sera généré sur une seule page dans le résultat. |
| [setAsFlatOpc(boolean value)](#setAsFlatOpc-boolean-) | Indique si l'enregistrement se fait sous forme de fichier OPC plat qui peut être généré par Open XML SDK. |
| [setAsNormalView(boolean value)](#setAsNormalView-boolean-) | Exportation du fichier Excel vers docx fiel en vue normale. |
| [setCachedFileFolder(String value)](#setCachedFileFolder-java.lang.String-) | Le dossier pour les fichiers temporaires pouvant être utilisés comme cache de données. |
| [setCheckExcelRestriction(boolean value)](#setCheckExcelRestriction-boolean-) | Indique si la vérification des restrictions du fichier Excel est effectuée lorsque l'utilisateur modifie les objets liés aux cellules. |
| [setCheckFontCompatibility(boolean value)](#setCheckFontCompatibility-boolean-) | Indique s’il faut vérifier la compatibilité des polices pour chaque caractère du texte. |
| [setCheckWorkbookDefaultFont(boolean value)](#setCheckWorkbookDefaultFont-boolean-) | Lorsque les caractères dans Excel sont Unicode et ne sont pas définis avec la police correcte dans le style de cellule, ils peuvent apparaître sous forme de blocs dans le pdf, l’image. |
| [setClearData(boolean value)](#setClearData-boolean-) | Rendre le classeur vide après l'enregistrement du fichier. |
| [setCreateDirectory(boolean value)](#setCreateDirectory-boolean-) | Si vrai et que le répertoire n'existe pas, le répertoire sera créé automatiquement avant d'enregistrer le fichier. |
| [setCustomRenderSettings(CustomRenderSettings value)](#setCustomRenderSettings-com.aspose.cells.CustomRenderSettings-) | Définit les paramètres personnalisés pendant le rendu. |
| [setDefaultEditLanguage(int value)](#setDefaultEditLanguage-int-) | Définit la langue d'édition par défaut. |
| [setDefaultFont(String value)](#setDefaultFont-java.lang.String-) | Lorsque les caractères dans Excel sont Unicode et ne sont pas définis avec la police correcte dans le style de cellule, ils peuvent apparaître sous forme de blocs dans le pdf, l’image. |
| [setDrawObjectEventHandler(DrawObjectEventHandler value)](#setDrawObjectEventHandler-com.aspose.cells.DrawObjectEventHandler-) | Implémentez cette interface pour obtenir DrawObject et Bound lors du rendu. |
| [setEmbedXlsxAsChartDataSource(boolean value)](#setEmbedXlsxAsChartDataSource-boolean-) | Indique si l'intégration d'un fichier xlsx comme source de données du graphique. |
| [setEmfRenderSetting(int value)](#setEmfRenderSetting-int-) | Paramètre pour le rendu du métafichier Emf. |
| [setEncryptDocumentProperties(boolean value)](#setEncryptDocumentProperties-boolean-) | Indique s'il faut chiffrer les propriétés du document lors de l'enregistrement au format .xls. |
| [setFontSubstitutionCharGranularity(boolean value)](#setFontSubstitutionCharGranularity-boolean-) | Indique s'il faut uniquement substituer la police du caractère lorsque la police de la cellule n'est pas compatible. |
| [setGridlineColor(Color value)](#setGridlineColor-com.aspose.cells.Color-) | Définit la couleur des lignes de grille. |
| [setGridlineType(int value)](#setGridlineType-int-) | Définit le type de ligne de grille. |
| [setIgnoreError(boolean value)](#setIgnoreError-boolean-) | Indique si vous devez masquer l’erreur lors du rendu. |
| [setMergeAreas(boolean value)](#setMergeAreas-boolean-) | Indique s'il faut fusionner les zones de mise en forme conditionnelle et de validation avant d'enregistrer le fichier. |
| [setOnePagePerSheet(boolean value)](#setOnePagePerSheet-boolean-) | Si OnePagePerSheet est true, tout le contenu d’une feuille sera généré sur une seule page dans le résultat. |
| [setOutputBlankPageWhenNothingToPrint(boolean value)](#setOutputBlankPageWhenNothingToPrint-boolean-) | Indique s’il faut générer une page blanche lorsqu’il n’y a rien à imprimer. |
| [setPageCount(int value)](#setPageCount-int-) | Définit le nombre de pages à enregistrer. |
| [setPageIndex(int value)](#setPageIndex-int-) | Définit l'index de base zéro de la première page à enregistrer. |
| [setPageSavingCallback(IPageSavingCallback value)](#setPageSavingCallback-com.aspose.cells.IPageSavingCallback-) | Contrôle/Indique la progression du processus d'enregistrement de la page. |
| [setPrintingPageType(int value)](#setPrintingPageType-int-) | Indique quelles pages ne seront pas imprimées. |
| [setRefreshChartCache(boolean value)](#setRefreshChartCache-boolean-) | Indique s'il faut mettre en cache les dernières données du graphique. |
| [setRenderingBehavior(int value)](#setRenderingBehavior-int-) | Définit les comportements de rendu spécifiques à Excel à appliquer. |
| [setSaveAsEditableShapes(boolean value)](#setSaveAsEditableShapes-boolean-) | Enregistrez tous les objets de dessin en tant que formes modifiables dans le fichier Word, afin de pouvoir les modifier dans Word. |
| [setSaveAsEditableShaps(boolean value)](#setSaveAsEditableShaps-boolean-) | Enregistrez tous les objets de dessin objecgts en tant que formes modifiables dans le fichier Word. Ainsi, vous pouvez les modifier dans Word. |
| [setSaveElementType(int value)](#setSaveElementType-int-) | Indique quels éléments doivent être enregistrés. |
| [setSheetSet(SheetSet value)](#setSheetSet-com.aspose.cells.SheetSet-) | Définit les feuilles à rendre. |
| [setSortExternalNames(boolean value)](#setSortExternalNames-boolean-) | Indique s'il faut trier les noms définis externes avant d'enregistrer le fichier. |
| [setSortNames(boolean value)](#setSortNames-boolean-) | Indique s'il faut trier les noms définis avant d'enregistrer le fichier. |
| [setTextCrossType(int value)](#setTextCrossType-int-) | Définit le type d'affichage du texte lorsque la largeur du texte est supérieure à la largeur de la cellule. |
| [setUpdateSmartArt(boolean value)](#setUpdateSmartArt-boolean-) | Indique s'il faut mettre à jour le paramètre SmartArt. |
| [setValidateMergedAreas(boolean value)](#setValidateMergedAreas-boolean-) | Indique s'il faut valider les cellules fusionnées avant d'enregistrer le fichier. |
| [setWarningCallback(IWarningCallback value)](#setWarningCallback-com.aspose.cells.IWarningCallback-) | Définit le rappel d’avertissement. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### DocxSaveOptions() {#DocxSaveOptions--}
```
public DocxSaveOptions()
```


Représente les options d'enregistrement du fichier .docx.

### DocxSaveOptions(boolean saveAsImage) {#DocxSaveOptions-boolean-}
```
public DocxSaveOptions(boolean saveAsImage)
```


Représente les options d'enregistrement du fichier .docx.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| saveAsImage | boolean | Si True, le classeur sera converti en quelques images du fichier .docx. Si False, le classeur sera converti en quelques tableaux du fichier .docx. |

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
### getAllColumnsInOnePagePerSheet() {#getAllColumnsInOnePagePerSheet--}
```
public boolean getAllColumnsInOnePagePerSheet()
```


Si AllColumnsInOnePagePerSheet est vrai, tout le contenu des colonnes d'une feuille sera exporté sur une seule page dans le résultat. La largeur du format de papier du paramètre pagesetup sera ignorée, et les autres paramètres de pagesetup resteront effectifs.

**Returns:**
boolean
### getAsFlatOpc() {#getAsFlatOpc--}
```
public boolean getAsFlatOpc()
```


Indique si l'enregistrement se fait sous forme de fichier OPC plat qui peut être généré par Open XML SDK.

**Returns:**
boolean
### getAsNormalView() {#getAsNormalView--}
```
public boolean getAsNormalView()
```


Exportation du fichier Excel vers un fichier docx en vue normale. Si cette propriété est true, une zone sera générée, et aucune échelle ne sera appliquée. La valeur par défaut est false.

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
### getCheckFontCompatibility() {#getCheckFontCompatibility--}
```
public boolean getCheckFontCompatibility()
```


Indique s’il faut vérifier la compatibilité des polices pour chaque caractère du texte.

**Remarks**

La valeur par défaut est true. Désactiver cette propriété peut améliorer les performances. Mais lorsque la police par défaut ou spécifiée du texte/caractère ne peut pas être utilisée pour le rendre, des caractères illisibles (comme des blocs) peuvent apparaître dans le PDF généré. Dans ce cas, l'utilisateur doit laisser cette propriété à true afin qu'une police alternative soit recherchée et utilisée pour rendre le texte à la place ;

**Returns:**
boolean
### getCheckWorkbookDefaultFont() {#getCheckWorkbookDefaultFont--}
```
public boolean getCheckWorkbookDefaultFont()
```


Lorsque les caractères dans Excel sont Unicode et ne sont pas définis avec la police correcte dans le style de cellule, ils peuvent apparaître sous forme de blocs dans le PDF ou l'image. Réglez ceci sur true pour essayer d'utiliser la police par défaut du classeur afin d'afficher d'abord ces caractères.

**Remarks**

La valeur par défaut est true.

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
### getCustomRenderSettings() {#getCustomRenderSettings--}
```
public CustomRenderSettings getCustomRenderSettings()
```


Obtient les paramètres personnalisés pendant le rendu.

**Returns:**
[CustomRenderSettings](../../com.aspose.cells/customrendersettings)
### getDefaultEditLanguage() {#getDefaultEditLanguage--}
```
public int getDefaultEditLanguage()
```


Obtient la langue d’édition par défaut.

Voir [DefaultEditLanguage](../../com.aspose.cells/defaulteditlanguage).

**Remarks**

Il peut afficher/rendre différentes mises en page pour le paragraphe de texte lorsque différentes langues d'édition sont définies. La valeur par défaut est [DefaultEditLanguage.AUTO](../../com.aspose.cells/defaulteditlanguage\\#AUTO).

**Returns:**
int
### getDefaultFont() {#getDefaultFont--}
```
public String getDefaultFont()
```


Lorsque les caractères dans Excel sont Unicode et ne sont pas définis avec la police correcte dans le style de cellule, ils peuvent apparaître sous forme de blocs dans le PDF ou l'image. Définissez la police par défaut (DefaultFont) comme MingLiu ou MS Gothic pour afficher ces caractères. Si cette propriété n'est pas définie, Aspose.Cells utilisera la police système par défaut pour afficher ces caractères Unicode.

**Returns:**
java.lang.String
### getDrawObjectEventHandler() {#getDrawObjectEventHandler--}
```
public DrawObjectEventHandler getDrawObjectEventHandler()
```


Implémentez cette interface pour obtenir DrawObject et Bound lors du rendu.

**Returns:**
[DrawObjectEventHandler](../../com.aspose.cells/drawobjecteventhandler)
### getEmbedXlsxAsChartDataSource() {#getEmbedXlsxAsChartDataSource--}
```
public boolean getEmbedXlsxAsChartDataSource()
```


Indique si l'intégration d'un fichier xlsx comme source de données du graphique.

**Remarks**

La valeur par défaut est true.

**Returns:**
boolean
### getEmfRenderSetting() {#getEmfRenderSetting--}
```
public int getEmfRenderSetting()
```


Paramètre pour le rendu du métafichier Emf.

Voir [EmfRenderSetting](../../com.aspose.cells/emfrendersetting).

**Remarks**

Les métafichiers EMF identifiés comme "EMF+ Dual" peuvent contenir à la fois des enregistrements EMF+ et des enregistrements EMF. Chaque type d'enregistrement peut être utilisé pour rendre l'image, uniquement les enregistrements EMF+, ou uniquement les enregistrements EMF. Lorsque [EmfRenderSetting.EMF\\_PLUS\\_PREFER](../../com.aspose.cells/emfrendersetting\\#EMF-PLUS-PREFER) est défini, les enregistrements EMF+ seront analysés lors du rendu de la page, sinon seuls les enregistrements EMF seront analysés. La valeur par défaut est [EmfRenderSetting.EMF\\_ONLY](../../com.aspose.cells/emfrendersetting\\#EMF-ONLY).

**Returns:**
int
### getEncryptDocumentProperties() {#getEncryptDocumentProperties--}
```
public boolean getEncryptDocumentProperties()
```


Indique si les propriétés du document sont chiffrées lors de l'enregistrement au format .xls. La valeur par défaut est true.

**Remarks**

Uniquement pour les fichiers .xls, .xlsx, .xlsb et .xlsm.

**Returns:**
boolean
### getGridlineColor() {#getGridlineColor--}
```
public Color getGridlineColor()
```


Obtient la couleur des lignes de grille.

**Remarks**

Il ignorera les paramètres de couleur des lignes de grille dans le fichier source.

**Returns:**
[Color](../../com.aspose.cells/color)
### getGridlineType() {#getGridlineType--}
```
public int getGridlineType()
```


Obtient le type des lignes de grille.

Voir [GridlineType](../../com.aspose.cells/gridlinetype).

**Remarks**

La valeur par défaut est le type Pointillé.

**Returns:**
int
### getIgnoreError() {#getIgnoreError--}
```
public boolean getIgnoreError()
```


Indique si vous devez masquer l'erreur lors du rendu. L'erreur peut provenir d'une forme, d'une image, du rendu d'un graphique, etc.

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
### getOnePagePerSheet() {#getOnePagePerSheet--}
```
public boolean getOnePagePerSheet()
```


Si OnePagePerSheet est vrai, tout le contenu d’une feuille sera exporté vers une seule page dans le résultat. La taille du papier de pagesetup sera invalide, et les autres paramètres de pagesetup resteront appliqués.

**Returns:**
boolean
### getOutputBlankPageWhenNothingToPrint() {#getOutputBlankPageWhenNothingToPrint--}
```
public boolean getOutputBlankPageWhenNothingToPrint()
```


Indique s’il faut générer une page blanche lorsqu’il n’y a rien à imprimer.

**Remarks**

La valeur par défaut est true.

**Returns:**
boolean
### getPageCount() {#getPageCount--}
```
public int getPageCount()
```


Obtient le nombre de pages à enregistrer.

**Remarks**

La valeur par défaut est System.Int32.MaxValue, ce qui signifie que toutes les pages seront rendues.

**Example**

L’exemple suivant montre comment rendre une plage de pages (3 et 4) d’un fichier Microsoft Excel en PDF.

```
         //Open an Excel file
         Workbook wb = new Workbook("Book1.xlsx");
 
         PdfSaveOptions options = new PdfSaveOptions();
 
         //Print only Page 3 and Page 4 in the output PDF
         //Starting page index (0-based index)
         options.setPageIndex(3);
         //Number of pages to be printed
         options.setPageCount(2);
 
         //Save the PDF file
         wb.save("output.pdf", options);
```

**Returns:**
int
### getPageIndex() {#getPageIndex--}
```
public int getPageIndex()
```


Obtient l’indice basé sur zéro de la première page à enregistrer.

**Remarks**

La valeur par défaut est 0.

**Example**

L’exemple suivant montre comment rendre une plage de pages (3 et 4) d’un fichier Microsoft Excel en PDF.

```
         //Open an Excel file
         Workbook wb = new Workbook("Book1.xlsx");
 
         PdfSaveOptions options = new PdfSaveOptions();
 
         //Print only Page 3 and Page 4 in the output PDF
         //Starting page index (0-based index)
         options.setPageIndex(3);
         //Number of pages to be printed
         options.setPageCount(2);
 
         //Save the PDF file
         wb.save("output.pdf", options);
```

**Returns:**
int
### getPageSavingCallback() {#getPageSavingCallback--}
```
public IPageSavingCallback getPageSavingCallback()
```


Contrôle/Indique la progression du processus d'enregistrement de la page.

**Returns:**
[IPageSavingCallback](../../com.aspose.cells/ipagesavingcallback)
### getPrintingPageType() {#getPrintingPageType--}
```
public int getPrintingPageType()
```


Indique quelles pages ne seront pas imprimées.

Voir [PrintingPageType](../../com.aspose.cells/printingpagetype).

**Remarks**

Si le contenu de la feuille est clairsemé, certaines pages seront totalement vides dans le fichier PDF de sortie. Si vous ne voulez pas ces pages vides, vous pouvez utiliser cette option pour les omettre.

**Example**

Le code suivant omet les pages vides ou les pages qui ne contiennent que du contenu de style comme le fond de cellule, les bordures.

```
         Workbook wb = new Workbook("Book1.xlsx");
 
         PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
 
         //ignore blank pages
         pdfSaveOptions.setPrintingPageType(PrintingPageType.IGNORE_BLANK);
 
         wb.save("output_ignore_blank_page.pdf", pdfSaveOptions);
 
 
         //ignore blank pages and pages which only contains some style content like cell background
         pdfSaveOptions.setPrintingPageType(PrintingPageType.IGNORE_STYLE);
 
         wb.save("output_ignore_blank_and_style_page.pdf", pdfSaveOptions);
```

**Returns:**
int
### getRefreshChartCache() {#getRefreshChartCache--}
```
public boolean getRefreshChartCache()
```


Indique s'il faut mettre en cache les dernières données du graphique.

**Returns:**
boolean
### getRenderingBehavior() {#getRenderingBehavior--}
```
public int getRenderingBehavior()
```


Obtient les comportements de rendu spécifiques à Excel à appliquer.

Voir [ExcelRenderingBehavior](../../com.aspose.cells/excelrenderingbehavior).

**Remarks**

La valeur par défaut est [ExcelRenderingBehavior.ALL](../../com.aspose.cells/excelrenderingbehavior\\#ALL).

**Returns:**
int
### getSaveAsEditableShapes() {#getSaveAsEditableShapes--}
```
public boolean getSaveAsEditableShapes()
```


Enregistrez tous les objets de dessin en tant que formes modifiables dans le fichier Word, afin de pouvoir les modifier dans Word.

**Remarks**

Uniquement pour les graphiques.

**Returns:**
boolean
### getSaveAsEditableShaps() {#getSaveAsEditableShaps--}
```
public boolean getSaveAsEditableShaps()
```


Enregistrez tous les objets de dessin objecgts en tant que formes modifiables dans le fichier Word. Ainsi, vous pouvez les modifier dans Word.

**Remarks**

NOTE : Ce membre est maintenant obsolète. À la place, veuillez utiliser la propriété [getSaveAsEditableShapes()](../../com.aspose.cells/docxsaveoptions\\#getSaveAsEditableShapes--). Cette propriété sera supprimée 6 mois plus tard à compter de mai 2025. Aspose s’excuse pour tout désagrément que vous avez pu rencontrer.

**Returns:**
boolean
### getSaveElementType() {#getSaveElementType--}
```
public int getSaveElementType()
```


Indique quels éléments doivent être enregistrés.

Voir [SaveElementType](../../com.aspose.cells/saveelementtype).

**Returns:**
int
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


Obtient les feuilles à rendre. La valeur par défaut est toutes les feuilles visibles du classeur : [SheetSet.getVisible()](../../com.aspose.cells/sheetset\#getVisible--).

**Example**

Le code suivant ne rend que la feuille active en PDF.

```
         Workbook workbook = new Workbook("Book1.xlsx");
 
         int activeSheetIndex = workbook.getWorksheets().getActiveSheetIndex();
 
         PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
         //set active sheet index to sheet set.
         pdfSaveOptions.setSheetSet(new SheetSet(new int[] { activeSheetIndex }));
         workbook.save("output.pdf", pdfSaveOptions);
```

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
### getTextCrossType() {#getTextCrossType--}
```
public int getTextCrossType()
```


Obtient le type d'affichage du texte lorsque la largeur du texte est supérieure à la largeur de la cellule.

Voir [TextCrossType](../../com.aspose.cells/textcrosstype).

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
### isFontSubstitutionCharGranularity() {#isFontSubstitutionCharGranularity--}
```
public boolean isFontSubstitutionCharGranularity()
```


Indique s'il faut uniquement substituer la police du caractère lorsque la police de la cellule n'est pas compatible.

**Remarks**

La valeur par défaut est false. Nous essaierons d’abord la police par défaut du classeur et de PdfSaveOption/system pour la police des cellules.

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




### setAllColumnsInOnePagePerSheet(boolean value) {#setAllColumnsInOnePagePerSheet-boolean-}
```
public void setAllColumnsInOnePagePerSheet(boolean value)
```


Si AllColumnsInOnePagePerSheet est vrai, tout le contenu des colonnes d'une feuille sera exporté sur une seule page dans le résultat. La largeur du format de papier du paramètre pagesetup sera ignorée, et les autres paramètres de pagesetup resteront effectifs.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setAsFlatOpc(boolean value) {#setAsFlatOpc-boolean-}
```
public void setAsFlatOpc(boolean value)
```


Indique si l'enregistrement se fait sous forme de fichier OPC plat qui peut être généré par Open XML SDK.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setAsNormalView(boolean value) {#setAsNormalView-boolean-}
```
public void setAsNormalView(boolean value)
```


Exportation du fichier Excel vers un fichier docx en vue normale. Si cette propriété est true, une zone sera générée, et aucune échelle ne sera appliquée. La valeur par défaut est false.

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

### setCheckFontCompatibility(boolean value) {#setCheckFontCompatibility-boolean-}
```
public void setCheckFontCompatibility(boolean value)
```


Indique s’il faut vérifier la compatibilité des polices pour chaque caractère du texte.

**Remarks**

La valeur par défaut est true. Désactiver cette propriété peut améliorer les performances. Mais lorsque la police par défaut ou spécifiée du texte/caractère ne peut pas être utilisée pour le rendre, des caractères illisibles (comme des blocs) peuvent apparaître dans le PDF généré. Dans ce cas, l'utilisateur doit laisser cette propriété à true afin qu'une police alternative soit recherchée et utilisée pour rendre le texte à la place ;

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setCheckWorkbookDefaultFont(boolean value) {#setCheckWorkbookDefaultFont-boolean-}
```
public void setCheckWorkbookDefaultFont(boolean value)
```


Lorsque les caractères dans Excel sont Unicode et ne sont pas définis avec la police correcte dans le style de cellule, ils peuvent apparaître sous forme de blocs dans le PDF ou l'image. Réglez ceci sur true pour essayer d'utiliser la police par défaut du classeur afin d'afficher d'abord ces caractères.

**Remarks**

La valeur par défaut est true.

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

### setCustomRenderSettings(CustomRenderSettings value) {#setCustomRenderSettings-com.aspose.cells.CustomRenderSettings-}
```
public void setCustomRenderSettings(CustomRenderSettings value)
```


Définit les paramètres personnalisés pendant le rendu.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | [CustomRenderSettings](../../com.aspose.cells/customrendersettings) |  |

### setDefaultEditLanguage(int value) {#setDefaultEditLanguage-int-}
```
public void setDefaultEditLanguage(int value)
```


Définit la langue d'édition par défaut.

Voir [DefaultEditLanguage](../../com.aspose.cells/defaulteditlanguage).

**Remarks**

Il peut afficher/rendre différentes mises en page pour le paragraphe de texte lorsque différentes langues d'édition sont définies. La valeur par défaut est [DefaultEditLanguage.AUTO](../../com.aspose.cells/defaulteditlanguage\\#AUTO).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setDefaultFont(String value) {#setDefaultFont-java.lang.String-}
```
public void setDefaultFont(String value)
```


Lorsque les caractères dans Excel sont Unicode et ne sont pas définis avec la police correcte dans le style de cellule, ils peuvent apparaître sous forme de blocs dans le PDF ou l'image. Définissez la police par défaut (DefaultFont) comme MingLiu ou MS Gothic pour afficher ces caractères. Si cette propriété n'est pas définie, Aspose.Cells utilisera la police système par défaut pour afficher ces caractères Unicode.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

### setDrawObjectEventHandler(DrawObjectEventHandler value) {#setDrawObjectEventHandler-com.aspose.cells.DrawObjectEventHandler-}
```
public void setDrawObjectEventHandler(DrawObjectEventHandler value)
```


Implémentez cette interface pour obtenir DrawObject et Bound lors du rendu.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | [DrawObjectEventHandler](../../com.aspose.cells/drawobjecteventhandler) |  |

### setEmbedXlsxAsChartDataSource(boolean value) {#setEmbedXlsxAsChartDataSource-boolean-}
```
public void setEmbedXlsxAsChartDataSource(boolean value)
```


Indique si l'intégration d'un fichier xlsx comme source de données du graphique.

**Remarks**

La valeur par défaut est true.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setEmfRenderSetting(int value) {#setEmfRenderSetting-int-}
```
public void setEmfRenderSetting(int value)
```


Paramètre pour le rendu du métafichier Emf.

Voir [EmfRenderSetting](../../com.aspose.cells/emfrendersetting).

**Remarks**

Les métafichiers EMF identifiés comme "EMF+ Dual" peuvent contenir à la fois des enregistrements EMF+ et des enregistrements EMF. Chaque type d'enregistrement peut être utilisé pour rendre l'image, uniquement les enregistrements EMF+, ou uniquement les enregistrements EMF. Lorsque [EmfRenderSetting.EMF\\_PLUS\\_PREFER](../../com.aspose.cells/emfrendersetting\\#EMF-PLUS-PREFER) est défini, les enregistrements EMF+ seront analysés lors du rendu de la page, sinon seuls les enregistrements EMF seront analysés. La valeur par défaut est [EmfRenderSetting.EMF\\_ONLY](../../com.aspose.cells/emfrendersetting\\#EMF-ONLY).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

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

### setFontSubstitutionCharGranularity(boolean value) {#setFontSubstitutionCharGranularity-boolean-}
```
public void setFontSubstitutionCharGranularity(boolean value)
```


Indique s'il faut uniquement substituer la police du caractère lorsque la police de la cellule n'est pas compatible.

**Remarks**

La valeur par défaut est false. Nous essaierons d’abord la police par défaut du classeur et de PdfSaveOption/system pour la police des cellules.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setGridlineColor(Color value) {#setGridlineColor-com.aspose.cells.Color-}
```
public void setGridlineColor(Color value)
```


Définit la couleur des lignes de grille.

**Remarks**

Il ignorera les paramètres de couleur des lignes de grille dans le fichier source.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | [Color](../../com.aspose.cells/color) |  |

### setGridlineType(int value) {#setGridlineType-int-}
```
public void setGridlineType(int value)
```


Définit le type de ligne de grille.

Voir [GridlineType](../../com.aspose.cells/gridlinetype).

**Remarks**

La valeur par défaut est le type Pointillé.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setIgnoreError(boolean value) {#setIgnoreError-boolean-}
```
public void setIgnoreError(boolean value)
```


Indique si vous devez masquer l'erreur lors du rendu. L'erreur peut provenir d'une forme, d'une image, du rendu d'un graphique, etc.

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

### setOnePagePerSheet(boolean value) {#setOnePagePerSheet-boolean-}
```
public void setOnePagePerSheet(boolean value)
```


Si OnePagePerSheet est vrai, tout le contenu d’une feuille sera exporté vers une seule page dans le résultat. La taille du papier de pagesetup sera invalide, et les autres paramètres de pagesetup resteront appliqués.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setOutputBlankPageWhenNothingToPrint(boolean value) {#setOutputBlankPageWhenNothingToPrint-boolean-}
```
public void setOutputBlankPageWhenNothingToPrint(boolean value)
```


Indique s’il faut générer une page blanche lorsqu’il n’y a rien à imprimer.

**Remarks**

La valeur par défaut est true.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setPageCount(int value) {#setPageCount-int-}
```
public void setPageCount(int value)
```


Définit le nombre de pages à enregistrer.

**Remarks**

La valeur par défaut est System.Int32.MaxValue, ce qui signifie que toutes les pages seront rendues.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setPageIndex(int value) {#setPageIndex-int-}
```
public void setPageIndex(int value)
```


Définit l'index de base zéro de la première page à enregistrer.

**Remarks**

La valeur par défaut est 0.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setPageSavingCallback(IPageSavingCallback value) {#setPageSavingCallback-com.aspose.cells.IPageSavingCallback-}
```
public void setPageSavingCallback(IPageSavingCallback value)
```


Contrôle/Indique la progression du processus d'enregistrement de la page.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | [IPageSavingCallback](../../com.aspose.cells/ipagesavingcallback) |  |

### setPrintingPageType(int value) {#setPrintingPageType-int-}
```
public void setPrintingPageType(int value)
```


Indique quelles pages ne seront pas imprimées.

Voir [PrintingPageType](../../com.aspose.cells/printingpagetype).

**Remarks**

Si le contenu de la feuille est clairsemé, certaines pages seront totalement vides dans le fichier PDF de sortie. Si vous ne voulez pas ces pages vides, vous pouvez utiliser cette option pour les omettre.

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

### setRenderingBehavior(int value) {#setRenderingBehavior-int-}
```
public void setRenderingBehavior(int value)
```


Définit les comportements de rendu spécifiques à Excel à appliquer.

Voir [ExcelRenderingBehavior](../../com.aspose.cells/excelrenderingbehavior).

**Remarks**

La valeur par défaut est [ExcelRenderingBehavior.ALL](../../com.aspose.cells/excelrenderingbehavior\\#ALL).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setSaveAsEditableShapes(boolean value) {#setSaveAsEditableShapes-boolean-}
```
public void setSaveAsEditableShapes(boolean value)
```


Enregistrez tous les objets de dessin en tant que formes modifiables dans le fichier Word, afin de pouvoir les modifier dans Word.

**Remarks**

Uniquement pour les graphiques.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setSaveAsEditableShaps(boolean value) {#setSaveAsEditableShaps-boolean-}
```
public void setSaveAsEditableShaps(boolean value)
```


Enregistrez tous les objets de dessin objecgts en tant que formes modifiables dans le fichier Word. Ainsi, vous pouvez les modifier dans Word.

**Remarks**

NOTE : Ce membre est maintenant obsolète. À la place, veuillez utiliser la propriété [getSaveAsEditableShapes()](../../com.aspose.cells/docxsaveoptions\\#getSaveAsEditableShapes--). Cette propriété sera supprimée 6 mois plus tard à compter de mai 2025. Aspose s’excuse pour tout désagrément que vous avez pu rencontrer.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setSaveElementType(int value) {#setSaveElementType-int-}
```
public void setSaveElementType(int value)
```


Indique quels éléments doivent être enregistrés.

Voir [SaveElementType](../../com.aspose.cells/saveelementtype).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setSheetSet(SheetSet value) {#setSheetSet-com.aspose.cells.SheetSet-}
```
public void setSheetSet(SheetSet value)
```


Définit les feuilles à rendre. La valeur par défaut est toutes les feuilles visibles du classeur : [SheetSet.getVisible()](../../com.aspose.cells/sheetset\#getVisible--).

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

### setTextCrossType(int value) {#setTextCrossType-int-}
```
public void setTextCrossType(int value)
```


Définit le type d'affichage du texte lorsque la largeur du texte est supérieure à la largeur de la cellule.

Voir [TextCrossType](../../com.aspose.cells/textcrosstype).

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

