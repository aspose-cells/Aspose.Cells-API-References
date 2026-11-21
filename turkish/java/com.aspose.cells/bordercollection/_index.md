---
title: "BorderCollection"
second_title: "Aspose.Cells for Java API Referansı"
description: "Nesnelerin bir koleksiyonunu kapsar."
type: docs
url: /tr/java/com.aspose.cells/bordercollection/
---

**Inheritance:**
java.lang.Object
```
public class BorderCollection
```

[Border](../../com.aspose.cells/border) nesnelerinin bir koleksiyonunu kapsar.

**Example**

```
         //Instantiating a Workbook object
         Workbook workbook = new Workbook();
 
         //Adding a new worksheet to the Excel object
         workbook.getWorksheets().add();
 
         //Obtaining the reference of the newly added worksheet by passing its sheet index
         Worksheet worksheet = workbook.getWorksheets().get(0);
 
         //Accessing the "A1" cell from the worksheet
         Cell cell = worksheet.getCells().get("A1");
 
         //Adding some value to the "A1" cell
         cell.putValue("Visit Aspose!");
 
         Style style = cell.getStyle();
 
         //Setting the line style of the top border
         style.getBorders().getByBorderType(BorderType.TOP_BORDER).setLineStyle(CellBorderType.THICK);
 
         //Setting the color of the top border
         style.getBorders().getByBorderType(BorderType.TOP_BORDER).setColor(Color.getBlack());
 
         //Setting the line style of the bottom border
         style.getBorders().getByBorderType(BorderType.BOTTOM_BORDER).setLineStyle(CellBorderType.THICK);
 
         //Setting the color of the bottom border
         style.getBorders().getByBorderType(BorderType.BOTTOM_BORDER).setColor(Color.getBlack());
 
         //Setting the line style of the left border
         style.getBorders().getByBorderType(BorderType.LEFT_BORDER).setLineStyle(CellBorderType.THICK);
 
         //Setting the color of the left border
         style.getBorders().getByBorderType(BorderType.LEFT_BORDER).setColor(Color.getBlack());
 
         //Setting the line style of the right border
         style.getBorders().getByBorderType(BorderType.RIGHT_BORDER).setLineStyle(CellBorderType.THICK);
 
         //Setting the color of the right border
         style.getBorders().getByBorderType(BorderType.RIGHT_BORDER).setColor(Color.getBlack());
 
         cell.setStyle(style);
 
         //Saving the Excel file
         workbook.save("book1.xls");
```
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getByBorderType(int borderType)](#getByBorderType-int-) | Belirtilen indeksteki [Border](../../com.aspose.cells/border) öğesini alır. |
| [getClass()](#getClass--) |  |
| [getDiagonalColor()](#getDiagonalColor--) | Diagonal çizgilerin [Color](../../com.aspose.cells/color) değerini alır. |
| [getDiagonalStyle()](#getDiagonalStyle--) | Diagonal çizgilerin stilini alır. |
| [hashCode()](#hashCode--) |  |
| [isOutline()](#isOutline--) | Sol, sağ, üst ve alt kenarlıkların yalnızca bir hücre aralığının dış kenarlıklarına uygulanıp uygulanmayacağını belirtir. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setColor(Color color)](#setColor-com.aspose.cells.Color-) | Koleksiyondaki tüm kenarlıkların [Color](../../com.aspose.cells/color) değerini ayarlar. |
| [setDiagonalColor(Color value)](#setDiagonalColor-com.aspose.cells.Color-) | Diagonal çizgilerin [Color](../../com.aspose.cells/color) değerini ayarlar. |
| [setDiagonalStyle(int value)](#setDiagonalStyle-int-) | Diagonal çizgilerin stilini ayarlar. |
| [setOutline(boolean value)](#setOutline-boolean-) | Sol, sağ, üst ve alt kenarlıkların yalnızca bir hücre aralığının dış kenarlıklarına uygulanıp uygulanmayacağını belirtir. |
| [setStyle(int style)](#setStyle-int-) | Koleksiyonun tüm kenarlıklarının stilini ayarlar. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| arg0 | java.lang.Object |  |

**Returns:**
boolean
### getByBorderType(int borderType) {#getByBorderType-int-}
```
public Border getByBorderType(int borderType)
```


Belirtilen indeksteki [Border](../../com.aspose.cells/border) öğesini alır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| borderType | int | [BorderType](../../com.aspose.cells/bordertype). Alınacak kenarlık. |

**Returns:**
[Border](../../com.aspose.cells/border) - The element at the specified index.
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getDiagonalColor() {#getDiagonalColor--}
```
public Color getDiagonalColor()
```


Diagonal çizgilerin [Color](../../com.aspose.cells/color) değerini alır.

**Returns:**
[Color](../../com.aspose.cells/color)
### getDiagonalStyle() {#getDiagonalStyle--}
```
public int getDiagonalStyle()
```


Diagonal çizgilerin stilini alır.

Bakınız [CellBorderType](../../com.aspose.cells/cellbordertype).

**Returns:**
int
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isOutline() {#isOutline--}
```
public boolean isOutline()
```


Sol, sağ, üst ve alt kenarlıkların yalnızca bir hücre aralığının dış kenarlıklarına uygulanıp uygulanmayacağını belirtir. Varsayılan değer doğrudur.

**Remarks**

Yalnızca koşullu biçimlendirmeler, pivot tablolar için bir aralığa uygulanırken çalışır. false ise, sol, sağ, üst ve alt kenarlıklar her hücreye uygulanır, aksi takdirde yalnızca bir hücre aralığının dış kenarlıklarına uygulanır. true ise, lütfen koşullu biçimlendirmeler, pivot tablolar için aralığın iç kenarlıklarının yatay ve dikey kenarlıklarını ayarlayın.

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




### setColor(Color color) {#setColor-com.aspose.cells.Color-}
```
public void setColor(Color color)
```


Koleksiyondaki tüm kenarlıkların [Color](../../com.aspose.cells/color) değerini ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| color | [Color](../../com.aspose.cells/color) | Kenarlıkların [Color](../../com.aspose.cells/color) değeri. |

### setDiagonalColor(Color value) {#setDiagonalColor-com.aspose.cells.Color-}
```
public void setDiagonalColor(Color value)
```


Diagonal çizgilerin [Color](../../com.aspose.cells/color) değerini ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | [Color](../../com.aspose.cells/color) |  |

### setDiagonalStyle(int value) {#setDiagonalStyle-int-}
```
public void setDiagonalStyle(int value)
```


Diagonal çizgilerin stilini ayarlar.

Bakınız [CellBorderType](../../com.aspose.cells/cellbordertype).

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setOutline(boolean value) {#setOutline-boolean-}
```
public void setOutline(boolean value)
```


Sol, sağ, üst ve alt kenarlıkların yalnızca bir hücre aralığının dış kenarlıklarına uygulanıp uygulanmayacağını belirtir. Varsayılan değer doğrudur.

**Remarks**

Yalnızca koşullu biçimlendirmeler, pivot tablolar için bir aralığa uygulanırken çalışır. false ise, sol, sağ, üst ve alt kenarlıklar her hücreye uygulanır, aksi takdirde yalnızca bir hücre aralığının dış kenarlıklarına uygulanır. true ise, lütfen koşullu biçimlendirmeler, pivot tablolar için aralığın iç kenarlıklarının yatay ve dikey kenarlıklarını ayarlayın.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setStyle(int style) {#setStyle-int-}
```
public void setStyle(int style)
```


Koleksiyonun tüm kenarlıklarının stilini ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| style | int | [CellBorderType](../../com.aspose.cells/cellbordertype). Kenarlıkların stili |

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
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

