---
title: "PdfSaveOptions"
second_title: "Référence API d'Aspose.Cells pour Java"
description: "Représente les options d'enregistrement du fichier PDF."
type: docs
url: /fr/java/com.aspose.cells/pdfsaveoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.SaveOptions](../../com.aspose.cells/saveoptions), [com.aspose.cells.PaginatedSaveOptions](../../com.aspose.cells/paginatedsaveoptions)
```
public class PdfSaveOptions extends PaginatedSaveOptions
```

Représente les options d'enregistrement du fichier PDF.
## Constructeurs

| Constructeur | Description |
| --- | --- |
| [PdfSaveOptions()](#PdfSaveOptions--) | Crée les options pour enregistrer le fichier PDF. |
## Méthodes

| Méthode | Description |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAllColumnsInOnePagePerSheet()](#getAllColumnsInOnePagePerSheet--) | Si AllColumnsInOnePagePerSheet est true, tout le contenu des colonnes d’une feuille sera généré sur une seule page dans le résultat. |
| [getBookmark()](#getBookmark--) | Obtient l’objet [PdfBookmarkEntry](../../com.aspose.cells/pdfbookmarkentry). |
| [getCachedFileFolder()](#getCachedFileFolder--) | Le dossier pour les fichiers temporaires pouvant être utilisés comme cache de données. |
| [getCalculateFormula()](#getCalculateFormula--) | Indique si les formules doivent être calculées avant d'enregistrer le fichier pdf. |
| [getCheckExcelRestriction()](#getCheckExcelRestriction--) | Indique si la vérification des restrictions du fichier Excel est effectuée lorsque l'utilisateur modifie les objets liés aux cellules. |
| [getCheckFontCompatibility()](#getCheckFontCompatibility--) | Indique s’il faut vérifier la compatibilité des polices pour chaque caractère du texte. |
| [getCheckWorkbookDefaultFont()](#getCheckWorkbookDefaultFont--) | Lorsque les caractères dans Excel sont Unicode et ne sont pas définis avec la police correcte dans le style de cellule, ils peuvent apparaître sous forme de blocs dans le pdf, l’image. |
| [getClass()](#getClass--) |  |
| [getClearData()](#getClearData--) | Rendre le classeur vide après l'enregistrement du fichier. |
| [getCompliance()](#getCompliance--) | Obtient le niveau de conformité aux normes PDF pour les documents de sortie. |
| [getCreateDirectory()](#getCreateDirectory--) | Si vrai et que le répertoire n'existe pas, le répertoire sera créé automatiquement avant d'enregistrer le fichier. |
| [getCreatedTime()](#getCreatedTime--) | Obtient l'heure de génération du document pdf. |
| [getCustomPropertiesExport()](#getCustomPropertiesExport--) | Obtient une valeur déterminant la façon dont [CustomDocumentPropertyCollection](../../com.aspose.cells/customdocumentpropertycollection) sont exportées vers le fichier PDF. |
| [getCustomRenderSettings()](#getCustomRenderSettings--) | Obtient les paramètres personnalisés pendant le rendu. |
| [getDefaultEditLanguage()](#getDefaultEditLanguage--) | Obtient la langue d’édition par défaut. |
| [getDefaultFont()](#getDefaultFont--) | Lorsque les caractères dans Excel sont Unicode et ne sont pas définis avec la police correcte dans le style de cellule, ils peuvent apparaître sous forme de blocs dans le pdf, l’image. |
| [getDisplayDocTitle()](#getDisplayDocTitle--) | Indique si la barre de titre de la fenêtre doit afficher le titre du document. |
| [getDrawObjectEventHandler()](#getDrawObjectEventHandler--) | Implémentez cette interface pour obtenir DrawObject et Bound lors du rendu. |
| [getEmbedAttachments()](#getEmbedAttachments--) | Indique s'il faut incorporer une pièce jointe pour les objets Ole dans Excel. |
| [getEmbedStandardWindowsFonts()](#getEmbedStandardWindowsFonts--) | Vrai pour incorporer les polices TrueType. |
| [getEmfRenderSetting()](#getEmfRenderSetting--) | Paramètre pour le rendu du métafichier Emf. |
| [getEncryptDocumentProperties()](#getEncryptDocumentProperties--) | Indique s'il faut chiffrer les propriétés du document lors de l'enregistrement au format .xls. |
| [getExportDocumentStructure()](#getExportDocumentStructure--) | Indique s'il faut exporter la structure du document. |
| [getFontEncoding()](#getFontEncoding--) | Obtient l'encodage des polices incorporées dans le pdf. |
| [getGridlineColor()](#getGridlineColor--) | Obtient la couleur des lignes de grille. |
| [getGridlineType()](#getGridlineType--) | Obtient le type des lignes de grille. |
| [getIgnoreError()](#getIgnoreError--) | Indique si vous devez masquer l’erreur lors du rendu. |
| [getImageType()](#getImageType--) | Représente le type d'image lors de la conversion du graphique et de la forme. |
| [getMergeAreas()](#getMergeAreas--) | Indique s'il faut fusionner les zones de mise en forme conditionnelle et de validation avant d'enregistrer le fichier. |
| [getOnePagePerSheet()](#getOnePagePerSheet--) | Si OnePagePerSheet est true, tout le contenu d’une feuille sera généré sur une seule page dans le résultat. |
| [getOptimizationType()](#getOptimizationType--) | Obtient le type d'optimisation du pdf. |
| [getOutputBlankPageWhenNothingToPrint()](#getOutputBlankPageWhenNothingToPrint--) | Indique s’il faut générer une page blanche lorsqu’il n’y a rien à imprimer. |
| [getPageCount()](#getPageCount--) | Obtient le nombre de pages à enregistrer. |
| [getPageIndex()](#getPageIndex--) | Obtient l’indice basé sur zéro de la première page à enregistrer. |
| [getPageSavingCallback()](#getPageSavingCallback--) | Contrôle/Indique la progression du processus d'enregistrement de la page. |
| [getPdfCompression()](#getPdfCompression--) | Indique l'algorithme de compression |
| [getPrintingPageType()](#getPrintingPageType--) | Indique quelles pages ne seront pas imprimées. |
| [getProducer()](#getProducer--) | Obtient le producteur du document pdf généré. |
| [getRefreshChartCache()](#getRefreshChartCache--) | Indique s'il faut mettre en cache les dernières données du graphique. |
| [getRenderingBehavior()](#getRenderingBehavior--) | Obtient les comportements de rendu spécifiques à Excel à appliquer. |
| [getSaveFormat()](#getSaveFormat--) | Obtient le format de fichier d'enregistrement. |
| [getSecurityOptions()](#getSecurityOptions--) | Définissez ces options lorsque la sécurité est requise dans le résultat xls2pdf. |
| [getSheetSet()](#getSheetSet--) | Obtient les feuilles à rendre. |
| [getSortExternalNames()](#getSortExternalNames--) | Indique s'il faut trier les noms définis externes avant d'enregistrer le fichier. |
| [getSortNames()](#getSortNames--) | Indique s'il faut trier les noms définis avant d'enregistrer le fichier. |
| [getTextCrossType()](#getTextCrossType--) | Obtient le type d'affichage du texte lorsque la largeur du texte est supérieure à la largeur de la cellule. |
| [getUpdateSmartArt()](#getUpdateSmartArt--) | Indique s'il faut mettre à jour le paramètre SmartArt. |
| [getValidateMergedAreas()](#getValidateMergedAreas--) | Indique s'il faut valider les cellules fusionnées avant d'enregistrer le fichier. |
| [getWarningCallback()](#getWarningCallback--) | Obtient le rappel d'avertissement. |
| [getWatermark()](#getWatermark--) | Obtient le filigrane à produire. |
| [getZoomBehavior()](#getZoomBehavior--) | Obtient le mode d'affichage initial lorsque le document PDF généré est ouvert. |
| [getZoomFactor()](#getZoomFactor--) | Obtient le pourcentage de zoom utilisé lorsque [getZoomBehavior()](../../com.aspose.cells/pdfsaveoptions\#getZoomBehavior--) est [PdfZoomBehavior.ZOOM\_FACTOR](../../com.aspose.cells/pdfzoombehavior\#ZOOM-FACTOR). |
| [hashCode()](#hashCode--) |  |
| [isFontSubstitutionCharGranularity()](#isFontSubstitutionCharGranularity--) | Indique s'il faut uniquement substituer la police du caractère lorsque la police de la cellule n'est pas compatible. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAllColumnsInOnePagePerSheet(boolean value)](#setAllColumnsInOnePagePerSheet-boolean-) | Si AllColumnsInOnePagePerSheet est true, tout le contenu des colonnes d’une feuille sera généré sur une seule page dans le résultat. |
| [setBookmark(PdfBookmarkEntry value)](#setBookmark-com.aspose.cells.PdfBookmarkEntry-) | Définit l'objet [PdfBookmarkEntry](../../com.aspose.cells/pdfbookmarkentry). |
| [setCachedFileFolder(String value)](#setCachedFileFolder-java.lang.String-) | Le dossier pour les fichiers temporaires pouvant être utilisés comme cache de données. |
| [setCalculateFormula(boolean value)](#setCalculateFormula-boolean-) | Indique si les formules doivent être calculées avant d'enregistrer le fichier pdf. |
| [setCheckExcelRestriction(boolean value)](#setCheckExcelRestriction-boolean-) | Indique si la vérification des restrictions du fichier Excel est effectuée lorsque l'utilisateur modifie les objets liés aux cellules. |
| [setCheckFontCompatibility(boolean value)](#setCheckFontCompatibility-boolean-) | Indique s’il faut vérifier la compatibilité des polices pour chaque caractère du texte. |
| [setCheckWorkbookDefaultFont(boolean value)](#setCheckWorkbookDefaultFont-boolean-) | Lorsque les caractères dans Excel sont Unicode et ne sont pas définis avec la police correcte dans le style de cellule, ils peuvent apparaître sous forme de blocs dans le pdf, l’image. |
| [setClearData(boolean value)](#setClearData-boolean-) | Rendre le classeur vide après l'enregistrement du fichier. |
| [setCompliance(int value)](#setCompliance-int-) | Définit le niveau de conformité aux normes PDF pour les documents de sortie. |
| [setCreateDirectory(boolean value)](#setCreateDirectory-boolean-) | Si vrai et que le répertoire n'existe pas, le répertoire sera créé automatiquement avant d'enregistrer le fichier. |
| [setCreatedTime(DateTime value)](#setCreatedTime-com.aspose.cells.DateTime-) | Définit l'heure de génération du document pdf. |
| [setCustomPropertiesExport(int value)](#setCustomPropertiesExport-int-) | Définit une valeur déterminant la façon dont [CustomDocumentPropertyCollection](../../com.aspose.cells/customdocumentpropertycollection) sont exportées vers le fichier PDF. |
| [setCustomRenderSettings(CustomRenderSettings value)](#setCustomRenderSettings-com.aspose.cells.CustomRenderSettings-) | Définit les paramètres personnalisés pendant le rendu. |
| [setDefaultEditLanguage(int value)](#setDefaultEditLanguage-int-) | Définit la langue d'édition par défaut. |
| [setDefaultFont(String value)](#setDefaultFont-java.lang.String-) | Lorsque les caractères dans Excel sont Unicode et ne sont pas définis avec la police correcte dans le style de cellule, ils peuvent apparaître sous forme de blocs dans le pdf, l’image. |
| [setDisplayDocTitle(boolean value)](#setDisplayDocTitle-boolean-) | Indique si la barre de titre de la fenêtre doit afficher le titre du document. |
| [setDrawObjectEventHandler(DrawObjectEventHandler value)](#setDrawObjectEventHandler-com.aspose.cells.DrawObjectEventHandler-) | Implémentez cette interface pour obtenir DrawObject et Bound lors du rendu. |
| [setEmbedAttachments(boolean value)](#setEmbedAttachments-boolean-) | Indique s'il faut incorporer une pièce jointe pour les objets Ole dans Excel. |
| [setEmbedStandardWindowsFonts(boolean value)](#setEmbedStandardWindowsFonts-boolean-) | Vrai pour incorporer les polices TrueType. |
| [setEmfRenderSetting(int value)](#setEmfRenderSetting-int-) | Paramètre pour le rendu du métafichier Emf. |
| [setEncryptDocumentProperties(boolean value)](#setEncryptDocumentProperties-boolean-) | Indique s'il faut chiffrer les propriétés du document lors de l'enregistrement au format .xls. |
| [setExportDocumentStructure(boolean value)](#setExportDocumentStructure-boolean-) | Indique s'il faut exporter la structure du document. |
| [setFontEncoding(int value)](#setFontEncoding-int-) | Définit l'encodage des polices incorporées dans le pdf. |
| [setFontSubstitutionCharGranularity(boolean value)](#setFontSubstitutionCharGranularity-boolean-) | Indique s'il faut uniquement substituer la police du caractère lorsque la police de la cellule n'est pas compatible. |
| [setGridlineColor(Color value)](#setGridlineColor-com.aspose.cells.Color-) | Définit la couleur des lignes de grille. |
| [setGridlineType(int value)](#setGridlineType-int-) | Définit le type de ligne de grille. |
| [setIgnoreError(boolean value)](#setIgnoreError-boolean-) | Indique si vous devez masquer l’erreur lors du rendu. |
| [setImageResample(int desiredPPI, int jpegQuality)](#setImageResample-int-int-) | Définit le PPI (pixels par pouce) souhaité pour le rééchantillonnage des images et la qualité jpeg. |
| [setImageType(ImageFormat value)](#setImageType-com.aspose.cells.ImageFormat-) | Représente le type d'image lors de la conversion du graphique et de la forme. |
| [setMergeAreas(boolean value)](#setMergeAreas-boolean-) | Indique s'il faut fusionner les zones de mise en forme conditionnelle et de validation avant d'enregistrer le fichier. |
| [setOnePagePerSheet(boolean value)](#setOnePagePerSheet-boolean-) | Si OnePagePerSheet est true, tout le contenu d’une feuille sera généré sur une seule page dans le résultat. |
| [setOptimizationType(int value)](#setOptimizationType-int-) | Définit le type d'optimisation du pdf. |
| [setOutputBlankPageWhenNothingToPrint(boolean value)](#setOutputBlankPageWhenNothingToPrint-boolean-) | Indique s’il faut générer une page blanche lorsqu’il n’y a rien à imprimer. |
| [setPageCount(int value)](#setPageCount-int-) | Définit le nombre de pages à enregistrer. |
| [setPageIndex(int value)](#setPageIndex-int-) | Définit l'index de base zéro de la première page à enregistrer. |
| [setPageSavingCallback(IPageSavingCallback value)](#setPageSavingCallback-com.aspose.cells.IPageSavingCallback-) | Contrôle/Indique la progression du processus d'enregistrement de la page. |
| [setPdfCompression(int value)](#setPdfCompression-int-) | Indique l'algorithme de compression |
| [setPrintingPageType(int value)](#setPrintingPageType-int-) | Indique quelles pages ne seront pas imprimées. |
| [setProducer(String value)](#setProducer-java.lang.String-) | Définit le producteur du document pdf généré. |
| [setRefreshChartCache(boolean value)](#setRefreshChartCache-boolean-) | Indique s'il faut mettre en cache les dernières données du graphique. |
| [setRenderingBehavior(int value)](#setRenderingBehavior-int-) | Définit les comportements de rendu spécifiques à Excel à appliquer. |
| [setSecurityOptions(PdfSecurityOptions value)](#setSecurityOptions-com.aspose.cells.PdfSecurityOptions-) | Définissez ces options lorsque la sécurité est requise dans le résultat xls2pdf. |
| [setSheetSet(SheetSet value)](#setSheetSet-com.aspose.cells.SheetSet-) | Définit les feuilles à rendre. |
| [setSortExternalNames(boolean value)](#setSortExternalNames-boolean-) | Indique s'il faut trier les noms définis externes avant d'enregistrer le fichier. |
| [setSortNames(boolean value)](#setSortNames-boolean-) | Indique s'il faut trier les noms définis avant d'enregistrer le fichier. |
| [setTextCrossType(int value)](#setTextCrossType-int-) | Définit le type d'affichage du texte lorsque la largeur du texte est supérieure à la largeur de la cellule. |
| [setUpdateSmartArt(boolean value)](#setUpdateSmartArt-boolean-) | Indique s'il faut mettre à jour le paramètre SmartArt. |
| [setValidateMergedAreas(boolean value)](#setValidateMergedAreas-boolean-) | Indique s'il faut valider les cellules fusionnées avant d'enregistrer le fichier. |
| [setWarningCallback(IWarningCallback value)](#setWarningCallback-com.aspose.cells.IWarningCallback-) | Définit le rappel d’avertissement. |
| [setWatermark(RenderingWatermark value)](#setWatermark-com.aspose.cells.RenderingWatermark-) | Définit le filigrane dans la sortie. |
| [setZoomBehavior(int value)](#setZoomBehavior-int-) | Définit le mode d'affichage initial lorsque le document PDF généré est ouvert. |
| [setZoomFactor(int value)](#setZoomFactor-int-) | Définit le pourcentage de zoom utilisé lorsque [getZoomBehavior()](../../com.aspose.cells/pdfsaveoptions\#getZoomBehavior--) est [PdfZoomBehavior.ZOOM\_FACTOR](../../com.aspose.cells/pdfzoombehavior\#ZOOM-FACTOR). |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### PdfSaveOptions() {#PdfSaveOptions--}
```
public PdfSaveOptions()
```


Crée les options pour enregistrer le fichier PDF.

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
### getBookmark() {#getBookmark--}
```
public PdfBookmarkEntry getBookmark()
```


Obtient l’objet [PdfBookmarkEntry](../../com.aspose.cells/pdfbookmarkentry).

**Returns:**
[PdfBookmarkEntry](../../com.aspose.cells/pdfbookmarkentry)
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


Indique si les formules doivent être calculées avant d'enregistrer le fichier pdf.

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
### getCompliance() {#getCompliance--}
```
public int getCompliance()
```


Obtient le niveau de conformité aux normes PDF pour les documents de sortie.

Voir [PdfCompliance](../../com.aspose.cells/pdfcompliance).

**Remarks**

La valeur par défaut est Pdf17.

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
### getCreatedTime() {#getCreatedTime--}
```
public DateTime getCreatedTime()
```


Obtient l'heure de génération du document pdf.

**Remarks**

si elle n'est pas définie, ce sera le moment de la génération du PDF.

**Returns:**
[DateTime](../../com.aspose.cells/datetime)
### getCustomPropertiesExport() {#getCustomPropertiesExport--}
```
public int getCustomPropertiesExport()
```


Obtient une valeur déterminant la façon dont [CustomDocumentPropertyCollection](../../com.aspose.cells/customdocumentpropertycollection) sont exportées vers le fichier PDF. La valeur par défaut est None.

Voir [PdfCustomPropertiesExport](../../com.aspose.cells/pdfcustompropertiesexport).

**Returns:**
int
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
### getDisplayDocTitle() {#getDisplayDocTitle--}
```
public boolean getDisplayDocTitle()
```


Indique si la barre de titre de la fenêtre doit afficher le titre du document.

**Remarks**

Si false, la barre de titre doit afficher le nom du fichier PDF à la place. La valeur par défaut est false.

**Returns:**
boolean
### getDrawObjectEventHandler() {#getDrawObjectEventHandler--}
```
public DrawObjectEventHandler getDrawObjectEventHandler()
```


Implémentez cette interface pour obtenir DrawObject et Bound lors du rendu.

**Returns:**
[DrawObjectEventHandler](../../com.aspose.cells/drawobjecteventhandler)
### getEmbedAttachments() {#getEmbedAttachments--}
```
public boolean getEmbedAttachments()
```


Indique s'il faut incorporer une pièce jointe pour les objets Ole dans Excel.

**Remarks**

La valeur par défaut est false. La valeur doit être false lorsque la conformité PDF/A est définie ou que le chiffrement PDF est activé.

**Returns:**
boolean
### getEmbedStandardWindowsFonts() {#getEmbedStandardWindowsFonts--}
```
public boolean getEmbedStandardWindowsFonts()
```


True pour incorporer les polices TrueType. N'affecte que les caractères ASCII 32-127. Les polices pour les codes de caractères supérieurs à 127 sont toujours incorporées. Les polices sont toujours incorporées pour les standards PDF/A-1a, PDF/A-1b. La valeur par défaut est true.

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
### getExportDocumentStructure() {#getExportDocumentStructure--}
```
public boolean getExportDocumentStructure()
```


Indique s'il faut exporter la structure du document.

**Returns:**
boolean
### getFontEncoding() {#getFontEncoding--}
```
public int getFontEncoding()
```


Obtient l'encodage des polices incorporées dans le pdf.

Voir [PdfFontEncoding](../../com.aspose.cells/pdffontencoding).

**Remarks**

La valeur par défaut est [PdfFontEncoding.IDENTITY](../../com.aspose.cells/pdffontencoding\#IDENTITY)

**Returns:**
int
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
### getImageType() {#getImageType--}
```
public ImageFormat getImageType()
```


Représente le type d'image lors de la conversion du graphique et de la forme.

**Remarks**

NOTE : Ce membre est maintenant obsolète. À la place, Chart et Shape sont toujours rendus comme des éléments vectoriels (par ex. point, ligne) pour la qualité du rendu. Cette propriété sera supprimée 12 mois après juin 2022. Aspose s’excuse pour tout désagrément que vous auriez pu rencontrer.

**Returns:**
[ImageFormat](../../com.aspose.cells/imageformat)
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
### getOptimizationType() {#getOptimizationType--}
```
public int getOptimizationType()
```


Obtient le type d'optimisation du pdf.

Voir [PdfOptimizationType](../../com.aspose.cells/pdfoptimizationtype).

**Remarks**

La valeur par défaut est [PdfOptimizationType.STANDARD](../../com.aspose.cells/pdfoptimizationtype\#STANDARD)

**Returns:**
int
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
### getPdfCompression() {#getPdfCompression--}
```
public int getPdfCompression()
```


Indique l'algorithme de compression

Voir [PdfCompressionCore](../../com.aspose.cells/pdfcompressioncore).

**Returns:**
int
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
### getProducer() {#getProducer--}
```
public String getProducer()
```


Obtient le producteur du document pdf généré.

**Remarks**

Si la valeur est null, ou qu'une LICENSE valide n'est pas définie, la chaîne Aspose.Cells vVERSION sera utilisée.

**Returns:**
java.lang.String
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
### getSaveFormat() {#getSaveFormat--}
```
public int getSaveFormat()
```


Obtient le format de fichier d'enregistrement.

Voir [SaveFormat](../../com.aspose.cells/saveformat).

**Returns:**
int
### getSecurityOptions() {#getSecurityOptions--}
```
public PdfSecurityOptions getSecurityOptions()
```


Définissez ces options lorsque la sécurité est requise dans le résultat xls2pdf.

**Example**

Le code suivant définit la permission d'impression de résolution de hauteur pour le PDF de sortie.

```
         Workbook wb = new Workbook();
         wb.getWorksheets().get(0).getCells().get("A1").setValue("Aspose");
 
         PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
 
 
         PdfSecurityOptions pdfSecurityOptions = new PdfSecurityOptions();
 
         //set owner password
         pdfSecurityOptions.setOwnerPassword("YourOwnerPassword");
 
         //set user password
         pdfSecurityOptions.setUserPassword("YourUserPassword");
 
         //set print permisson
         pdfSecurityOptions.setPrintPermission(true);
 
         //set high resolution for print
         pdfSecurityOptions.setFullQualityPrintPermission(true);
 
 
         pdfSaveOptions.setSecurityOptions(pdfSecurityOptions);
 
         wb.save("output.pdf", pdfSaveOptions);
```

**Returns:**
[PdfSecurityOptions](../../com.aspose.cells/pdfsecurityoptions)
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
### getWatermark() {#getWatermark--}
```
public RenderingWatermark getWatermark()
```


Obtient le filigrane à produire.

**Example**

Le code suivant définit le filigrane dans le PDF de sortie.

```
         //prepare a workbook with 3 pages.
         Workbook wb = new Workbook();
         wb.getWorksheets().get(0).getCells().get("A1").putValue("Page1");
         int index = wb.getWorksheets().add();
         wb.getWorksheets().get(index).getCells().get("A1").putValue("Page2");
         index = wb.getWorksheets().add();
         wb.getWorksheets().get(index).getCells().get("A1").putValue("Page3");
         wb.getWorksheets().get(index).getPageSetup().setPaperSize(PaperSizeType.PAPER_A_3);
 
         //create a font for watermark, and specify bold, italic, color
         RenderingFont font = new RenderingFont("Calibri", 68);
         font.setItalic(true);
         font.setBold(true);
         font.setColor(Color.getBlue());
 
         //create a watermark from text and the specified font
         RenderingWatermark watermark = new RenderingWatermark("Watermark", font);
 
         //specify horizontal and vertical alignment
         watermark.setHAlignment(TextAlignmentType.CENTER);
         watermark.setVAlignment(TextAlignmentType.CENTER);
 
         //specify rotation
         watermark.setRotation(30);
 
         //specify opacity
         watermark.setOpacity(0.6f);
 
         //specify the scale to page(e.g. 100, 50) in percent.
         watermark.setScaleToPagePercent(50);
 
         //spcify watermark for rendering to pdf.
         PdfSaveOptions options = new PdfSaveOptions();
         options.setWatermark(watermark);
 
         wb.save("output_watermark.pdf", options);
```

**Returns:**
[RenderingWatermark](../../com.aspose.cells/renderingwatermark)
### getZoomBehavior() {#getZoomBehavior--}
```
public int getZoomBehavior()
```


Obtient le mode d'affichage initial lorsque le document PDF généré est ouvert. La valeur par défaut est [PdfZoomBehavior.NONE](../../com.aspose.cells/pdfzoombehavior\#NONE).

Voir [PdfZoomBehavior](../../com.aspose.cells/pdfzoombehavior).

**Returns:**
int
### getZoomFactor() {#getZoomFactor--}
```
public int getZoomFactor()
```


Obtient le pourcentage de zoom utilisé lorsque [getZoomBehavior()](../../com.aspose.cells/pdfsaveoptions\#getZoomBehavior--) est [PdfZoomBehavior.ZOOM\_FACTOR](../../com.aspose.cells/pdfzoombehavior\#ZOOM-FACTOR).

**Remarks**

Cette propriété est ignorée sauf si [getZoomBehavior()](../../com.aspose.cells/pdfsaveoptions\#getZoomBehavior--) est [PdfZoomBehavior.ZOOM\_FACTOR](../../com.aspose.cells/pdfzoombehavior\#ZOOM-FACTOR).

**Returns:**
int
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

### setBookmark(PdfBookmarkEntry value) {#setBookmark-com.aspose.cells.PdfBookmarkEntry-}
```
public void setBookmark(PdfBookmarkEntry value)
```


Définit l'objet [PdfBookmarkEntry](../../com.aspose.cells/pdfbookmarkentry).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | [PdfBookmarkEntry](../../com.aspose.cells/pdfbookmarkentry) |  |

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


Indique si les formules doivent être calculées avant d'enregistrer le fichier pdf.

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

### setCompliance(int value) {#setCompliance-int-}
```
public void setCompliance(int value)
```


Définit le niveau de conformité aux normes PDF pour les documents de sortie.

Voir [PdfCompliance](../../com.aspose.cells/pdfcompliance).

**Remarks**

La valeur par défaut est Pdf17.

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

### setCreatedTime(DateTime value) {#setCreatedTime-com.aspose.cells.DateTime-}
```
public void setCreatedTime(DateTime value)
```


Définit l'heure de génération du document pdf.

**Remarks**

si elle n'est pas définie, ce sera le moment de la génération du PDF.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | [DateTime](../../com.aspose.cells/datetime) |  |

### setCustomPropertiesExport(int value) {#setCustomPropertiesExport-int-}
```
public void setCustomPropertiesExport(int value)
```


Définit une valeur déterminant la façon dont [CustomDocumentPropertyCollection](../../com.aspose.cells/customdocumentpropertycollection) sont exportées vers le fichier PDF. La valeur par défaut est None.

Voir [PdfCustomPropertiesExport](../../com.aspose.cells/pdfcustompropertiesexport).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

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

### setDisplayDocTitle(boolean value) {#setDisplayDocTitle-boolean-}
```
public void setDisplayDocTitle(boolean value)
```


Indique si la barre de titre de la fenêtre doit afficher le titre du document.

**Remarks**

Si false, la barre de titre doit afficher le nom du fichier PDF à la place. La valeur par défaut est false.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setDrawObjectEventHandler(DrawObjectEventHandler value) {#setDrawObjectEventHandler-com.aspose.cells.DrawObjectEventHandler-}
```
public void setDrawObjectEventHandler(DrawObjectEventHandler value)
```


Implémentez cette interface pour obtenir DrawObject et Bound lors du rendu.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | [DrawObjectEventHandler](../../com.aspose.cells/drawobjecteventhandler) |  |

### setEmbedAttachments(boolean value) {#setEmbedAttachments-boolean-}
```
public void setEmbedAttachments(boolean value)
```


Indique s'il faut incorporer une pièce jointe pour les objets Ole dans Excel.

**Remarks**

La valeur par défaut est false. La valeur doit être false lorsque la conformité PDF/A est définie ou que le chiffrement PDF est activé.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setEmbedStandardWindowsFonts(boolean value) {#setEmbedStandardWindowsFonts-boolean-}
```
public void setEmbedStandardWindowsFonts(boolean value)
```


True pour incorporer les polices TrueType. N'affecte que les caractères ASCII 32-127. Les polices pour les codes de caractères supérieurs à 127 sont toujours incorporées. Les polices sont toujours incorporées pour les standards PDF/A-1a, PDF/A-1b. La valeur par défaut est true.

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

### setExportDocumentStructure(boolean value) {#setExportDocumentStructure-boolean-}
```
public void setExportDocumentStructure(boolean value)
```


Indique s'il faut exporter la structure du document.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setFontEncoding(int value) {#setFontEncoding-int-}
```
public void setFontEncoding(int value)
```


Définit l'encodage des polices incorporées dans le pdf.

Voir [PdfFontEncoding](../../com.aspose.cells/pdffontencoding).

**Remarks**

La valeur par défaut est [PdfFontEncoding.IDENTITY](../../com.aspose.cells/pdffontencoding\#IDENTITY)

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

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

### setImageResample(int desiredPPI, int jpegQuality) {#setImageResample-int-int-}
```
public void setImageResample(int desiredPPI, int jpegQuality)
```


Définit le PPI (pixels par pouce) souhaité pour le rééchantillonnage des images et la qualité JPEG. Toutes les images seront converties en JPEG avec le paramètre de qualité spécifié, et les images dont le PPI dépasse la valeur spécifiée seront rééchantillonnées.

**Example**

Le code suivant définit le PPI souhaité à 96 et la qualité JPEG à 80 pour les images dans le PDF de sortie.

```
         //load the source file with images.
         Workbook wb = new Workbook("Book1.xlsx");
 
         PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
 
         //set desired PPI as 96 and jpeg quality as 80.
         pdfSaveOptions.setImageResample(96, 80);
 
         wb.save("output.pdf", pdfSaveOptions);
```

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| desiredPPI | int | Pixels par pouce souhaités. 220 haute qualité. 150 qualité d'écran. 96 qualité d'e-mail. |
| jpegQuality | int | Qualité JPEG de 0 à 100 %. |

### setImageType(ImageFormat value) {#setImageType-com.aspose.cells.ImageFormat-}
```
public void setImageType(ImageFormat value)
```


Représente le type d'image lors de la conversion du graphique et de la forme.

**Remarks**

NOTE : Ce membre est maintenant obsolète. À la place, Chart et Shape sont toujours rendus comme des éléments vectoriels (par ex. point, ligne) pour la qualité du rendu. Cette propriété sera supprimée 12 mois après juin 2022. Aspose s’excuse pour tout désagrément que vous auriez pu rencontrer.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | [ImageFormat](../../com.aspose.cells/imageformat) |  |

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

### setOptimizationType(int value) {#setOptimizationType-int-}
```
public void setOptimizationType(int value)
```


Définit le type d'optimisation du pdf.

Voir [PdfOptimizationType](../../com.aspose.cells/pdfoptimizationtype).

**Remarks**

La valeur par défaut est [PdfOptimizationType.STANDARD](../../com.aspose.cells/pdfoptimizationtype\#STANDARD)

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

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

### setPdfCompression(int value) {#setPdfCompression-int-}
```
public void setPdfCompression(int value)
```


Indique l'algorithme de compression

Voir [PdfCompressionCore](../../com.aspose.cells/pdfcompressioncore).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

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

### setProducer(String value) {#setProducer-java.lang.String-}
```
public void setProducer(String value)
```


Définit le producteur du document pdf généré.

**Remarks**

Si la valeur est null, ou qu'une LICENSE valide n'est pas définie, la chaîne Aspose.Cells vVERSION sera utilisée.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

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

### setSecurityOptions(PdfSecurityOptions value) {#setSecurityOptions-com.aspose.cells.PdfSecurityOptions-}
```
public void setSecurityOptions(PdfSecurityOptions value)
```


Définissez ces options lorsque la sécurité est requise dans le résultat xls2pdf.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | [PdfSecurityOptions](../../com.aspose.cells/pdfsecurityoptions) |  |

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

### setWatermark(RenderingWatermark value) {#setWatermark-com.aspose.cells.RenderingWatermark-}
```
public void setWatermark(RenderingWatermark value)
```


Définit le filigrane dans la sortie.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | [RenderingWatermark](../../com.aspose.cells/renderingwatermark) |  |

### setZoomBehavior(int value) {#setZoomBehavior-int-}
```
public void setZoomBehavior(int value)
```


Définit le mode d'affichage initial lorsque le document PDF généré est ouvert. La valeur par défaut est [PdfZoomBehavior.NONE](../../com.aspose.cells/pdfzoombehavior\\#NONE).

Voir [PdfZoomBehavior](../../com.aspose.cells/pdfzoombehavior).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setZoomFactor(int value) {#setZoomFactor-int-}
```
public void setZoomFactor(int value)
```


Définit le pourcentage de zoom utilisé lorsque [getZoomBehavior()](../../com.aspose.cells/pdfsaveoptions\#getZoomBehavior--) est [PdfZoomBehavior.ZOOM\_FACTOR](../../com.aspose.cells/pdfzoombehavior\#ZOOM-FACTOR).

**Remarks**

Cette propriété est ignorée sauf si [getZoomBehavior()](../../com.aspose.cells/pdfsaveoptions\#getZoomBehavior--) est [PdfZoomBehavior.ZOOM\_FACTOR](../../com.aspose.cells/pdfzoombehavior\#ZOOM-FACTOR).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

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

