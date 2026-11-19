---
title: "PageSetup"
second_title: "Référence API d'Aspose.Cells pour Java"
description: "Encapsule l'objet qui représente la description de la configuration de la page."
type: docs
url: /fr/java/com.aspose.cells/pagesetup/
---

**Inheritance:**
java.lang.Object
```
public class PageSetup
```

Encapsule l'objet qui représente la description de la configuration de page. L'objet PageSetup contient toutes les options de configuration de page.

**Example**

```
         Workbook workbook = new Workbook();
 
         WorksheetCollection sheets = workbook.getWorksheets();
 
         //Add a worksheet
         sheets.add();
         Worksheet sheet = sheets.get(1);
         PageSetup pageSetup = sheet.getPageSetup();
         pageSetup.setPrintArea("D1:K13");
 
         //do your business
```
## Méthodes

| Méthode | Description |
| --- | --- |
| [clearHeaderFooter()](#clearHeaderFooter--) | Efface les paramètres d'en-tête et de pied de page. |
| [copy(PageSetup source, CopyOptions copyOptions)](#copy-com.aspose.cells.PageSetup-com.aspose.cells.CopyOptions-) | Copie les paramètres de la configuration de page. |
| [customPaperSize(double width, double height)](#customPaperSize-double-double-) | Définit la taille du papier personnalisée, en pouces. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getBlackAndWhite()](#getBlackAndWhite--) | Indique si les éléments du document seront imprimés en noir et blanc. |
| [getBottomMargin()](#getBottomMargin--) | Indique la taille de la marge inférieure, en centimètres. |
| [getBottomMarginInch()](#getBottomMarginInch--) | Indique la taille de la marge inférieure, en pouces. |
| [getCenterHorizontally()](#getCenterHorizontally--) | Indique si la feuille est imprimée centrée horizontalement. |
| [getCenterVertically()](#getCenterVertically--) | Indique si la feuille est imprimée centrée verticalement. |
| [getClass()](#getClass--) |  |
| [getCommands(String headerFooterScript)](#getCommands-java.lang.String-) | Récupère toutes les commandes d’en-tête ou de pied de page. |
| [getEvenFooter(int section)](#getEvenFooter-int-) | Récupère un script formatant le pied de page pair d’un fichier Excel. |
| [getEvenHeader(int section)](#getEvenHeader-int-) | Récupère un script formatant l’en-tête pair d’un fichier Excel. |
| [getFirstPageFooter(int section)](#getFirstPageFooter-int-) | Récupère un script formatant le pied de page de la première page d’un fichier Excel. |
| [getFirstPageHeader(int section)](#getFirstPageHeader-int-) | Récupère un script formatant l’en-tête de la première page d’un fichier Excel. |
| [getFirstPageNumber()](#getFirstPageNumber--) | Représente le numéro de la première page qui sera utilisé lors de l’impression de cette feuille. |
| [getFitToPagesTall()](#getFitToPagesTall--) | Représente le nombre de pages en hauteur auquel la feuille de calcul sera mise à l’échelle lors de l’impression. |
| [getFitToPagesWide()](#getFitToPagesWide--) | Représente le nombre de pages en largeur auquel la feuille de calcul sera mise à l’échelle lors de l’impression. |
| [getFooter(int section)](#getFooter-int-) | Récupère un script formatant le pied de page d’un fichier Excel. |
| [getFooterMargin()](#getFooterMargin--) | Représente la distance du bas de la page au pied de page, en centimètres. |
| [getFooterMarginInch()](#getFooterMarginInch--) | Représente la distance du bas de la page au pied de page, en pouces. |
| [getHeader(int section)](#getHeader-int-) | Récupère un script formatant l’en-tête d’un fichier Excel. |
| [getHeaderMargin()](#getHeaderMargin--) | Représente la distance du haut de la page à l’en-tête, en centimètres. |
| [getHeaderMarginInch()](#getHeaderMarginInch--) | Représente la distance du haut de la page à l’en-tête, en pouces. |
| [getLeftMargin()](#getLeftMargin--) | Représente la taille de la marge gauche, en centimètres. |
| [getLeftMarginInch()](#getLeftMarginInch--) | Représente la taille de la marge gauche, en pouces. |
| [getODSPageBackground()](#getODSPageBackground--) | Récupère l’arrière-plan d’ODS. |
| [getOrder()](#getOrder--) | Représente l’ordre que Microsoft Excel utilise pour numéroter les pages lors de l’impression d’une grande feuille de calcul. |
| [getOrientation()](#getOrientation--) | Représente l’orientation d’impression de la page. |
| [getPaperHeight()](#getPaperHeight--) | Récupère la hauteur du papier en pouces, considérée pour l’orientation de la page. |
| [getPaperSize()](#getPaperSize--) | Représente la taille du papier. |
| [getPaperWidth()](#getPaperWidth--) | Récupère la largeur du papier en pouces, considérée pour l’orientation de la page. |
| [getPicture(boolean isFirst, boolean isEven, boolean isHeader, int section)](#getPicture-boolean-boolean-boolean-int-) | Récupère l’objet [Picture](../../com.aspose.cells/picture) de l’en-tête / du pied de page. |
| [getPicture(boolean isHeader, int section)](#getPicture-boolean-int-) | Récupère l’objet [Picture](../../com.aspose.cells/picture) de l’en-tête / du pied de page. |
| [getPrintArea()](#getPrintArea--) | Représente la plage à imprimer. |
| [getPrintComments()](#getPrintComments--) | Représente la façon dont les commentaires sont imprimés avec la feuille. |
| [getPrintCopies()](#getPrintCopies--) | Récupère le nombre de copies à imprimer. |
| [getPrintDraft()](#getPrintDraft--) | Représente si la feuille sera imprimée sans graphiques. |
| [getPrintErrors()](#getPrintErrors--) | Spécifie le type d'erreur d'impression affichée. |
| [getPrintGridlines()](#getPrintGridlines--) | Représente si les lignes de grille des cellules sont imprimées sur la page. |
| [getPrintHeadings()](#getPrintHeadings--) | Représente si les en-têtes de lignes et de colonnes sont imprimés avec cette page. |
| [getPrintQuality()](#getPrintQuality--) | Représente la qualité d'impression. |
| [getPrintTitleColumns()](#getPrintTitleColumns--) | Représente les colonnes contenant les cellules à répéter sur le côté gauche de chaque page. |
| [getPrintTitleRows()](#getPrintTitleRows--) | Représente les lignes contenant les cellules à répéter en haut de chaque page. |
| [getPrinterSettings()](#getPrinterSettings--) | Obtient les paramètres de l'imprimante par défaut. |
| [getRightMargin()](#getRightMargin--) | Représente la taille de la marge droite, en centimètres. |
| [getRightMarginInch()](#getRightMarginInch--) | Représente la taille de la marge droite, en pouces. |
| [getTopMargin()](#getTopMargin--) | Représente la taille de la marge supérieure, en centimètres. |
| [getTopMarginInch()](#getTopMarginInch--) | Représente la taille de la marge supérieure, en pouces. |
| [getZoom()](#getZoom--) | Représente le facteur d'échelle en pourcentage. |
| [hashCode()](#hashCode--) |  |
| [isAutoFirstPageNumber()](#isAutoFirstPageNumber--) | Indique si le numéro de la première page est attribué automatiquement. |
| [isAutomaticPaperSize()](#isAutomaticPaperSize--) | Indique si la taille du papier est automatique. |
| [isHFAlignMargins()](#isHFAlignMargins--) | Indique si les marges d'en-tête et de pied de page sont alignées avec les marges de la page. |
| [isHFDiffFirst()](#isHFDiffFirst--) | Vrai signifie que l'en-tête/pied de page de la première page est différent des autres pages. |
| [isHFDiffOddEven()](#isHFDiffOddEven--) | Vrai signifie que l'en-tête/pied de page des pages impaires est différent des pages impaires. |
| [isHFScaleWithDoc()](#isHFScaleWithDoc--) | Indique si l'en-tête et le pied de page sont mis à l'échelle avec le redimensionnement du document. |
| [isPercentScale()](#isPercentScale--) | Si cette propriété est False, les propriétés FitToPagesWide et FitToPagesTall contrôlent la façon dont la feuille de calcul est mise à l'échelle. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAutoFirstPageNumber(boolean value)](#setAutoFirstPageNumber-boolean-) | Indique si le numéro de la première page est attribué automatiquement. |
| [setBlackAndWhite(boolean value)](#setBlackAndWhite-boolean-) | Indique si les éléments du document seront imprimés en noir et blanc. |
| [setBottomMargin(double value)](#setBottomMargin-double-) | Indique la taille de la marge inférieure, en centimètres. |
| [setBottomMarginInch(double value)](#setBottomMarginInch-double-) | Indique la taille de la marge inférieure, en pouces. |
| [setCenterHorizontally(boolean value)](#setCenterHorizontally-boolean-) | Indique si la feuille est imprimée centrée horizontalement. |
| [setCenterVertically(boolean value)](#setCenterVertically-boolean-) | Indique si la feuille est imprimée centrée verticalement. |
| [setEvenFooter(int section, String footerScript)](#setEvenFooter-int-java.lang.String-) | Définit un script formatant le pied de page des pages paires d'un fichier Excel. |
| [setEvenHeader(int section, String headerScript)](#setEvenHeader-int-java.lang.String-) | Définit un script formatant l'en-tête des pages paires d'un fichier Excel. |
| [setFirstPageFooter(int section, String footerScript)](#setFirstPageFooter-int-java.lang.String-) | Définit un script formatant le pied de page de la première page d'un fichier Excel. |
| [setFirstPageHeader(int section, String headerScript)](#setFirstPageHeader-int-java.lang.String-) | Définit un script formatant l'en-tête de la première page d'un fichier Excel. |
| [setFirstPageNumber(int value)](#setFirstPageNumber-int-) | Représente le numéro de la première page qui sera utilisé lors de l’impression de cette feuille. |
| [setFitToPages(int wide, int tall)](#setFitToPages-int-int-) | Définit le nombre de pages auxquelles la feuille de calcul sera mise à l'échelle lors de l'impression. |
| [setFitToPagesTall(int value)](#setFitToPagesTall-int-) | Représente le nombre de pages en hauteur auquel la feuille de calcul sera mise à l’échelle lors de l’impression. |
| [setFitToPagesWide(int value)](#setFitToPagesWide-int-) | Représente le nombre de pages en largeur auquel la feuille de calcul sera mise à l’échelle lors de l’impression. |
| [setFooter(int section, String footerScript)](#setFooter-int-java.lang.String-) | Définit un script formatant le pied de page d'un fichier Excel. |
| [setFooterMargin(double value)](#setFooterMargin-double-) | Représente la distance du bas de la page au pied de page, en centimètres. |
| [setFooterMarginInch(double value)](#setFooterMarginInch-double-) | Représente la distance du bas de la page au pied de page, en pouces. |
| [setFooterPicture(int section, byte[] footerPicture)](#setFooterPicture-int-byte---) | Définit une image dans le pied de page d'une feuille de calcul. |
| [setHFAlignMargins(boolean value)](#setHFAlignMargins-boolean-) | Indique si les marges d'en-tête et de pied de page sont alignées avec les marges de la page. |
| [setHFDiffFirst(boolean value)](#setHFDiffFirst-boolean-) | Vrai signifie que l'en-tête/pied de page de la première page est différent des autres pages. |
| [setHFDiffOddEven(boolean value)](#setHFDiffOddEven-boolean-) | Vrai signifie que l'en-tête/pied de page des pages impaires est différent des pages impaires. |
| [setHFScaleWithDoc(boolean value)](#setHFScaleWithDoc-boolean-) | Indique si l'en-tête et le pied de page sont mis à l'échelle avec le redimensionnement du document. |
| [setHeader(int section, String headerScript)](#setHeader-int-java.lang.String-) | Définit un script formatant l'en-tête d'un fichier Excel. |
| [setHeaderMargin(double value)](#setHeaderMargin-double-) | Représente la distance du haut de la page à l’en-tête, en centimètres. |
| [setHeaderMarginInch(double value)](#setHeaderMarginInch-double-) | Représente la distance du haut de la page à l’en-tête, en pouces. |
| [setHeaderPicture(int section, byte[] headerPicture)](#setHeaderPicture-int-byte---) | Définit une image dans l'en-tête d'une feuille de calcul. |
| [setLeftMargin(double value)](#setLeftMargin-double-) | Représente la taille de la marge gauche, en centimètres. |
| [setLeftMarginInch(double value)](#setLeftMarginInch-double-) | Représente la taille de la marge gauche, en pouces. |
| [setOrder(int value)](#setOrder-int-) | Représente l’ordre que Microsoft Excel utilise pour numéroter les pages lors de l’impression d’une grande feuille de calcul. |
| [setOrientation(int value)](#setOrientation-int-) | Représente l’orientation d’impression de la page. |
| [setPaperSize(int value)](#setPaperSize-int-) | Représente la taille du papier. |
| [setPercentScale(boolean value)](#setPercentScale-boolean-) | Si cette propriété est False, les propriétés FitToPagesWide et FitToPagesTall contrôlent la façon dont la feuille de calcul est mise à l'échelle. |
| [setPicture(boolean isFirst, boolean isEven, boolean isHeader, int section, byte[] imageData)](#setPicture-boolean-boolean-boolean-int-byte---) | Définit une image dans l'en-tête/le pied de page d'une feuille de calcul. |
| [setPrintArea(String value)](#setPrintArea-java.lang.String-) | Représente la plage à imprimer. |
| [setPrintComments(int value)](#setPrintComments-int-) | Représente la façon dont les commentaires sont imprimés avec la feuille. |
| [setPrintCopies(int value)](#setPrintCopies-int-) | Définit le nombre de copies à imprimer. |
| [setPrintDraft(boolean value)](#setPrintDraft-boolean-) | Représente si la feuille sera imprimée sans graphiques. |
| [setPrintErrors(int value)](#setPrintErrors-int-) | Spécifie le type d'erreur d'impression affichée. |
| [setPrintGridlines(boolean value)](#setPrintGridlines-boolean-) | Représente si les lignes de grille des cellules sont imprimées sur la page. |
| [setPrintHeadings(boolean value)](#setPrintHeadings-boolean-) | Représente si les en-têtes de lignes et de colonnes sont imprimés avec cette page. |
| [setPrintQuality(int value)](#setPrintQuality-int-) | Représente la qualité d'impression. |
| [setPrintTitleColumns(String value)](#setPrintTitleColumns-java.lang.String-) | Représente les colonnes contenant les cellules à répéter sur le côté gauche de chaque page. |
| [setPrintTitleRows(String value)](#setPrintTitleRows-java.lang.String-) | Représente les lignes contenant les cellules à répéter en haut de chaque page. |
| [setPrinterSettings(byte[] value)](#setPrinterSettings-byte---) | Définit les paramètres de l'imprimante par défaut. |
| [setRightMargin(double value)](#setRightMargin-double-) | Représente la taille de la marge droite, en centimètres. |
| [setRightMarginInch(double value)](#setRightMarginInch-double-) | Représente la taille de la marge droite, en pouces. |
| [setTopMargin(double value)](#setTopMargin-double-) | Représente la taille de la marge supérieure, en centimètres. |
| [setTopMarginInch(double value)](#setTopMarginInch-double-) | Représente la taille de la marge supérieure, en pouces. |
| [setZoom(int value)](#setZoom-int-) | Représente le facteur d'échelle en pourcentage. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### clearHeaderFooter() {#clearHeaderFooter--}
```
public void clearHeaderFooter()
```


Efface les paramètres d'en-tête et de pied de page.

### copy(PageSetup source, CopyOptions copyOptions) {#copy-com.aspose.cells.PageSetup-com.aspose.cells.CopyOptions-}
```
public void copy(PageSetup source, CopyOptions copyOptions)
```


Copie les paramètres de la configuration de page.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| source | [PageSetup](../../com.aspose.cells/pagesetup) | La source. |
| copyOptions | [CopyOptions](../../com.aspose.cells/copyoptions) | Les options de copie. |

### customPaperSize(double width, double height) {#customPaperSize-double-double-}
```
public void customPaperSize(double width, double height)
```


Définit la taille du papier personnalisée, en pouces.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| largeur | double | La largeur du papier. |
| hauteur | double | La hauteur du papier. |

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
### getBlackAndWhite() {#getBlackAndWhite--}
```
public boolean getBlackAndWhite()
```


Indique si les éléments du document seront imprimés en noir et blanc.

**Returns:**
boolean
### getBottomMargin() {#getBottomMargin--}
```
public double getBottomMargin()
```


Indique la taille de la marge inférieure, en centimètres.

**Returns:**
double
### getBottomMarginInch() {#getBottomMarginInch--}
```
public double getBottomMarginInch()
```


Indique la taille de la marge inférieure, en pouces.

**Returns:**
double
### getCenterHorizontally() {#getCenterHorizontally--}
```
public boolean getCenterHorizontally()
```


Indique si la feuille est imprimée centrée horizontalement.

**Returns:**
boolean
### getCenterVertically() {#getCenterVertically--}
```
public boolean getCenterVertically()
```


Indique si la feuille est imprimée centrée verticalement.

**Returns:**
boolean
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getCommands(String headerFooterScript) {#getCommands-java.lang.String-}
```
public HeaderFooterCommand[] getCommands(String headerFooterScript)
```


Récupère toutes les commandes d’en-tête ou de pied de page.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| headerFooterScript | java.lang.String | Le script d'en-tête/pied de page |

**Returns:**
com.aspose.cells.HeaderFooterCommand[] - Retourne toutes les commandes d'en-tête ou de pied de page.
### getEvenFooter(int section) {#getEvenFooter-int-}
```
public String getEvenFooter(int section)
```


Récupère un script formatant le pied de page pair d’un fichier Excel.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| section | int | 0: Section gauche, 1: Section centrale, 2: Section droite. |

**Returns:**
java.lang.String
### getEvenHeader(int section) {#getEvenHeader-int-}
```
public String getEvenHeader(int section)
```


Récupère un script formatant l’en-tête pair d’un fichier Excel.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| section | int | 0: Section gauche, 1: Section centrale, 2: Section droite. |

**Returns:**
java.lang.String
### getFirstPageFooter(int section) {#getFirstPageFooter-int-}
```
public String getFirstPageFooter(int section)
```


Récupère un script formatant le pied de page de la première page d’un fichier Excel.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| section | int | 0: Section gauche, 1: Section centrale, 2: Section droite. |

**Returns:**
java.lang.String
### getFirstPageHeader(int section) {#getFirstPageHeader-int-}
```
public String getFirstPageHeader(int section)
```


Récupère un script formatant l’en-tête de la première page d’un fichier Excel.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| section | int | 0: Section gauche, 1: Section centrale, 2: Section droite. |

**Returns:**
java.lang.String
### getFirstPageNumber() {#getFirstPageNumber--}
```
public int getFirstPageNumber()
```


Représente le numéro de la première page qui sera utilisé lors de l’impression de cette feuille.

**Returns:**
int
### getFitToPagesTall() {#getFitToPagesTall--}
```
public int getFitToPagesTall()
```


Représente le nombre de pages en hauteur auquel la feuille de calcul sera mise à l'échelle lors de l'impression. La valeur par défaut est 1.

**Remarks**

Vous devez définir FitToPagesWide à zéro si vous souhaitez faire tenir toutes les lignes sur une page.

**Returns:**
int
### getFitToPagesWide() {#getFitToPagesWide--}
```
public int getFitToPagesWide()
```


Représente le nombre de pages en largeur auquel la feuille de calcul sera mise à l'échelle lors de l'impression. La valeur par défaut est 1.

**Remarks**

Vous devez définir FitToPagesTall à zéro si vous souhaitez faire tenir toutes les colonnes sur une page.

**Returns:**
int
### getFooter(int section) {#getFooter-int-}
```
public String getFooter(int section)
```


Récupère un script formatant le pied de page d’un fichier Excel.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| section | int | 0: Section gauche, 1: Section centrale, 2: Section droite. |

**Returns:**
java.lang.String
### getFooterMargin() {#getFooterMargin--}
```
public double getFooterMargin()
```


Représente la distance du bas de la page au pied de page, en centimètres.

**Returns:**
double
### getFooterMarginInch() {#getFooterMarginInch--}
```
public double getFooterMarginInch()
```


Représente la distance du bas de la page au pied de page, en pouces.

**Returns:**
double
### getHeader(int section) {#getHeader-int-}
```
public String getHeader(int section)
```


Récupère un script formatant l’en-tête d’un fichier Excel.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| section | int | 0: Section gauche, 1: Section centrale, 2: Section droite. |

**Returns:**
java.lang.String
### getHeaderMargin() {#getHeaderMargin--}
```
public double getHeaderMargin()
```


Représente la distance du haut de la page à l’en-tête, en centimètres.

**Returns:**
double
### getHeaderMarginInch() {#getHeaderMarginInch--}
```
public double getHeaderMarginInch()
```


Représente la distance du haut de la page à l’en-tête, en pouces.

**Returns:**
double
### getLeftMargin() {#getLeftMargin--}
```
public double getLeftMargin()
```


Représente la taille de la marge gauche, en centimètres.

**Returns:**
double
### getLeftMarginInch() {#getLeftMarginInch--}
```
public double getLeftMarginInch()
```


Représente la taille de la marge gauche, en pouces.

**Returns:**
double
### getODSPageBackground() {#getODSPageBackground--}
```
public OdsPageBackground getODSPageBackground()
```


Récupère l’arrière-plan d’ODS.

**Returns:**
[OdsPageBackground](../../com.aspose.cells/odspagebackground)
### getOrder() {#getOrder--}
```
public int getOrder()
```


Représente l’ordre que Microsoft Excel utilise pour numéroter les pages lors de l’impression d’une grande feuille de calcul.

Voir [PrintOrderType](../../com.aspose.cells/printordertype).

**Returns:**
int
### getOrientation() {#getOrientation--}
```
public int getOrientation()
```


Représente l’orientation d’impression de la page.

Voir [PageOrientationType](../../com.aspose.cells/pageorientationtype).

**Returns:**
int
### getPaperHeight() {#getPaperHeight--}
```
public double getPaperHeight()
```


Récupère la hauteur du papier en pouces, considérée pour l’orientation de la page.

**Returns:**
double
### getPaperSize() {#getPaperSize--}
```
public int getPaperSize()
```


Représente la taille du papier.

Voir [PaperSizeType](../../com.aspose.cells/papersizetype).

**Returns:**
int
### getPaperWidth() {#getPaperWidth--}
```
public double getPaperWidth()
```


Récupère la largeur du papier en pouces, considérée pour l’orientation de la page.

**Returns:**
double
### getPicture(boolean isFirst, boolean isEven, boolean isHeader, int section) {#getPicture-boolean-boolean-boolean-int-}
```
public Picture getPicture(boolean isFirst, boolean isEven, boolean isHeader, int section)
```


Récupère l’objet [Picture](../../com.aspose.cells/picture) de l’en-tête / du pied de page.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| isFirst | boolean | Indique si l'on récupère l'image de l'en-tête/pied de page de la première page. |
| isEven | boolean | Indique si l'on récupère l'image de l'en-tête/pied de page des pages paires. |
| isHeader | boolean | Indique si l'image d'en-tête/pied de page est obtenue. |
| section | int | 0: Section gauche, 1: Section centrale, 2: Section droite. |

**Returns:**
[Picture](../../com.aspose.cells/picture) - Returns [Picture](../../com.aspose.cells/picture) object.
### getPicture(boolean isHeader, int section) {#getPicture-boolean-int-}
```
public Picture getPicture(boolean isHeader, int section)
```


Récupère l’objet [Picture](../../com.aspose.cells/picture) de l’en-tête / du pied de page.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| isHeader | boolean | Indique s'il se trouve dans l'en-tête ou le pied de page. |
| section | int | 0: Section gauche, 1: Section centrale, 2: Section droite. |

**Returns:**
[Picture](../../com.aspose.cells/picture) - Returns [Picture](../../com.aspose.cells/picture) object. Returns null if there is no picture.
### getPrintArea() {#getPrintArea--}
```
public String getPrintArea()
```


Représente la plage à imprimer.

**Returns:**
java.lang.String
### getPrintComments() {#getPrintComments--}
```
public int getPrintComments()
```


Représente la façon dont les commentaires sont imprimés avec la feuille.

Voir [PrintCommentsType](../../com.aspose.cells/printcommentstype).

**Returns:**
int
### getPrintCopies() {#getPrintCopies--}
```
public int getPrintCopies()
```


Récupère le nombre de copies à imprimer.

**Returns:**
int
### getPrintDraft() {#getPrintDraft--}
```
public boolean getPrintDraft()
```


Représente si la feuille sera imprimée sans graphiques.

**Returns:**
boolean
### getPrintErrors() {#getPrintErrors--}
```
public int getPrintErrors()
```


Spécifie le type d'erreur d'impression affichée.

Voir [PrintErrorsType](../../com.aspose.cells/printerrorstype).

**Returns:**
int
### getPrintGridlines() {#getPrintGridlines--}
```
public boolean getPrintGridlines()
```


Représente si les lignes de grille des cellules sont imprimées sur la page.

**Returns:**
boolean
### getPrintHeadings() {#getPrintHeadings--}
```
public boolean getPrintHeadings()
```


Représente si les en-têtes de lignes et de colonnes sont imprimés avec cette page.

**Returns:**
boolean
### getPrintQuality() {#getPrintQuality--}
```
public int getPrintQuality()
```


Représente la qualité d'impression.

**Returns:**
int
### getPrintTitleColumns() {#getPrintTitleColumns--}
```
public String getPrintTitleColumns()
```


Représente les colonnes contenant les cellules à répéter sur le côté gauche de chaque page.

**Example**

```
         pageSetup.setPrintTitleColumns("$A:$A");
```

**Returns:**
java.lang.String
### getPrintTitleRows() {#getPrintTitleRows--}
```
public String getPrintTitleRows()
```


Représente les lignes contenant les cellules à répéter en haut de chaque page.

**Example**

```
         pageSetup.setPrintTitleRows("$1:$1");
```

**Returns:**
java.lang.String
### getPrinterSettings() {#getPrinterSettings--}
```
public byte[] getPrinterSettings()
```


Obtient les paramètres de l'imprimante par défaut.

**Returns:**
byte[]
### getRightMargin() {#getRightMargin--}
```
public double getRightMargin()
```


Représente la taille de la marge droite, en centimètres.

**Returns:**
double
### getRightMarginInch() {#getRightMarginInch--}
```
public double getRightMarginInch()
```


Représente la taille de la marge droite, en pouces.

**Returns:**
double
### getTopMargin() {#getTopMargin--}
```
public double getTopMargin()
```


Représente la taille de la marge supérieure, en centimètres.

**Returns:**
double
### getTopMarginInch() {#getTopMarginInch--}
```
public double getTopMarginInch()
```


Représente la taille de la marge supérieure, en pouces.

**Returns:**
double
### getZoom() {#getZoom--}
```
public int getZoom()
```


Représente le facteur d'échelle en pourcentage. Il doit être compris entre 10 et 400.

**Returns:**
int
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isAutoFirstPageNumber() {#isAutoFirstPageNumber--}
```
public boolean isAutoFirstPageNumber()
```


Indique si le numéro de la première page est attribué automatiquement.

**Returns:**
boolean
### isAutomaticPaperSize() {#isAutomaticPaperSize--}
```
public boolean isAutomaticPaperSize()
```


Indique si la taille du papier est automatique.

**Returns:**
boolean
### isHFAlignMargins() {#isHFAlignMargins--}
```
public boolean isHFAlignMargins()
```


Indique si les marges d'en-tête et de pied de page sont alignées avec les marges de la page. Si cette propriété est vraie, l'en-tête et le pied de page gauche seront alignés avec la marge gauche, et l'en-tête et le pied de page droit seront alignés avec la marge droite. Cette option est activée par défaut.

**Returns:**
boolean
### isHFDiffFirst() {#isHFDiffFirst--}
```
public boolean isHFDiffFirst()
```


Vrai signifie que l'en-tête/pied de page de la première page est différent des autres pages.

**Returns:**
boolean
### isHFDiffOddEven() {#isHFDiffOddEven--}
```
public boolean isHFDiffOddEven()
```


Vrai signifie que l'en-tête/pied de page des pages impaires est différent des pages impaires.

**Returns:**
boolean
### isHFScaleWithDoc() {#isHFScaleWithDoc--}
```
public boolean isHFScaleWithDoc()
```


Indique si l'en-tête et le pied de page sont mis à l'échelle avec le redimensionnement du document. S'applique uniquement à Excel 2007.

**Returns:**
boolean
### isPercentScale() {#isPercentScale--}
```
public boolean isPercentScale()
```


Si cette propriété est False, les propriétés FitToPagesWide et FitToPagesTall contrôlent la façon dont la feuille de calcul est mise à l'échelle.

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




### setAutoFirstPageNumber(boolean value) {#setAutoFirstPageNumber-boolean-}
```
public void setAutoFirstPageNumber(boolean value)
```


Indique si le numéro de la première page est attribué automatiquement.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setBlackAndWhite(boolean value) {#setBlackAndWhite-boolean-}
```
public void setBlackAndWhite(boolean value)
```


Indique si les éléments du document seront imprimés en noir et blanc.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setBottomMargin(double value) {#setBottomMargin-double-}
```
public void setBottomMargin(double value)
```


Indique la taille de la marge inférieure, en centimètres.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | double |  |

### setBottomMarginInch(double value) {#setBottomMarginInch-double-}
```
public void setBottomMarginInch(double value)
```


Indique la taille de la marge inférieure, en pouces.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | double |  |

### setCenterHorizontally(boolean value) {#setCenterHorizontally-boolean-}
```
public void setCenterHorizontally(boolean value)
```


Indique si la feuille est imprimée centrée horizontalement.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setCenterVertically(boolean value) {#setCenterVertically-boolean-}
```
public void setCenterVertically(boolean value)
```


Indique si la feuille est imprimée centrée verticalement.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setEvenFooter(int section, String footerScript) {#setEvenFooter-int-java.lang.String-}
```
public void setEvenFooter(int section, String footerScript)
```


Définit un script formatant le pied de page des pages paires d'un fichier Excel. N'a d'effet dans Excel 2007 que lorsque IsHFDiffOddEven est vrai.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| section | int | 0: Section gauche, 1: Section centrale, 2: Section droite. |
| footerScript | java.lang.String | Script de format du pied de page. |

### setEvenHeader(int section, String headerScript) {#setEvenHeader-int-java.lang.String-}
```
public void setEvenHeader(int section, String headerScript)
```


Définit un script formatant l'en-tête des pages paires d'un fichier Excel. N'a d'effet dans Excel 2007 que lorsque IsHFDiffOddEven est vrai.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| section | int | 0: Section gauche, 1: Section centrale, 2: Section droite. |
| headerScript | java.lang.String | Script de format de l'en-tête. |

### setFirstPageFooter(int section, String footerScript) {#setFirstPageFooter-int-java.lang.String-}
```
public void setFirstPageFooter(int section, String footerScript)
```


Définit un script formatant le pied de page de la première page d'un fichier Excel.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| section | int | 0: Section gauche, 1: Section centrale, 2: Section droite. |
| footerScript | java.lang.String | Script de format du pied de page. |

### setFirstPageHeader(int section, String headerScript) {#setFirstPageHeader-int-java.lang.String-}
```
public void setFirstPageHeader(int section, String headerScript)
```


Définit un script formatant l'en-tête de la première page d'un fichier Excel. N'a d'effet dans Excel 2007 que lorsque IsHFDiffFirst est vrai.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| section | int | 0: Section gauche, 1: Section centrale, 2: Section droite. |
| headerScript | java.lang.String | Script de format de l'en-tête. |

### setFirstPageNumber(int value) {#setFirstPageNumber-int-}
```
public void setFirstPageNumber(int value)
```


Représente le numéro de la première page qui sera utilisé lors de l’impression de cette feuille.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setFitToPages(int wide, int tall) {#setFitToPages-int-int-}
```
public void setFitToPages(int wide, int tall)
```


Définit le nombre de pages auxquelles la feuille de calcul sera mise à l'échelle lors de l'impression.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| large | int | Pages en largeur. |
| haut | int | Pages en hauteur. |

### setFitToPagesTall(int value) {#setFitToPagesTall-int-}
```
public void setFitToPagesTall(int value)
```


Représente le nombre de pages en hauteur auquel la feuille de calcul sera mise à l'échelle lors de l'impression. La valeur par défaut est 1.

**Remarks**

Vous devez définir FitToPagesWide à zéro si vous souhaitez faire tenir toutes les lignes sur une page.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setFitToPagesWide(int value) {#setFitToPagesWide-int-}
```
public void setFitToPagesWide(int value)
```


Représente le nombre de pages en largeur auquel la feuille de calcul sera mise à l'échelle lors de l'impression. La valeur par défaut est 1.

**Remarks**

Vous devez définir FitToPagesTall à zéro si vous souhaitez faire tenir toutes les colonnes sur une page.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setFooter(int section, String footerScript) {#setFooter-int-java.lang.String-}
```
public void setFooter(int section, String footerScript)
```


Définit un script formatant le pied de page d'un fichier Excel.

**Remarks**

Commandes du script:

| Commande | Description |
| -------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------- |
| &P | Numéro de page actuel\u9286\u20ac |
| &N | Nombre de pages\u9286\u20ac |
| &D | Date actuelle\u9286\u20ac |
| &T | Heure actuelle |
| &A | Nom de la feuille |
| &F | Nom de fichier sans le chemin |
| &"<FontName>" | Nom de police, par exemple : &"Arial" |
| &"<FontName>, <FontStyle>" | Nom de police et style de police, par exemple : &"Arial,Bold" |
| &<FontSize> | Taille de police. Si cette commande est suivie d’un nombre simple à imprimer dans l’en-tête, il sera séparé de la hauteur de police par un caractère d’espace. |
| &K<RRGGBB> | Couleur de police, par exemple (ROUGE) : &KFF0000 |
| &G | Script d'image |

Par exemple : "&Arial,Bold&8Footer Note"

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| section | int | 0: Section gauche, 1: Section centrale, 2: Section droite. |
| footerScript | java.lang.String | Script de format du pied de page. |

### setFooterMargin(double value) {#setFooterMargin-double-}
```
public void setFooterMargin(double value)
```


Représente la distance du bas de la page au pied de page, en centimètres.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | double |  |

### setFooterMarginInch(double value) {#setFooterMarginInch-double-}
```
public void setFooterMarginInch(double value)
```


Représente la distance du bas de la page au pied de page, en pouces.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | double |  |

### setFooterPicture(int section, byte[] footerPicture) {#setFooterPicture-int-byte---}
```
public Picture setFooterPicture(int section, byte[] footerPicture)
```


Définit une image dans le pied de page d'une feuille de calcul.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| section | int | 0: Section gauche, 1: Section centrale, 2: Section droite. |
| footerPicture | byte[] | Données d'image. |

**Returns:**
[Picture](../../com.aspose.cells/picture) - Returns [Picture](../../com.aspose.cells/picture) object.
### setHFAlignMargins(boolean value) {#setHFAlignMargins-boolean-}
```
public void setHFAlignMargins(boolean value)
```


Indique si les marges d'en-tête et de pied de page sont alignées avec les marges de la page. Si cette propriété est vraie, l'en-tête et le pied de page gauche seront alignés avec la marge gauche, et l'en-tête et le pied de page droit seront alignés avec la marge droite. Cette option est activée par défaut.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setHFDiffFirst(boolean value) {#setHFDiffFirst-boolean-}
```
public void setHFDiffFirst(boolean value)
```


Vrai signifie que l'en-tête/pied de page de la première page est différent des autres pages.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setHFDiffOddEven(boolean value) {#setHFDiffOddEven-boolean-}
```
public void setHFDiffOddEven(boolean value)
```


Vrai signifie que l'en-tête/pied de page des pages impaires est différent des pages impaires.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setHFScaleWithDoc(boolean value) {#setHFScaleWithDoc-boolean-}
```
public void setHFScaleWithDoc(boolean value)
```


Indique si l'en-tête et le pied de page sont mis à l'échelle avec le redimensionnement du document. S'applique uniquement à Excel 2007.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setHeader(int section, String headerScript) {#setHeader-int-java.lang.String-}
```
public void setHeader(int section, String headerScript)
```


Définit un script formatant l'en-tête d'un fichier Excel.

**Remarks**

Commandes du script:

| Commande | Description |
| -------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------- |
| &P | Numéro de page actuel\u9286\u20ac |
| &N | Nombre de pages\u9286\u20ac |
| &D | Date actuelle\u9286\u20ac |
| &T | Heure actuelle |
| &A | Nom de la feuille |
| &F | Nom de fichier sans le chemin |
| &"<FontName>" | Nom de police, par exemple : &"Arial" |
| &"<FontName>, <FontStyle>" | Nom de police et style de police, par exemple : &"Arial,Bold" |
| &<FontSize> | Taille de police. Si cette commande est suivie d’un nombre simple à imprimer dans l’en-tête, il sera séparé de la hauteur de police par un caractère d’espace. |
| &K<RRGGBB> | Couleur de police, par exemple (ROUGE) : &KFF0000 |
| &G | Script d'image |

Par exemple : "&Arial,Bold&8Header Note"

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| section | int | 0: Section gauche, 1: Section centrale, 2: Section droite. |
| headerScript | java.lang.String | Script de format de l'en-tête. |

### setHeaderMargin(double value) {#setHeaderMargin-double-}
```
public void setHeaderMargin(double value)
```


Représente la distance du haut de la page à l’en-tête, en centimètres.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | double |  |

### setHeaderMarginInch(double value) {#setHeaderMarginInch-double-}
```
public void setHeaderMarginInch(double value)
```


Représente la distance du haut de la page à l’en-tête, en pouces.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | double |  |

### setHeaderPicture(int section, byte[] headerPicture) {#setHeaderPicture-int-byte---}
```
public Picture setHeaderPicture(int section, byte[] headerPicture)
```


Définit une image dans l'en-tête d'une feuille de calcul.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| section | int | 0: Section gauche, 1: Section centrale, 2: Section droite. |
| headerPicture | byte[] | Données d'image. |

**Returns:**
[Picture](../../com.aspose.cells/picture) - Returns [Picture](../../com.aspose.cells/picture) object.
### setLeftMargin(double value) {#setLeftMargin-double-}
```
public void setLeftMargin(double value)
```


Représente la taille de la marge gauche, en centimètres.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | double |  |

### setLeftMarginInch(double value) {#setLeftMarginInch-double-}
```
public void setLeftMarginInch(double value)
```


Représente la taille de la marge gauche, en pouces.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | double |  |

### setOrder(int value) {#setOrder-int-}
```
public void setOrder(int value)
```


Représente l’ordre que Microsoft Excel utilise pour numéroter les pages lors de l’impression d’une grande feuille de calcul.

Voir [PrintOrderType](../../com.aspose.cells/printordertype).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setOrientation(int value) {#setOrientation-int-}
```
public void setOrientation(int value)
```


Représente l’orientation d’impression de la page.

Voir [PageOrientationType](../../com.aspose.cells/pageorientationtype).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setPaperSize(int value) {#setPaperSize-int-}
```
public void setPaperSize(int value)
```


Représente la taille du papier.

Voir [PaperSizeType](../../com.aspose.cells/papersizetype).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setPercentScale(boolean value) {#setPercentScale-boolean-}
```
public void setPercentScale(boolean value)
```


Si cette propriété est False, les propriétés FitToPagesWide et FitToPagesTall contrôlent la façon dont la feuille de calcul est mise à l'échelle.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setPicture(boolean isFirst, boolean isEven, boolean isHeader, int section, byte[] imageData) {#setPicture-boolean-boolean-boolean-int-byte---}
```
public Picture setPicture(boolean isFirst, boolean isEven, boolean isHeader, int section, byte[] imageData)
```


Définit une image dans l'en-tête/le pied de page d'une feuille de calcul.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| isFirst | boolean | Indique si la configuration de l’image d’en-tête/pied de page de la première page. |
| isEven | boolean | Indique si la configuration de l’image d’en-tête/pied de page des pages paires. |
| isHeader | boolean | Indique si la configuration de l’image d’en-tête/pied de page. |
| section | int | 0: Section gauche, 1: Section centrale, 2: Section droite. |
| imageData | byte[] | Données d'image. |

**Returns:**
[Picture](../../com.aspose.cells/picture) - Returns [Picture](../../com.aspose.cells/picture) object.
### setPrintArea(String value) {#setPrintArea-java.lang.String-}
```
public void setPrintArea(String value)
```


Représente la plage à imprimer.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

### setPrintComments(int value) {#setPrintComments-int-}
```
public void setPrintComments(int value)
```


Représente la façon dont les commentaires sont imprimés avec la feuille.

Voir [PrintCommentsType](../../com.aspose.cells/printcommentstype).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setPrintCopies(int value) {#setPrintCopies-int-}
```
public void setPrintCopies(int value)
```


Définit le nombre de copies à imprimer.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setPrintDraft(boolean value) {#setPrintDraft-boolean-}
```
public void setPrintDraft(boolean value)
```


Représente si la feuille sera imprimée sans graphiques.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setPrintErrors(int value) {#setPrintErrors-int-}
```
public void setPrintErrors(int value)
```


Spécifie le type d'erreur d'impression affichée.

Voir [PrintErrorsType](../../com.aspose.cells/printerrorstype).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setPrintGridlines(boolean value) {#setPrintGridlines-boolean-}
```
public void setPrintGridlines(boolean value)
```


Représente si les lignes de grille des cellules sont imprimées sur la page.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setPrintHeadings(boolean value) {#setPrintHeadings-boolean-}
```
public void setPrintHeadings(boolean value)
```


Représente si les en-têtes de lignes et de colonnes sont imprimés avec cette page.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setPrintQuality(int value) {#setPrintQuality-int-}
```
public void setPrintQuality(int value)
```


Représente la qualité d'impression.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setPrintTitleColumns(String value) {#setPrintTitleColumns-java.lang.String-}
```
public void setPrintTitleColumns(String value)
```


Représente les colonnes contenant les cellules à répéter sur le côté gauche de chaque page.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

### setPrintTitleRows(String value) {#setPrintTitleRows-java.lang.String-}
```
public void setPrintTitleRows(String value)
```


Représente les lignes contenant les cellules à répéter en haut de chaque page.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

### setPrinterSettings(byte[] value) {#setPrinterSettings-byte---}
```
public void setPrinterSettings(byte[] value)
```


Définit les paramètres de l'imprimante par défaut.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | byte[] |  |

### setRightMargin(double value) {#setRightMargin-double-}
```
public void setRightMargin(double value)
```


Représente la taille de la marge droite, en centimètres.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | double |  |

### setRightMarginInch(double value) {#setRightMarginInch-double-}
```
public void setRightMarginInch(double value)
```


Représente la taille de la marge droite, en pouces.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | double |  |

### setTopMargin(double value) {#setTopMargin-double-}
```
public void setTopMargin(double value)
```


Représente la taille de la marge supérieure, en centimètres.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | double |  |

### setTopMarginInch(double value) {#setTopMarginInch-double-}
```
public void setTopMarginInch(double value)
```


Représente la taille de la marge supérieure, en pouces.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | double |  |

### setZoom(int value) {#setZoom-int-}
```
public void setZoom(int value)
```


Représente le facteur d'échelle en pourcentage. Il doit être compris entre 10 et 400.

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

