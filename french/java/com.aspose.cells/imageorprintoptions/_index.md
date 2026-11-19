---
title: "ImageOrPrintOptions"
second_title: "Référence API d'Aspose.Cells pour Java"
description: "Permet de spécifier les options lors du rendu d'une feuille de calcul en images, de l'impression de la feuille de calcul ou du rendu d'un graphique en image."
type: docs
url: /fr/java/com.aspose.cells/imageorprintoptions/
---

**Inheritance:**
java.lang.Object
```
public class ImageOrPrintOptions
```

Permet de spécifier des options lors du rendu d'une feuille de calcul en images, de l'impression de la feuille ou du rendu d'un graphique en image.

**Example**

```
         //Set Image Or Print Options
         ImageOrPrintOptions options = new ImageOrPrintOptions();
 
         //Set output image format
         options.setImageType(ImageType.PNG);
 
         //Set Horizontal resolution
         options.setHorizontalResolution(300);
 
         //Set Vertical Resolution
         options.setVerticalResolution(300);
 
         //Instantiate Workbook
         Workbook book = new Workbook("test.xls");
 
         //Save chart as Image using ImageOrPrint Options
         book.getWorksheets().get(0).getCharts().get(0).toImage("chart.png", options);
```
## Constructeurs

| Constructeur | Description |
| --- | --- |
| [ImageOrPrintOptions()](#ImageOrPrintOptions--) | Ctor. |
## Méthodes

| Méthode | Description |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAllColumnsInOnePagePerSheet()](#getAllColumnsInOnePagePerSheet--) | Si AllColumnsInOnePagePerSheet est true, tout le contenu des colonnes d’une feuille sera généré sur une seule page dans le résultat. |
| [getChartImageType()](#getChartImageType--) | Indiquez le type d'image du graphique lors de la conversion. |
| [getCheckWorkbookDefaultFont()](#getCheckWorkbookDefaultFont--) | Lorsque les caractères dans Excel sont Unicode et ne sont pas définis avec la police correcte dans le style de cellule, ils peuvent apparaître sous forme de blocs dans le pdf, l’image. |
| [getClass()](#getClass--) |  |
| [getCustomRenderSettings()](#getCustomRenderSettings--) | Obtient les paramètres personnalisés pendant le rendu. |
| [getDefaultEditLanguage()](#getDefaultEditLanguage--) | Obtient la langue d’édition par défaut. |
| [getDefaultFont()](#getDefaultFont--) | Lorsque les caractères dans Excel sont Unicode et ne sont pas définis avec la police correcte dans le style de cellule, ils peuvent apparaître sous forme de blocs dans le pdf, l’image. |
| [getDrawObjectEventHandler()](#getDrawObjectEventHandler--) | Implémentez cette interface pour obtenir DrawObject et Bound lors du rendu. |
| [getEmbededImageNameInSvg()](#getEmbededImageNameInSvg--) | Indiquez le nom de fichier de l'image intégrée dans le SVG. |
| [getEmfRenderSetting()](#getEmfRenderSetting--) | Paramètre pour le rendu des métafichiers EMF dans le fichier source. |
| [getGridlineColor()](#getGridlineColor--) | Obtient la couleur de la ligne de grille. |
| [getGridlineType()](#getGridlineType--) | Obtient le type des lignes de grille. |
| [getHorizontalResolution()](#getHorizontalResolution--) | Obtient la résolution horizontale des images générées, en points par pouce. |
| [getImageType()](#getImageType--) | Obtient le format des images générées. |
| [getOnePagePerSheet()](#getOnePagePerSheet--) | Si OnePagePerSheet est true, tout le contenu d’une feuille sera généré sur une seule page dans le résultat. |
| [getOnlyArea()](#getOnlyArea--) | Si cette propriété est vraie, une zone sera générée et aucune échelle ne sera appliquée. |
| [getOutputBlankPageWhenNothingToPrint()](#getOutputBlankPageWhenNothingToPrint--) | Indique s’il faut générer une page blanche lorsqu’il n’y a rien à imprimer. |
| [getPageCount()](#getPageCount--) | Obtient le nombre de pages à enregistrer. |
| [getPageIndex()](#getPageIndex--) | Obtient l’indice basé sur zéro de la première page à enregistrer. |
| [getPageSavingCallback()](#getPageSavingCallback--) | Contrôle/Indique la progression du processus d'enregistrement de la page. |
| [getPrintWithStatusDialog()](#getPrintWithStatusDialog--) | Si PrintWithStatusDialog = true, une boîte de dialogue affichant l'état d'impression actuel sera affichée. |
| [getPrintingPage()](#getPrintingPage--) | Indique quelles pages ne seront pas imprimées. |
| [getQuality()](#getQuality--) | Obtient une valeur déterminant la qualité des images générées à appliquer uniquement lors de l'enregistrement des pages au format `Jpeg`. |
| [getSVGFitToViewPort()](#getSVGFitToViewPort--) | si cette propriété est vraie, le SVG généré s'adaptera à la fenêtre d'affichage. |
| [getSaveFormat()](#getSaveFormat--) | Obtient le type de format de fichier de sortie, prise en charge Tiff/XPS |
| [getSheetSet()](#getSheetSet--) | Obtient les feuilles à rendre. |
| [getSvgCssPrefix()](#getSvgCssPrefix--) | Obtient le préfixe du nom CSS dans le SVG, la valeur par défaut est une chaîne vide. |
| [getTextCrossType()](#getTextCrossType--) | Obtient le type d'affichage du texte lorsque la largeur du texte est supérieure à la largeur de la cellule. |
| [getTiffColorDepth()](#getTiffColorDepth--) | Obtient la profondeur de bits à appliquer uniquement lors de l'enregistrement des pages au format `Tiff`. |
| [getTiffCompression()](#getTiffCompression--) | Obtient le type de compression à appliquer uniquement lors de l'enregistrement des pages au format `Tiff`. |
| [getTiffPhotometricInterpretation()](#getTiffPhotometricInterpretation--) | Obtient le type d'interprétation photométrique à appliquer uniquement lors de l'enregistrement des pages au format `Tiff`. |
| [getTransparent()](#getTransparent--) | Indique si l'arrière-plan de l'image générée doit être transparent. |
| [getVerticalResolution()](#getVerticalResolution--) | Obtient la résolution verticale des images générées, en points par pouce. |
| [getWarningCallback()](#getWarningCallback--) | Obtient le rappel d'avertissement. |
| [hashCode()](#hashCode--) |  |
| [isCellAutoFit()](#isCellAutoFit--) | Indique si la largeur et la hauteur des cellules sont automatiquement ajustées en fonction de la valeur de la cellule. |
| [isFontSubstitutionCharGranularity()](#isFontSubstitutionCharGranularity--) | Indique s'il faut uniquement substituer la police du caractère lorsque la police de la cellule n'est pas compatible. |
| [isOptimized()](#isOptimized--) | Indique s'il faut optimiser les éléments de sortie. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAllColumnsInOnePagePerSheet(boolean value)](#setAllColumnsInOnePagePerSheet-boolean-) | Si AllColumnsInOnePagePerSheet est true, tout le contenu des colonnes d’une feuille sera généré sur une seule page dans le résultat. |
| [setCellAutoFit(boolean value)](#setCellAutoFit-boolean-) | Indique si la largeur et la hauteur des cellules sont automatiquement ajustées en fonction de la valeur de la cellule. |
| [setChartImageType(ImageFormat value)](#setChartImageType-com.aspose.cells.ImageFormat-) | Indiquez le type d'image du graphique lors de la conversion. |
| [setCheckWorkbookDefaultFont(boolean value)](#setCheckWorkbookDefaultFont-boolean-) | Lorsque les caractères dans Excel sont Unicode et ne sont pas définis avec la police correcte dans le style de cellule, ils peuvent apparaître sous forme de blocs dans le pdf, l’image. |
| [setCustomRenderSettings(CustomRenderSettings value)](#setCustomRenderSettings-com.aspose.cells.CustomRenderSettings-) | Définit les paramètres personnalisés pendant le rendu. |
| [setDefaultEditLanguage(int value)](#setDefaultEditLanguage-int-) | Définit la langue d'édition par défaut. |
| [setDefaultFont(String value)](#setDefaultFont-java.lang.String-) | Lorsque les caractères dans Excel sont Unicode et ne sont pas définis avec la police correcte dans le style de cellule, ils peuvent apparaître sous forme de blocs dans le pdf, l’image. |
| [setDesiredSize(int desiredWidth, int desiredHeight)](#setDesiredSize-int-int-) | Définit la largeur et la hauteur souhaitées de l'image. |
| [setDesiredSize(int desiredWidth, int desiredHeight, boolean keepAspectRatio)](#setDesiredSize-int-int-boolean-) | Définit la largeur et la hauteur souhaitées de l'image. |
| [setDrawObjectEventHandler(DrawObjectEventHandler value)](#setDrawObjectEventHandler-com.aspose.cells.DrawObjectEventHandler-) | Implémentez cette interface pour obtenir DrawObject et Bound lors du rendu. |
| [setEmbededImageNameInSvg(String value)](#setEmbededImageNameInSvg-java.lang.String-) | Indiquez le nom de fichier de l'image intégrée dans le SVG. |
| [setEmfRenderSetting(int value)](#setEmfRenderSetting-int-) | Paramètre pour le rendu des métafichiers EMF dans le fichier source. |
| [setFontSubstitutionCharGranularity(boolean value)](#setFontSubstitutionCharGranularity-boolean-) | Indique s'il faut uniquement substituer la police du caractère lorsque la police de la cellule n'est pas compatible. |
| [setGridlineColor(Color value)](#setGridlineColor-com.aspose.cells.Color-) | Définit la couleur de la ligne de grille. |
| [setGridlineType(int value)](#setGridlineType-int-) | Définit le type de ligne de grille. |
| [setHorizontalResolution(int value)](#setHorizontalResolution-int-) | Définit la résolution horizontale des images générées, en points par pouce. |
| [setImageType(int value)](#setImageType-int-) | Définit le format des images générées. |
| [setOnePagePerSheet(boolean value)](#setOnePagePerSheet-boolean-) | Si OnePagePerSheet est true, tout le contenu d’une feuille sera généré sur une seule page dans le résultat. |
| [setOnlyArea(boolean value)](#setOnlyArea-boolean-) | Si cette propriété est vraie, une zone sera générée et aucune échelle ne sera appliquée. |
| [setOptimized(boolean value)](#setOptimized-boolean-) | Indique s'il faut optimiser les éléments de sortie. |
| [setOutputBlankPageWhenNothingToPrint(boolean value)](#setOutputBlankPageWhenNothingToPrint-boolean-) | Indique s’il faut générer une page blanche lorsqu’il n’y a rien à imprimer. |
| [setPageCount(int value)](#setPageCount-int-) | Définit le nombre de pages à enregistrer. |
| [setPageIndex(int value)](#setPageIndex-int-) | Définit l'index de base zéro de la première page à enregistrer. |
| [setPageSavingCallback(IPageSavingCallback value)](#setPageSavingCallback-com.aspose.cells.IPageSavingCallback-) | Contrôle/Indique la progression du processus d'enregistrement de la page. |
| [setPrintWithStatusDialog(boolean value)](#setPrintWithStatusDialog-boolean-) | Si PrintWithStatusDialog = true, une boîte de dialogue affichant l'état d'impression actuel sera affichée. |
| [setPrintingPage(int value)](#setPrintingPage-int-) | Indique quelles pages ne seront pas imprimées. |
| [setQuality(int value)](#setQuality-int-) | Définit une valeur déterminant la qualité des images générées à appliquer uniquement lors de l’enregistrement des pages au format `Jpeg`. |
| [setRenderingHint(RenderingHints.Key key, Object value)](#setRenderingHint-java.awt.RenderingHints.Key-java.lang.Object-) | Définit la valeur d’une préférence unique pour les algorithmes de rendu. |
| [setSVGFitToViewPort(boolean value)](#setSVGFitToViewPort-boolean-) | si cette propriété est vraie, le SVG généré s'adaptera à la fenêtre d'affichage. |
| [setSaveFormat(int value)](#setSaveFormat-int-) | Définit le type de format de fichier de sortie, prise en charge Tiff/XPS. |
| [setSheetSet(SheetSet value)](#setSheetSet-com.aspose.cells.SheetSet-) | Définit les feuilles à rendre. |
| [setSvgCssPrefix(String value)](#setSvgCssPrefix-java.lang.String-) | Définit le préfixe du nom CSS dans le SVG, la valeur par défaut est une chaîne vide. |
| [setTextCrossType(int value)](#setTextCrossType-int-) | Définit le type d'affichage du texte lorsque la largeur du texte est supérieure à la largeur de la cellule. |
| [setTiffColorDepth(int value)](#setTiffColorDepth-int-) | Définit la profondeur de couleur à appliquer uniquement lors de l’enregistrement des pages au format `Tiff`. |
| [setTiffCompression(int value)](#setTiffCompression-int-) | Définit le type de compression à appliquer uniquement lors de l’enregistrement des pages au format `Tiff`. |
| [setTiffPhotometricInterpretation(int value)](#setTiffPhotometricInterpretation-int-) | Définit le type de PhotometricInterpretation à appliquer uniquement lors de l’enregistrement des pages au format `Tiff`. |
| [setTransparent(boolean value)](#setTransparent-boolean-) | Indique si l'arrière-plan de l'image générée doit être transparent. |
| [setVerticalResolution(int value)](#setVerticalResolution-int-) | Définit la résolution verticale des images générées, en points par pouce. |
| [setWarningCallback(IWarningCallback value)](#setWarningCallback-com.aspose.cells.IWarningCallback-) | Définit le rappel d’avertissement. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### ImageOrPrintOptions() {#ImageOrPrintOptions--}
```
public ImageOrPrintOptions()
```


Ctor.

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


Si AllColumnsInOnePagePerSheet est true, tout le contenu des colonnes d’une feuille sera exporté sur une seule page dans le résultat. La largeur du format de papier de pagesetup sera invalide, et les autres paramètres de pagesetup resteront effectifs.

**Returns:**
boolean
### getChartImageType() {#getChartImageType--}
```
public ImageFormat getChartImageType()
```


Indique le type d’image du graphique lors de la conversion. valeur par défaut : PNG.

**Remarks**

NOTE : Ce membre est maintenant obsolète. À la place, Chart et Shape sont toujours rendus comme des éléments vectoriels (par ex. point, ligne) pour la qualité du rendu. Cette propriété sera supprimée 12 mois après juin 2022. Aspose s’excuse pour tout désagrément que vous auriez pu rencontrer.

**Returns:**
[ImageFormat](../../com.aspose.cells/imageformat)
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
### getEmbededImageNameInSvg() {#getEmbededImageNameInSvg--}
```
public String getEmbededImageNameInSvg()
```


Indique le nom de fichier de l’image incorporée dans le svg. Cela doit être le chemin complet avec le répertoire, par exemple "c:\\xpsEmbedded".

**Remarks**

NOTE : Ce membre est maintenant obsolète. À la place, veuillez supprimer cette propriété car les images sont désormais toujours incorporées dans le Svg au format base64. Cette propriété sera supprimée 12 mois après avril 2025. Aspose s’excuse pour tout désagrément que vous auriez pu rencontrer.

**Returns:**
java.lang.String
### getEmfRenderSetting() {#getEmfRenderSetting--}
```
public int getEmfRenderSetting()
```


Paramètre pour le rendu des métafichiers EMF dans le fichier source.

Voir [EmfRenderSetting](../../com.aspose.cells/emfrendersetting).

**Remarks**

Les métafichiers EMF identifiés comme "EMF+ Dual" peuvent contenir à la fois des enregistrements EMF+ et des enregistrements EMF. Chaque type d’enregistrement peut être utilisé pour rendre l’image, uniquement les enregistrements EMF+, ou uniquement les enregistrements EMF. Lorsque [EmfRenderSetting.EMF\\_PLUS\\_PREFER](../../com.aspose.cells/emfrendersetting\\#EMF-PLUS-PREFER) est défini, les enregistrements EMF+ seront analysés lors du rendu de l’image, sinon seuls les enregistrements EMF seront analysés. La valeur par défaut est [EmfRenderSetting.EMF\\_ONLY](../../com.aspose.cells/emfrendersetting\\#EMF-ONLY). Pour les frameworks qui dépendent de .NET System.Drawing.Common, ce paramètre est ignoré.

**Returns:**
int
### getGridlineColor() {#getGridlineColor--}
```
public Color getGridlineColor()
```


Obtient la couleur de la ligne de grille.

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
### getHorizontalResolution() {#getHorizontalResolution--}
```
public int getHorizontalResolution()
```


Obtient la résolution horizontale des images générées, en points par pouce.

**Remarks**

La valeur par défaut est 96. La configuration de  et  affecte la largeur et la hauteur de l’image de sortie en pixels.

**Example**

Le code suivant définit la résolution à 192, la largeur et la hauteur de l’image générée sont le double de celles obtenues avec la résolution laissée à la valeur par défaut 96.

```
         Workbook wb = new Workbook("Book1.xlsx");
 
         ImageOrPrintOptions opts = new ImageOrPrintOptions();
 
         //Set output image type: png.
         opts.setImageType(ImageType.PNG);
 
         //Set resolution to 192.
         opts.setHorizontalResolution(192);
         opts.setVerticalResolution(192);
 
         //Render worksheet page to image.
         SheetRender sr = new SheetRender(wb.getWorksheets().get(0), opts);
         sr.toImage(0, "Sheet_Page1.png");
```

**Returns:**
int
### getImageType() {#getImageType--}
```
public int getImageType()
```


Obtient le format des images générées. valeur par défaut : PNG.

Voir [ImageType](../../com.aspose.cells/imagetype).

**Returns:**
int
### getOnePagePerSheet() {#getOnePagePerSheet--}
```
public boolean getOnePagePerSheet()
```


Si OnePagePerSheet est vrai, tout le contenu d’une feuille sera exporté vers une seule page dans le résultat. La taille du papier de pagesetup sera invalide, et les autres paramètres de pagesetup resteront appliqués.

**Returns:**
boolean
### getOnlyArea() {#getOnlyArea--}
```
public boolean getOnlyArea()
```


Si cette propriété est vraie, une zone sera générée et aucune échelle ne sera appliquée.

**Returns:**
boolean
### getOutputBlankPageWhenNothingToPrint() {#getOutputBlankPageWhenNothingToPrint--}
```
public boolean getOutputBlankPageWhenNothingToPrint()
```


Indique s’il faut générer une page blanche lorsqu’il n’y a rien à imprimer.

**Remarks**

La valeur par défaut est false.

**Returns:**
boolean
### getPageCount() {#getPageCount--}
```
public int getPageCount()
```


Obtient le nombre de pages à enregistrer.

**Remarks**

La valeur par défaut est System.Int32.MaxValue, ce qui signifie que toutes les pages seront rendues.

**Returns:**
int
### getPageIndex() {#getPageIndex--}
```
public int getPageIndex()
```


Obtient l’indice basé sur zéro de la première page à enregistrer.

**Remarks**

La valeur par défaut est 0.

**Returns:**
int
### getPageSavingCallback() {#getPageSavingCallback--}
```
public IPageSavingCallback getPageSavingCallback()
```


Contrôle/Indique la progression du processus d'enregistrement de la page.

**Returns:**
[IPageSavingCallback](../../com.aspose.cells/ipagesavingcallback)
### getPrintWithStatusDialog() {#getPrintWithStatusDialog--}
```
public boolean getPrintWithStatusDialog()
```


Si PrintWithStatusDialog = true, une boîte de dialogue affichant l’état d’impression actuel sera affichée. Sinon, aucune boîte de dialogue ne sera affichée.

**Returns:**
boolean
### getPrintingPage() {#getPrintingPage--}
```
public int getPrintingPage()
```


Indique quelles pages ne seront pas imprimées.

Voir [PrintingPageType](../../com.aspose.cells/printingpagetype).

**Returns:**
int
### getQuality() {#getQuality--}
```
public int getQuality()
```


Obtient une valeur déterminant la qualité des images générées à appliquer uniquement lors de l'enregistrement des pages au format `Jpeg`. La valeur par défaut est 100.

**Remarks**

N'a d'effet que lors de l'enregistrement au format JPEG. La valeur doit être comprise entre 0 et 100. La valeur par défaut est 100.

**Returns:**
int
### getSVGFitToViewPort() {#getSVGFitToViewPort--}
```
public boolean getSVGFitToViewPort()
```


si cette propriété est vraie, le SVG généré s'adaptera à la fenêtre d'affichage.

**Remarks**

NOTE : Ce membre est maintenant obsolète. À la place, veuillez utiliser [SvgImageOptions.getFitToViewPort()](../../com.aspose.cells/svgimageoptions\#getFitToViewPort--). Cette propriété sera supprimée 12 mois plus tard, à partir d’avril 2025. Aspose s’excuse pour tout désagrément que vous auriez pu rencontrer.

**Returns:**
boolean
### getSaveFormat() {#getSaveFormat--}
```
public int getSaveFormat()
```


Obtient le type de format de fichier de sortie, prise en charge Tiff/XPS

Voir [SaveFormat](../../com.aspose.cells/saveformat).

**Remarks**

NOTE : Ce membre est maintenant obsolète. À la place, pour Tiff/Svg, utilisez [getImageType()](../../com.aspose.cells/imageorprintoptions\#getImageType--); pour Xps, utilisez [Workbook.save(String,SaveOptions)](../../com.aspose.cells/workbook\#save-String-SaveOptions-) avec [XpsSaveOptions](../../com.aspose.cells/xpssaveoptions). Cette propriété sera supprimée 12 mois plus tard, à partir d’août 2022. Aspose s’excuse pour tout désagrément que vous auriez pu rencontrer.

**Returns:**
int
### getSheetSet() {#getSheetSet--}
```
public SheetSet getSheetSet()
```


Obtient les feuilles à rendre. La valeur par défaut est toutes les feuilles visibles du classeur : [SheetSet.getVisible()](../../com.aspose.cells/sheetset\#getVisible--).

**Remarks**

Le paramètre est ignoré lorsqu'il est utilisé dans [SheetRender](../../com.aspose.cells/sheetrender).

**Returns:**
[SheetSet](../../com.aspose.cells/sheetset)
### getSvgCssPrefix() {#getSvgCssPrefix--}
```
public String getSvgCssPrefix()
```


Obtient le préfixe du nom CSS dans le SVG, la valeur par défaut est une chaîne vide.

**Remarks**

NOTE : Ce membre est maintenant obsolète. À la place, veuillez utiliser [SvgImageOptions.getCssPrefix()](../../com.aspose.cells/svgimageoptions\#getCssPrefix--). Cette propriété sera supprimée 12 mois plus tard, à partir d’avril 2025. Aspose s’excuse pour tout désagrément que vous auriez pu rencontrer.

**Returns:**
java.lang.String
### getTextCrossType() {#getTextCrossType--}
```
public int getTextCrossType()
```


Obtient le type d'affichage du texte lorsque la largeur du texte est supérieure à la largeur de la cellule.

Voir [TextCrossType](../../com.aspose.cells/textcrosstype).

**Returns:**
int
### getTiffColorDepth() {#getTiffColorDepth--}
```
public int getTiffColorDepth()
```


Obtient la profondeur de bits à appliquer uniquement lors de l'enregistrement des pages au format `Tiff`.

Voir [ColorDepth](../../com.aspose.cells/colordepth).

**Remarks**

N'a d'effet que lors de l'enregistrement au format TIFF. Si TiffCompression est réglé sur CCITT3 ou CCITT4, cela ne prendra pas effet, la profondeur de bits de l'image TIFF générée sera toujours de 1.

**Returns:**
int
### getTiffCompression() {#getTiffCompression--}
```
public int getTiffCompression()
```


Obtient le type de compression à appliquer uniquement lors de l'enregistrement des pages au format `Tiff`.

Voir [TiffCompression](../../com.aspose.cells/tiffcompression).

**Remarks**

N'a d'effet que lors de l'enregistrement au format TIFF. La valeur par défaut est Lzw.

**Returns:**
int
### getTiffPhotometricInterpretation() {#getTiffPhotometricInterpretation--}
```
public int getTiffPhotometricInterpretation()
```


Obtient le type d'interprétation photométrique à appliquer uniquement lors de l'enregistrement des pages au format `Tiff`.

**Remarks**

N'a d'effet que lors de l'enregistrement au format TIFF. La valeur par défaut est -1, ce qui signifie qu'aucune PhotometricInterpretation n'est appliquée.

**Returns:**
int
### getTransparent() {#getTransparent--}
```
public boolean getTransparent()
```


Indique si l'arrière-plan de l'image générée doit être transparent.

**Remarks**

La valeur par défaut est false. Cela signifie que l'arrière-plan des images générées est blanc.

**Returns:**
boolean
### getVerticalResolution() {#getVerticalResolution--}
```
public int getVerticalResolution()
```


Obtient la résolution verticale des images générées, en points par pouce.

**Remarks**

La valeur par défaut est 96. La configuration de  et  affecte la largeur et la hauteur de l’image de sortie en pixels.

**Example**

Le code suivant définit la résolution à 192, la largeur et la hauteur de l’image générée sont le double de celles obtenues avec la résolution laissée à la valeur par défaut 96.

```
         Workbook wb = new Workbook("Book1.xlsx");
 
         ImageOrPrintOptions opts = new ImageOrPrintOptions();
 
         //Set output image type: png.
         opts.setImageType(ImageType.PNG);
 
         //Set resolution to 192.
         opts.setHorizontalResolution(192);
         opts.setVerticalResolution(192);
 
         //Render Chart to image.
         wb.getWorksheets().get(0).getCharts().get(0).toImage("Chart.png", opts);
```

**Returns:**
int
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
### isCellAutoFit() {#isCellAutoFit--}
```
public boolean isCellAutoFit()
```


Indique si la largeur et la hauteur des cellules sont automatiquement ajustées en fonction de la valeur de la cellule. La valeur par défaut est false.

**Remarks**

NOTE : Ce membre est maintenant obsolète. À la place, cette propriété n'est pas utilisée, veuillez la supprimer. Cette propriété sera supprimée 12 mois plus tard, à partir d’août 2022. Aspose s’excuse pour tout désagrément que vous auriez pu rencontrer.

**Returns:**
boolean
### isFontSubstitutionCharGranularity() {#isFontSubstitutionCharGranularity--}
```
public boolean isFontSubstitutionCharGranularity()
```


Indique s'il faut uniquement substituer la police du caractère lorsque la police de la cellule n'est pas compatible.

**Remarks**

La valeur par défaut est false. Nous essaierons d’abord la police par défaut du classeur et de PdfSaveOption/system pour la police des cellules.

**Returns:**
boolean
### isOptimized() {#isOptimized--}
```
public boolean isOptimized()
```


Indique s'il faut optimiser les éléments de sortie.

**Remarks**

La valeur par défaut est false. Actuellement, lorsque cette propriété est définie sur true, les optimisations suivantes sont effectuées : 1. optimiser les lignes de bordure. 2. optimiser la taille du fichier lors du rendu en image Svg.

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


Si AllColumnsInOnePagePerSheet est true, tout le contenu des colonnes d’une feuille sera exporté sur une seule page dans le résultat. La largeur du format de papier de pagesetup sera invalide, et les autres paramètres de pagesetup resteront effectifs.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setCellAutoFit(boolean value) {#setCellAutoFit-boolean-}
```
public void setCellAutoFit(boolean value)
```


Indique si la largeur et la hauteur des cellules sont automatiquement ajustées en fonction de la valeur de la cellule. La valeur par défaut est false.

**Remarks**

NOTE : Ce membre est maintenant obsolète. À la place, cette propriété n'est pas utilisée, veuillez la supprimer. Cette propriété sera supprimée 12 mois plus tard, à partir d’août 2022. Aspose s’excuse pour tout désagrément que vous auriez pu rencontrer.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setChartImageType(ImageFormat value) {#setChartImageType-com.aspose.cells.ImageFormat-}
```
public void setChartImageType(ImageFormat value)
```


Indique le type d’image du graphique lors de la conversion. valeur par défaut : PNG.

**Remarks**

NOTE : Ce membre est maintenant obsolète. À la place, Chart et Shape sont toujours rendus comme des éléments vectoriels (par ex. point, ligne) pour la qualité du rendu. Cette propriété sera supprimée 12 mois après juin 2022. Aspose s’excuse pour tout désagrément que vous auriez pu rencontrer.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | [ImageFormat](../../com.aspose.cells/imageformat) |  |

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

### setDesiredSize(int desiredWidth, int desiredHeight) {#setDesiredSize-int-int-}
```
public void setDesiredSize(int desiredWidth, int desiredHeight)
```


Définit la largeur et la hauteur souhaitées de l'image.

**Remarks**

NOTE : Ce membre est maintenant obsolète. À la place, veuillez utiliser [setDesiredSize(int,int,boolean)](../../com.aspose.cells/imageorprintoptions\#setDesiredSize-int-int-boolean-) en définissant le paramètre keepAspectRatio sur false. Cette propriété sera supprimée 12 mois plus tard, à partir de mai 2023. Aspose s’excuse pour tout désagrément que vous auriez pu rencontrer.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| desiredWidth | int | largeur souhaitée en pixels |
| desiredHeight | int | hauteur souhaitée en pixels |

### setDesiredSize(int desiredWidth, int desiredHeight, boolean keepAspectRatio) {#setDesiredSize-int-int-boolean-}
```
public void setDesiredSize(int desiredWidth, int desiredHeight, boolean keepAspectRatio)
```


Définit la largeur et la hauteur souhaitées de l'image.

**Remarks**

La largeur et la hauteur de l'image de sortie en pixels seront uniquement basées sur la largeur et la hauteur souhaitées définies. Les  et  n'auront aucun effet sur la largeur et la hauteur de l'image de sortie dans ce cas.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| desiredWidth | int | largeur souhaitée en pixels |
| desiredHeight | int | hauteur souhaitée en pixels |
| keepAspectRatio | boolean | indique s'il faut conserver le ratio d'aspect de l'image d'origine |

### setDrawObjectEventHandler(DrawObjectEventHandler value) {#setDrawObjectEventHandler-com.aspose.cells.DrawObjectEventHandler-}
```
public void setDrawObjectEventHandler(DrawObjectEventHandler value)
```


Implémentez cette interface pour obtenir DrawObject et Bound lors du rendu.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | [DrawObjectEventHandler](../../com.aspose.cells/drawobjecteventhandler) |  |

### setEmbededImageNameInSvg(String value) {#setEmbededImageNameInSvg-java.lang.String-}
```
public void setEmbededImageNameInSvg(String value)
```


Indique le nom de fichier de l’image incorporée dans le svg. Cela doit être le chemin complet avec le répertoire, par exemple "c:\\xpsEmbedded".

**Remarks**

NOTE : Ce membre est maintenant obsolète. À la place, veuillez supprimer cette propriété car les images sont désormais toujours incorporées dans le Svg au format base64. Cette propriété sera supprimée 12 mois après avril 2025. Aspose s’excuse pour tout désagrément que vous auriez pu rencontrer.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

### setEmfRenderSetting(int value) {#setEmfRenderSetting-int-}
```
public void setEmfRenderSetting(int value)
```


Paramètre pour le rendu des métafichiers EMF dans le fichier source.

Voir [EmfRenderSetting](../../com.aspose.cells/emfrendersetting).

**Remarks**

Les métafichiers EMF identifiés comme "EMF+ Dual" peuvent contenir à la fois des enregistrements EMF+ et des enregistrements EMF. Chaque type d’enregistrement peut être utilisé pour rendre l’image, uniquement les enregistrements EMF+, ou uniquement les enregistrements EMF. Lorsque [EmfRenderSetting.EMF\\_PLUS\\_PREFER](../../com.aspose.cells/emfrendersetting\\#EMF-PLUS-PREFER) est défini, les enregistrements EMF+ seront analysés lors du rendu de l’image, sinon seuls les enregistrements EMF seront analysés. La valeur par défaut est [EmfRenderSetting.EMF\\_ONLY](../../com.aspose.cells/emfrendersetting\\#EMF-ONLY). Pour les frameworks qui dépendent de .NET System.Drawing.Common, ce paramètre est ignoré.

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


Définit la couleur de la ligne de grille.

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

### setHorizontalResolution(int value) {#setHorizontalResolution-int-}
```
public void setHorizontalResolution(int value)
```


Définit la résolution horizontale des images générées, en points par pouce.

**Remarks**

La valeur par défaut est 96. La configuration de  et  affecte la largeur et la hauteur de l’image de sortie en pixels.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setImageType(int value) {#setImageType-int-}
```
public void setImageType(int value)
```


Définit le format des images générées. valeur par défaut : PNG.

Voir [ImageType](../../com.aspose.cells/imagetype).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setOnePagePerSheet(boolean value) {#setOnePagePerSheet-boolean-}
```
public void setOnePagePerSheet(boolean value)
```


Si OnePagePerSheet est vrai, tout le contenu d’une feuille sera exporté vers une seule page dans le résultat. La taille du papier de pagesetup sera invalide, et les autres paramètres de pagesetup resteront appliqués.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setOnlyArea(boolean value) {#setOnlyArea-boolean-}
```
public void setOnlyArea(boolean value)
```


Si cette propriété est vraie, une zone sera générée et aucune échelle ne sera appliquée.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setOptimized(boolean value) {#setOptimized-boolean-}
```
public void setOptimized(boolean value)
```


Indique s'il faut optimiser les éléments de sortie.

**Remarks**

La valeur par défaut est false. Actuellement, lorsque cette propriété est définie sur true, les optimisations suivantes sont effectuées : 1. optimiser les lignes de bordure. 2. optimiser la taille du fichier lors du rendu en image Svg.

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

La valeur par défaut est false.

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

### setPrintWithStatusDialog(boolean value) {#setPrintWithStatusDialog-boolean-}
```
public void setPrintWithStatusDialog(boolean value)
```


Si PrintWithStatusDialog = true, une boîte de dialogue affichant l’état d’impression actuel sera affichée. Sinon, aucune boîte de dialogue ne sera affichée.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setPrintingPage(int value) {#setPrintingPage-int-}
```
public void setPrintingPage(int value)
```


Indique quelles pages ne seront pas imprimées.

Voir [PrintingPageType](../../com.aspose.cells/printingpagetype).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setQuality(int value) {#setQuality-int-}
```
public void setQuality(int value)
```


Définit une valeur déterminant la qualité des images générées à appliquer uniquement lors de l'enregistrement des pages au format `Jpeg`. La valeur par défaut est 100.

**Remarks**

N'a d'effet que lors de l'enregistrement au format JPEG. La valeur doit être comprise entre 0 et 100. La valeur par défaut est 100.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setRenderingHint(RenderingHints.Key key, Object value) {#setRenderingHint-java.awt.RenderingHints.Key-java.lang.Object-}
```
public void setRenderingHint(RenderingHints.Key key, Object value)
```


Définit la valeur d'une préférence unique pour les algorithmes de rendu. Les catégories d'indices comprennent des contrôles de la qualité de rendu et du compromis global temps/qualité dans le processus de rendu. Référez-vous à la classe RenderingHints pour les définitions de certaines clés et valeurs courantes.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| clé | java.awt.RenderingHints.Key | la clé de l'indice à définir. |
| valeur | java.lang.Object | la valeur indiquant les préférences pour la catégorie d'indice spécifiée. |

### setSVGFitToViewPort(boolean value) {#setSVGFitToViewPort-boolean-}
```
public void setSVGFitToViewPort(boolean value)
```


si cette propriété est vraie, le SVG généré s'adaptera à la fenêtre d'affichage.

**Remarks**

NOTE : Ce membre est maintenant obsolète. À la place, veuillez utiliser [SvgImageOptions.getFitToViewPort()](../../com.aspose.cells/svgimageoptions\#getFitToViewPort--). Cette propriété sera supprimée 12 mois plus tard, à partir d’avril 2025. Aspose s’excuse pour tout désagrément que vous auriez pu rencontrer.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setSaveFormat(int value) {#setSaveFormat-int-}
```
public void setSaveFormat(int value)
```


Définit le type de format de fichier de sortie, prise en charge Tiff/XPS.

Voir [SaveFormat](../../com.aspose.cells/saveformat).

**Remarks**

NOTE : Ce membre est maintenant obsolète. À la place, pour Tiff/Svg, utilisez [getImageType()](../../com.aspose.cells/imageorprintoptions\#getImageType--); pour Xps, utilisez [Workbook.save(String,SaveOptions)](../../com.aspose.cells/workbook\#save-String-SaveOptions-) avec [XpsSaveOptions](../../com.aspose.cells/xpssaveoptions). Cette propriété sera supprimée 12 mois plus tard, à partir d’août 2022. Aspose s’excuse pour tout désagrément que vous auriez pu rencontrer.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setSheetSet(SheetSet value) {#setSheetSet-com.aspose.cells.SheetSet-}
```
public void setSheetSet(SheetSet value)
```


Définit les feuilles à rendre. La valeur par défaut est toutes les feuilles visibles du classeur : [SheetSet.getVisible()](../../com.aspose.cells/sheetset\#getVisible--).

**Remarks**

Le paramètre est ignoré lorsqu'il est utilisé dans [SheetRender](../../com.aspose.cells/sheetrender).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | [SheetSet](../../com.aspose.cells/sheetset) |  |

### setSvgCssPrefix(String value) {#setSvgCssPrefix-java.lang.String-}
```
public void setSvgCssPrefix(String value)
```


Définit le préfixe du nom CSS dans le SVG, la valeur par défaut est une chaîne vide.

**Remarks**

NOTE : Ce membre est maintenant obsolète. À la place, veuillez utiliser [SvgImageOptions.getCssPrefix()](../../com.aspose.cells/svgimageoptions\#getCssPrefix--). Cette propriété sera supprimée 12 mois plus tard, à partir d’avril 2025. Aspose s’excuse pour tout désagrément que vous auriez pu rencontrer.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

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

### setTiffColorDepth(int value) {#setTiffColorDepth-int-}
```
public void setTiffColorDepth(int value)
```


Définit la profondeur de couleur à appliquer uniquement lors de l’enregistrement des pages au format `Tiff`.

Voir [ColorDepth](../../com.aspose.cells/colordepth).

**Remarks**

N'a d'effet que lors de l'enregistrement au format TIFF. Si TiffCompression est réglé sur CCITT3 ou CCITT4, cela ne prendra pas effet, la profondeur de bits de l'image TIFF générée sera toujours de 1.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setTiffCompression(int value) {#setTiffCompression-int-}
```
public void setTiffCompression(int value)
```


Définit le type de compression à appliquer uniquement lors de l’enregistrement des pages au format `Tiff`.

Voir [TiffCompression](../../com.aspose.cells/tiffcompression).

**Remarks**

N'a d'effet que lors de l'enregistrement au format TIFF. La valeur par défaut est Lzw.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setTiffPhotometricInterpretation(int value) {#setTiffPhotometricInterpretation-int-}
```
public void setTiffPhotometricInterpretation(int value)
```


Définit le type de PhotometricInterpretation à appliquer uniquement lors de l’enregistrement des pages au format `Tiff`.

**Remarks**

N'a d'effet que lors de l'enregistrement au format TIFF. La valeur par défaut est -1, ce qui signifie qu'aucune PhotometricInterpretation n'est appliquée.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setTransparent(boolean value) {#setTransparent-boolean-}
```
public void setTransparent(boolean value)
```


Indique si l'arrière-plan de l'image générée doit être transparent.

**Remarks**

La valeur par défaut est false. Cela signifie que l'arrière-plan des images générées est blanc.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setVerticalResolution(int value) {#setVerticalResolution-int-}
```
public void setVerticalResolution(int value)
```


Définit la résolution verticale des images générées, en points par pouce.

**Remarks**

La valeur par défaut est 96. La configuration de  et  affecte la largeur et la hauteur de l’image de sortie en pixels.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

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

