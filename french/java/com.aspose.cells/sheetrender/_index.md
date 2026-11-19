---
title: "SheetRender"
second_title: "Référence API d'Aspose.Cells pour Java"
description: "Représente un rendu de feuille de calcul qui peut rendre la feuille de calcul en diverses images telles que BMP PNG JPEG TIFF.."
type: docs
url: /fr/java/com.aspose.cells/sheetrender/
---

**Inheritance:**
java.lang.Object
```
public class SheetRender
```

Représente un rendu de feuille de calcul qui peut rendre la feuille de calcul en diverses images telles que (BMP, PNG, JPEG, TIFF..) Le constructeur de cette classe doit être utilisé après la modification de la configuration de page, du style de cellule.
## Constructeurs

| Constructeur | Description |
| --- | --- |
| [SheetRender(Worksheet worksheet, ImageOrPrintOptions options)](#SheetRender-com.aspose.cells.Worksheet-com.aspose.cells.ImageOrPrintOptions-) | la construction de SheetRender, nécessite une feuille de calcul et ImageOrPrintOptions comme paramètres |
## Méthodes

| Méthode | Description |
| --- | --- |
| [dispose()](#dispose--) | Libère les ressources créées et utilisées pour le rendu. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getPageCount()](#getPageCount--) | Obtient le nombre total de pages de la feuille de calcul actuelle. |
| [getPageScale()](#getPageScale--) | Obtient l'échelle de page calculée de la feuille. |
| [getPageSizeInch(int pageIndex)](#getPageSizeInch-int-) | Obtient la taille de la page en pouces de l'image de sortie. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [toImage(int pageIndex, InputStream stream)](#toImage-int-java.io.InputStream-) | Rend une page donnée vers un flux. |
| [toImage(int pageIndex, OutputStream stream)](#toImage-int-java.io.OutputStream-) | Rend une page donnée vers un flux. |
| [toImage(int pageIndex, String fileName)](#toImage-int-java.lang.String-) | Rend une page donnée vers un fichier. |
| [toPrinter(String printerName)](#toPrinter-java.lang.String-) | Rendre la feuille de calcul vers l'imprimante |
| [toPrinter(String printerName, int printPageIndex, int printPageCount)](#toPrinter-java.lang.String-int-int-) | Rendre la feuille de calcul vers l'imprimante |
| [toPrinter(String printerName, String jobName)](#toPrinter-java.lang.String-java.lang.String-) | Rendre la feuille de calcul vers l'imprimante |
| [toString()](#toString--) |  |
| [toTiff(InputStream stream)](#toTiff-java.io.InputStream-) | Rendre toute la feuille de calcul en image Tiff vers le flux. |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### SheetRender(Worksheet worksheet, ImageOrPrintOptions options) {#SheetRender-com.aspose.cells.Worksheet-com.aspose.cells.ImageOrPrintOptions-}
```
public SheetRender(Worksheet worksheet, ImageOrPrintOptions options)
```


la construction de SheetRender, nécessite une feuille de calcul et ImageOrPrintOptions comme paramètres

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| worksheet | [Worksheet](../../com.aspose.cells/worksheet) | Indique quelle feuille de calcul doit être rendue. |
| options | [ImageOrPrintOptions](../../com.aspose.cells/imageorprintoptions) | ImageOrPrintOptions contient certaines propriétés de l'image de sortie |

### dispose() {#dispose--}
```
public void dispose()
```


Libère les ressources créées et utilisées pour le rendu.

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
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getPageCount() {#getPageCount--}
```
public int getPageCount()
```


Obtient le nombre total de pages de la feuille de calcul actuelle.

**Returns:**
int
### getPageScale() {#getPageScale--}
```
public double getPageScale()
```


Obtient l'échelle de page calculée de la feuille. Retourne l'échelle définie si [PageSetup.getZoom()](../../com.aspose.cells/pagesetup\#getZoom--) est définie. Sinon, retourne l'échelle calculée selon [PageSetup.getFitToPagesWide()](../../com.aspose.cells/pagesetup\#getFitToPagesWide--) et [PageSetup.getFitToPagesTall()](../../com.aspose.cells/pagesetup\#getFitToPagesTall--).

**Example**

```
         Workbook wb = new Workbook("Book1.xlsx");
 
         SheetRender sheetRender = new SheetRender(wb.getWorksheets().get(0), new ImageOrPrintOptions());
 
         //Gets calculated page scale of the sheet.
         double pageScale = sheetRender.getPageScale();
```

**Returns:**
double
### getPageSizeInch(int pageIndex) {#getPageSizeInch-int-}
```
public float[] getPageSizeInch(int pageIndex)
```


Obtient la taille de la page en pouces de l'image de sortie.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| pageIndex | int | L'index de page commence à zéro. |

**Returns:**
float[] - Taille de la page de l'image, [0] pour la largeur et [1] pour la hauteur
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




### toImage(int pageIndex, InputStream stream) {#toImage-int-java.io.InputStream-}
```
public void toImage(int pageIndex, InputStream stream)
```


Rend une page donnée vers un flux.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| pageIndex | int | indique quelle page doit être convertie |
| stream | java.io.InputStream | le flux de l'image de sortie |

### toImage(int pageIndex, OutputStream stream) {#toImage-int-java.io.OutputStream-}
```
public void toImage(int pageIndex, OutputStream stream)
```


Rend une page donnée vers un flux.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| pageIndex | int | indique quelle page doit être convertie |
| stream | java.io.OutputStream | le flux de l'image de sortie |

### toImage(int pageIndex, String fileName) {#toImage-int-java.lang.String-}
```
public void toImage(int pageIndex, String fileName)
```


Rend une page donnée vers un fichier.

**Example**

Le code suivant génère la première page de la première feuille en image png.

```
         //load the source file with images.
         Workbook wb = new Workbook("Book1.xlsx");
 
         ImageOrPrintOptions imgOpt = new ImageOrPrintOptions();
 
         //set output image type.
         imgOpt.setImageType(ImageType.PNG);
 
         //render the first sheet.
         SheetRender sr = new SheetRender(wb.getWorksheets().get(0), imgOpt);
 
         //output the first page of the sheet to image.
         sr.toImage(0, "output.png");
```

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| pageIndex | int | indique quelle page doit être convertie |
| fileName | java.lang.String | nom de fichier de l'image de sortie |

### toPrinter(String printerName) {#toPrinter-java.lang.String-}
```
public void toPrinter(String printerName)
```


Rendre la feuille de calcul vers l'imprimante

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| printerName | java.lang.String | le nom de l'imprimante, par exemple : "Microsoft Office Document Image Writer" |

### toPrinter(String printerName, int printPageIndex, int printPageCount) {#toPrinter-java.lang.String-int-int-}
```
public void toPrinter(String printerName, int printPageIndex, int printPageCount)
```


Rendre la feuille de calcul vers l'imprimante

**Remarks**

NOTE : Cette méthode est maintenant obsolète. À la place, veuillez utiliser ToPrinter(string PrinterName) et ImageOrPrintOptions.PageIndex, PageCount pour définir la première page et le nombre de pages à imprimer. Cette propriété sera supprimée 12 mois plus tard, depuis décembre 2021. Aspose s'excuse pour tout désagrément que vous auriez pu rencontrer.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| printerName | java.lang.String | le nom de l'imprimante, par exemple : "Microsoft Office Document Image Writer" |
| printPageIndex | int | l'index basé sur 0 de la première page à imprimer, il doit être dans la plage [0, SheetRender.PageCount-1] |
| printPageCount | int | le nombre de pages à imprimer, il doit être supérieur à zéro |

### toPrinter(String printerName, String jobName) {#toPrinter-java.lang.String-java.lang.String-}
```
public void toPrinter(String printerName, String jobName)
```


Rendre la feuille de calcul vers l'imprimante

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| printerName | java.lang.String | le nom de l'imprimante, par exemple : "Microsoft Office Document Image Writer" |
| jobName | java.lang.String | définir le nom du travail d'impression |

### toString() {#toString--}
```
public String toString()
```




**Returns:**
java.lang.String
### toTiff(InputStream stream) {#toTiff-java.io.InputStream-}
```
public void toTiff(InputStream stream)
```


Rendre toute la feuille de calcul en image Tiff vers le flux.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| stream | java.io.InputStream | le flux de l'image de sortie |

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

