---
title: "WorkbookRender"
second_title: "Référence API d'Aspose.Cells pour Java"
description: "Représente un rendu de classeur."
type: docs
url: /fr/java/com.aspose.cells/workbookrender/
---

**Inheritance:**
java.lang.Object
```
public class WorkbookRender
```

Représente un rendu de Workbook. Le constructeur de cette classe doit être utilisé après la modification de la configuration de page, du style de cellule.

**Remarks**
## Constructeurs

| Constructeur | Description |
| --- | --- |
| [WorkbookRender(Workbook workbook, ImageOrPrintOptions options)](#WorkbookRender-com.aspose.cells.Workbook-com.aspose.cells.ImageOrPrintOptions-) | Le constructeur de WorkbookRender |
## Méthodes

| Méthode | Description |
| --- | --- |
| [dispose()](#dispose--) | Libère les ressources créées et utilisées pour le rendu. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getPageCount()](#getPageCount--) | Obtient le nombre total de pages du classeur. |
| [getPageSizeInch(int pageIndex)](#getPageSizeInch-int-) | Obtient la taille de la page en pouces de l'image de sortie. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [toImage(int pageIndex, InputStream stream)](#toImage-int-java.io.InputStream-) | Rend une page donnée vers un flux. |
| [toImage(int pageIndex, OutputStream stream)](#toImage-int-java.io.OutputStream-) | Rend une page donnée vers un flux. |
| [toImage(int pageIndex, String fileName)](#toImage-int-java.lang.String-) | Rend une page donnée vers un fichier. |
| [toImage(OutputStream stream)](#toImage-java.io.OutputStream-) | Rend l'ensemble du classeur en image Tiff vers un flux. |
| [toImage(String filename)](#toImage-java.lang.String-) | Rend l'ensemble du classeur en image Tiff vers un fichier. |
| [toPrinter(String printerName)](#toPrinter-java.lang.String-) | Rend le classeur vers l'imprimante |
| [toPrinter(String printerName, int printPageIndex, int printPageCount)](#toPrinter-java.lang.String-int-int-) | Rend le classeur vers l'imprimante |
| [toPrinter(String printerName, String jobName)](#toPrinter-java.lang.String-java.lang.String-) | Rend le classeur vers l'imprimante |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### WorkbookRender(Workbook workbook, ImageOrPrintOptions options) {#WorkbookRender-com.aspose.cells.Workbook-com.aspose.cells.ImageOrPrintOptions-}
```
public WorkbookRender(Workbook workbook, ImageOrPrintOptions options)
```


Le constructeur de WorkbookRender

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| workbook | [Workbook](../../com.aspose.cells/workbook) | Indique quel classeur doit être rendu. |
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


Obtient le nombre total de pages du classeur.

**Returns:**
int
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

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| pageIndex | int | indique quelle page doit être convertie |
| fileName | java.lang.String | nom de fichier de l'image de sortie |

### toImage(OutputStream stream) {#toImage-java.io.OutputStream-}
```
public void toImage(OutputStream stream)
```


Rend l'ensemble du classeur en image Tiff vers un flux.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| stream | java.io.OutputStream | le flux de l'image de sortie |

### toImage(String filename) {#toImage-java.lang.String-}
```
public void toImage(String filename)
```


Rend l'ensemble du classeur en image Tiff vers un fichier.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| nom de fichier | java.lang.String | le nom de fichier de l'image de sortie |

### toPrinter(String printerName) {#toPrinter-java.lang.String-}
```
public void toPrinter(String printerName)
```


Rend le classeur vers l'imprimante

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| printerName | java.lang.String | le nom de l'imprimante, par exemple : "Microsoft Office Document Image Writer" |

### toPrinter(String printerName, int printPageIndex, int printPageCount) {#toPrinter-java.lang.String-int-int-}
```
public void toPrinter(String printerName, int printPageIndex, int printPageCount)
```


Rend le classeur vers l'imprimante

**Remarks**

NOTE : Cette méthode est maintenant obsolète. À la place, veuillez utiliser ToPrinter(string PrinterName) et ImageOrPrintOptions.PageIndex, PageCount pour définir la première page et le nombre de pages à imprimer. Cette propriété sera supprimée 12 mois plus tard, depuis décembre 2021. Aspose s'excuse pour tout désagrément que vous auriez pu rencontrer.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| printerName | java.lang.String | le nom de l'imprimante, par exemple : "Microsoft Office Document Image Writer" |
| printPageIndex | int | l'index basé sur zéro de la première page à imprimer, il doit être dans la plage [0, WorkbookRender.PageCount-1] |
| printPageCount | int | le nombre de pages à imprimer, il doit être supérieur à zéro |

### toPrinter(String printerName, String jobName) {#toPrinter-java.lang.String-java.lang.String-}
```
public void toPrinter(String printerName, String jobName)
```


Rend le classeur vers l'imprimante

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

