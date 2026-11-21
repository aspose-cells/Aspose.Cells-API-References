---
title: "ŞekilKoleksiyonu"
second_title: "Aspose.Cells for Java API Referansı"
description: "çalışma sayfasındaki/çarttaki tüm şekli temsil eder."
type: docs
url: /tr/java/com.aspose.cells/shapecollection/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.CollectionBase](../../com.aspose.cells/collectionbase)
```
public class ShapeCollection extends CollectionBase
```

çalışma sayfasındaki/çarttaki tüm şekli temsil eder.

**Example**

```
         //Instantiating a Workbook object
         Workbook workbook = new Workbook();
 
         //get ShapeCollection
         ShapeCollection shapes = workbook.getWorksheets().get(0).getShapes();
 
         //do your business
 
         //Save the excel file.
         workbook.save("result.xlsx");
```
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [add(Object o)](#add-java.lang.Object-) | CollectionBase örneğine bir öğe ekler. |
| [addActiveXControl(int type, int topRow, int top, int leftColumn, int left, int width, int height)](#addActiveXControl-int-int-int-int-int-int-int-) | Bir Activex Kontrolü oluşturur. |
| [addArc(int topRow, int top, int leftColumn, int left, int height, int width)](#addArc-int-int-int-int-int-int-) | Çalışma sayfasına bir ArcShape ekler. |
| [addAutoShape(int type, int topRow, int top, int leftColumn, int left, int height, int width)](#addAutoShape-int-int-int-int-int-int-int-) | Çalışma sayfasına bir AutoShape ekler. |
| [addAutoShapeInChart(int type, int top, int left, int height, int width)](#addAutoShapeInChart-int-int-int-int-int-) | Grafiğe bir AutoShape ekler. |
| [addButton(int topRow, int top, int leftColumn, int left, int height, int width)](#addButton-int-int-int-int-int-int-) | Çalışma sayfasına bir Düğme ekler. |
| [addCheckBox(int topRow, int top, int leftColumn, int left, int height, int width)](#addCheckBox-int-int-int-int-int-int-) | Çalışma sayfasına bir onay kutusu ekler. |
| [addComboBox(int topRow, int top, int leftColumn, int left, int height, int width)](#addComboBox-int-int-int-int-int-int-) | Çalışma sayfasına bir ComboBox ekler. |
| [addCopy(Shape sourceShape, int topRow, int top, int leftColumn, int left)](#addCopy-com.aspose.cells.Shape-int-int-int-int-) | Çalışma sayfasına bir şekil ekler ve kopyalar. |
| [addCopy(Shape sourceShape, int topRow, int top, int leftColumn, int left, CopyOptions copyOptions)](#addCopy-com.aspose.cells.Shape-int-int-int-int-com.aspose.cells.CopyOptions-) | Çalışma sayfasına bir şekil ekler ve kopyalar. |
| [addEquation(int topRow, int top, int leftColumn, int left, int height, int width)](#addEquation-int-int-int-int-int-int-) | Çalışma sayfasına bir denklem nesnesi ekler. |
| [addFreeFloatingShape(int type, int top, int left, int height, int width, byte[] imageData, boolean isOriginalSize)](#addFreeFloatingShape-int-int-int-int-int-byte---boolean-) | Çalışma sayfasına serbest yüzen bir şekil ekler. Yalnızca çizgi/görsel şekil için geçerlidir. |
| [addFreeform(int topRow, int top, int leftColumn, int left, int height, int width, ShapePath[] paths)](#addFreeform-int-int-int-int-int-int-com.aspose.cells.ShapePath---) | Çalışma sayfasına serbest biçimli bir şekil ekler. |
| [addGroupBox(int topRow, int top, int leftColumn, int left, int height, int width)](#addGroupBox-int-int-int-int-int-int-) | Çalışma sayfasına bir GroupBox ekler. |
| [addIcons(int topRow, int top, int leftColumn, int left, int height, int width, byte[] imageByteData, byte[] compatibleImageData)](#addIcons-int-int-int-int-int-int-byte---byte---) | SVG görüntüsü ekler. |
| [addLaTeXEquation(int topRow, int top, int leftColumn, int left, int height, int width, String latex)](#addLaTeXEquation-int-int-int-int-int-int-java.lang.String-) | Çalışma sayfasına LaTeX biçimindeki dizgileri kullanarak bir denklem nesnesi ekler. |
| [addLabel(int topRow, int top, int leftColumn, int left, int height, int width)](#addLabel-int-int-int-int-int-int-) | Çalışma sayfasına bir Etiket ekler. |
| [addLabelInChart(int top, int left, int height, int width)](#addLabelInChart-int-int-int-int-) | Grafiğe bir etiket ekler. |
| [addLine(int topRow, int top, int leftColumn, int left, int height, int width)](#addLine-int-int-int-int-int-int-) | Çalışma sayfasına bir LineShape ekler. |
| [addLinkedPicture(int topRow, int leftColumn, int height, int width, String sourceFullName)](#addLinkedPicture-int-int-int-int-java.lang.String-) | Bağlantılı bir resim ekle. |
| [addListBox(int topRow, int top, int leftColumn, int left, int height, int width)](#addListBox-int-int-int-int-int-int-) | Çalışma sayfasına bir ListBox ekler. |
| [addOleObject(int topRow, int top, int leftColumn, int left, int height, int width, byte[] imageData)](#addOleObject-int-int-int-int-int-int-byte---) | Bir OleObject ekler. |
| [addOleObjectWithLinkedImage(int topRow, int leftColumn, int height, int width, String sourceFullName)](#addOleObjectWithLinkedImage-int-int-int-int-java.lang.String-) | Bağlantılı bir resim ekle. |
| [addOval(int topRow, int top, int leftColumn, int left, int height, int width)](#addOval-int-int-int-int-int-int-) | Çalışma sayfasına bir Oval ekler. |
| [addPicture(int topRow, int leftColumn, int bottomRow, int rightColumn, InputStream stream)](#addPicture-int-int-int-int-java.io.InputStream-) | Koleksiyona bir resim ekler. |
| [addPicture(int topRow, int leftColumn, InputStream stream, int widthScale, int heightScale)](#addPicture-int-int-java.io.InputStream-int-int-) | Koleksiyona bir resim ekler. |
| [addPictureInChart(int top, int left, InputStream stream, int widthScale, int heightScale)](#addPictureInChart-int-int-java.io.InputStream-int-int-) | Grafiğe bir resim ekler. |
| [addRadioButton(int topRow, int top, int leftColumn, int left, int height, int width)](#addRadioButton-int-int-int-int-int-int-) | Çalışma sayfasına bir RadioButton ekler. |
| [addRectangle(int topRow, int top, int leftColumn, int left, int height, int width)](#addRectangle-int-int-int-int-int-int-) | Çalışma sayfasına bir RectangleShape ekler. |
| [addScrollBar(int topRow, int top, int leftColumn, int left, int height, int width)](#addScrollBar-int-int-int-int-int-int-) | Çalışma sayfasına bir ScrollBar ekler. |
| [addShape(int type, int topRow, int top, int leftColumn, int left, int height, int width)](#addShape-int-int-int-int-int-int-int-) | Çalışma sayfasına bir Shape ekler. |
| [addShapeInChart(int type, int placement, int left, int top, int right, int bottom)](#addShapeInChart-int-int-int-int-int-int-) | Grafiğe bir şekil ekle. Tüm birim, grafik alanının 1/4000'idir. |
| [addShapeInChart(int type, int placement, int left, int top, int right, int bottom, byte[] imageData)](#addShapeInChart-int-int-int-int-int-int-byte---) | Grafiğe bir şekil ekle. Tüm birim, grafik alanının 1/4000'idir. |
| [addShapeInChartByScale(int type, int placement, double left, double top, double right, double bottom)](#addShapeInChartByScale-int-int-double-double-double-double-) | Grafiğe bir şekil ekle. |
| [addShapeInChartByScale(int type, int placement, double left, double top, double right, double bottom, byte[] imageData)](#addShapeInChartByScale-int-int-double-double-double-double-byte---) | Grafiğe bir şekil ekle. Tüm birim, grafik alanının 1/4000'idir. |
| [addSignatureLine(int topRow, int leftColumn, SignatureLine signatureLine)](#addSignatureLine-int-int-com.aspose.cells.SignatureLine-) | Çalışma sayfasına bir Signature Line ekler. |
| [addSpinner(int topRow, int top, int leftColumn, int left, int height, int width)](#addSpinner-int-int-int-int-int-int-) | Çalışma sayfasına bir Spinner ekler. |
| [addSvg(int topRow, int top, int leftColumn, int left, int height, int width, byte[] svgData, byte[] compatibleImageData)](#addSvg-int-int-int-int-int-int-byte---byte---) | SVG görüntüsü ekler. |
| [addTextBox(int topRow, int top, int leftColumn, int left, int height, int width)](#addTextBox-int-int-int-int-int-int-) | Çalışma sayfasına bir metin kutusu ekler. |
| [addTextBoxInChart(int top, int left, int height, int width)](#addTextBoxInChart-int-int-int-int-) | Grafiğe bir metin kutusu ekler. |
| [addTextEffect(int effect, String text, String fontName, int size, boolean fontBold, boolean fontItalic, int topRow, int top, int leftColumn, int left, int height, int width)](#addTextEffect-int-java.lang.String-java.lang.String-int-boolean-boolean-int-int-int-int-int-int-) | Bir WordArt nesnesi ekler. |
| [addTextEffectInChart(int effect, String text, String fontName, int size, boolean fontBold, boolean fontItalic, int top, int left, int height, int width)](#addTextEffectInChart-int-java.lang.String-java.lang.String-int-boolean-boolean-int-int-int-int-) | Grafiğe bir WordArt nesnesi ekler |
| [addWordArt(int style, String text, int topRow, int top, int leftColumn, int left, int height, int width)](#addWordArt-int-java.lang.String-int-int-int-int-int-int-) | Excel 2007'den beri önceden tanımlı WordArt ekler.s |
| [clear()](#clear--) | Çalışma sayfasındaki tüm şekilleri temizle. |
| [contains(Object o)](#contains-java.lang.Object-) | Örneğin bu nesneyi içerip içermediğini döndürür |
| [copyCommentsInRange(ShapeCollection shapes, CellArea ca, int destRow, int destColumn)](#copyCommentsInRange-com.aspose.cells.ShapeCollection-com.aspose.cells.CellArea-int-int-) | Aralıktaki tüm yorumları kopyala. |
| [copyInRange(ShapeCollection sourceShapes, CellArea ca, int destRow, int destColumn, boolean isContained)](#copyInRange-com.aspose.cells.ShapeCollection-com.aspose.cells.CellArea-int-int-boolean-) | Aralıktaki şekilleri hedef aralığa kopyala. |
| [deleteInRange(CellArea ca)](#deleteInRange-com.aspose.cells.CellArea-) | Aralıktaki şekilleri sil. Yorum şekilleri silinmeyecek. |
| [deleteShape(Shape shape)](#deleteShape-com.aspose.cells.Shape-) | Bir şekli sil. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [find(String what, int previous, FindOptions findOptions)](#find-java.lang.String-int-com.aspose.cells.FindOptions-) | Şekli metne göre bul |
| [get(int index)](#get-int-) | Listedeki belirli indeksteki [Shape](../../com.aspose.cells/shape) nesnesini al. |
| [get(String name)](#get-java.lang.String-) | Şeklin adıyla [Shape](../../com.aspose.cells/shape) nesnesini al. |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | CollectionBase örneğinde bulunan eleman sayısını alır. |
| [group(Shape[] groupItems)](#group-com.aspose.cells.Shape---) | Şekilleri grupla. |
| [hashCode()](#hashCode--) |  |
| [indexOf(Object o)](#indexOf-java.lang.Object-) | CollectionBase örneğindeki belirli bir öğenin dizinini belirler. |
| [iterator()](#iterator--) | CollectionBase örneği üzerinde yineleme yapan bir enumerator döndürür. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [remove(Shape shape)](#remove-com.aspose.cells.Shape-) | Şekli kaldır. |
| [removeAt(int index)](#removeAt-int-) | Şekli kaldır. |
| [toString()](#toString--) |  |
| [ungroup(GroupShape group)](#ungroup-com.aspose.cells.GroupShape-) | Şekil öğelerinin grubunu çöz. |
| [updateSelectedValue()](#updateSelectedValue--) | Şeklin bağlı hücre veya aralığının değeriyle seçili değeri güncelle. |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### add(Object o) {#add-java.lang.Object-}
```
public int add(Object o)
```


CollectionBase örneğine bir öğe ekler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| o | java.lang.Object | CollectionBase örneğine eklenecek Nesne. |

**Returns:**
int - Yeni elemanın eklendiği konum.
### addActiveXControl(int type, int topRow, int top, int leftColumn, int left, int width, int height) {#addActiveXControl-int-int-int-int-int-int-int-}
```
public Shape addActiveXControl(int type, int topRow, int top, int leftColumn, int left, int width, int height)
```


Bir Activex Kontrolü oluşturur.

**Example**

```
         //add an ActiveX control
         Shape activeXControl = shapes.addActiveXControl(com.aspose.cells.ControlType.CHECK_BOX, 1, 0, 1, 0, 100, 50);
```

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| type | int | [ControlType](../../com.aspose.cells/controltype). Kontrolün türü. |
| üstSatır | int | Üst sol satır indeksi. |
| üst | int | Şeklin sol satırından dikey ofsetini, piksel biriminde temsil eder. |
| leftColumn | int | Üst sol sütun indeksi. |
| sol | int | Şeklin sol sütunundan yatay ofsetini, piksel biriminde temsil eder. |
| genişlik | int | Şeklin genişliğini, piksel biriminde temsil eder. |
| yükseklik | int | Şeklin yüksekliğini, piksel biriminde temsil eder. |

**Returns:**
[Shape](../../com.aspose.cells/shape) - 
### addArc(int topRow, int top, int leftColumn, int left, int height, int width) {#addArc-int-int-int-int-int-int-}
```
public ArcShape addArc(int topRow, int top, int leftColumn, int left, int height, int width)
```


Çalışma sayfasına bir ArcShape ekler.

**Example**

```
         //add a arc
         ArcShape arcShape = shapes.addArc(1, 0, 1, 0, 100, 50);
```

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| üstSatır | int | Üst sol satır indeksi. |
| üst | int | ArcShape'in sol satırından dikey ofsetini, piksel biriminde temsil eder. |
| leftColumn | int | Üst sol sütun indeksi. |
| sol | int | ArcShape'in sol sütunundan yatay ofsetini, piksel biriminde temsil eder. |
| yükseklik | int | ArcShape'in yüksekliğini, piksel biriminde temsil eder. |
| genişlik | int | ArcShape'in genişliğini, piksel biriminde temsil eder. |

**Returns:**
[ArcShape](../../com.aspose.cells/arcshape) - A ArcShape object.
### addAutoShape(int type, int topRow, int top, int leftColumn, int left, int height, int width) {#addAutoShape-int-int-int-int-int-int-int-}
```
public Shape addAutoShape(int type, int topRow, int top, int leftColumn, int left, int height, int width)
```


Çalışma sayfasına bir AutoShape ekler.

**Remarks**

Tür, Chart/Comment/Picture/OleObject/Polygon/DialogBox olamaz

**Example**

```
         //Adds a AutoShape to the worksheet.
         Shape autoShape = shapes.addAutoShape(AutoShapeType.CUBE, 1, 0, 1, 0, 100, 50);
```

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| type | int | [AutoShapeType](../../com.aspose.cells/autoshapetype). Otomatik şekil türü. |
| üstSatır | int | Üst sol satır indeksi. |
| üst | int | Şeklin sol satırından dikey ofsetini, piksel biriminde temsil eder. |
| leftColumn | int | Üst sol sütun indeksi. |
| sol | int | Şeklin sol sütunundan yatay ofsetini, piksel biriminde temsil eder. |
| yükseklik | int | Şeklin yüksekliğini, piksel biriminde temsil eder. |
| genişlik | int | Şeklin genişliğini, piksel biriminde temsil eder. |

**Returns:**
[Shape](../../com.aspose.cells/shape) - A Shape object.
### addAutoShapeInChart(int type, int top, int left, int height, int width) {#addAutoShapeInChart-int-int-int-int-int-}
```
public Shape addAutoShapeInChart(int type, int top, int left, int height, int width)
```


Grafiğe bir AutoShape ekler.

**Remarks**

Tür, Chart/Comment/Picture/OleObject/Polygon/DialogBox olamaz

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| type | int | [AutoShapeType](../../com.aspose.cells/autoshapetype). Otomatik şekil türü. |
| üst | int | Metin kutusunun sol üst köşesinden dikey ofsetini, grafik alanının 1/4000 biriminde temsil eder. |
| sol | int | Metin kutusunun sol üst köşesinden dikey ofsetini, grafik alanının 1/4000 biriminde temsil eder. |
| yükseklik | int | Metin kutusunun yüksekliğini, grafik alanının 1/4000 biriminde temsil eder. |
| genişlik | int | Metin kutusunun genişliğini, grafik alanının 1/4000 biriminde temsil eder. |

**Returns:**
[Shape](../../com.aspose.cells/shape) - Returns a shape object.
### addButton(int topRow, int top, int leftColumn, int left, int height, int width) {#addButton-int-int-int-int-int-int-}
```
public Button addButton(int topRow, int top, int leftColumn, int left, int height, int width)
```


Çalışma sayfasına bir Düğme ekler.

**Example**

```
         //add a button
         Button button = shapes.addButton(1, 0, 1, 0, 100, 50);
```

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| üstSatır | int | Üst sol satır indeksi. |
| üst | int | Düğmenin sol satırından dikey ofsetini, piksel biriminde temsil eder. |
| leftColumn | int | Üst sol sütun indeksi. |
| sol | int | Düğmenin sol sütunundan yatay ofsetini, piksel biriminde temsil eder. |
| yükseklik | int | Düğmenin yüksekliğini, piksel biriminde temsil eder. |
| genişlik | int | Düğmenin genişliğini, piksel biriminde temsil eder. |

**Returns:**
[Button](../../com.aspose.cells/button) - A Button object.
### addCheckBox(int topRow, int top, int leftColumn, int left, int height, int width) {#addCheckBox-int-int-int-int-int-int-}
```
public CheckBox addCheckBox(int topRow, int top, int leftColumn, int left, int height, int width)
```


Çalışma sayfasına bir onay kutusu ekler.

**Example**

```
         //add a CheckBox
         CheckBox checkBox = shapes.addCheckBox(1, 0, 1, 0, 100, 50);
```

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| üstSatır | int | Üst sol satır indeksi. |
| üst | int | Onay kutusunun üst satırından dikey ofsetini, piksel biriminde temsil eder. |
| leftColumn | int | Üst sol sütun indeksi. |
| sol | int | Metin kutusunun sol sütunundan yatay ofsetini, piksel biriminde temsil eder. |
| yükseklik | int | Metin kutusunun yüksekliği, piksel biriminde. |
| genişlik | int | Metin kutusunun genişliği, piksel biriminde. |

**Returns:**
[CheckBox](../../com.aspose.cells/checkbox) - The new CheckBox object index.
### addComboBox(int topRow, int top, int leftColumn, int left, int height, int width) {#addComboBox-int-int-int-int-int-int-}
```
public ComboBox addComboBox(int topRow, int top, int leftColumn, int left, int height, int width)
```


Çalışma sayfasına bir ComboBox ekler.

**Example**

```
         //add a combo box
         ComboBox comboBox = shapes.addComboBox(1, 0, 1, 0, 100, 50);
```

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| üstSatır | int | Üst sol satır indeksi. |
| üst | int | ComboBox'ın sol satırından dikey ofsetini, piksel biriminde temsil eder. |
| leftColumn | int | Üst sol sütun indeksi. |
| sol | int | ComboBox'ın sol sütunundan yatay ofsetini, piksel biriminde temsil eder. |
| yükseklik | int | ComboBox yüksekliğini temsil eder, birim olarak piksel. |
| genişlik | int | ComboBox genişliğini temsil eder, birim olarak piksel. |

**Returns:**
[ComboBox](../../com.aspose.cells/combobox) - A ComboBox object.
### addCopy(Shape sourceShape, int topRow, int top, int leftColumn, int left) {#addCopy-com.aspose.cells.Shape-int-int-int-int-}
```
public Shape addCopy(Shape sourceShape, int topRow, int top, int leftColumn, int left)
```


Çalışma sayfasına bir şekil ekler ve kopyalar.

**Example**

```
         //add a shape
         RectangleShape rectangle = shapes.addRectangle(2, 0, 2, 0, 130, 130);
         //Adds and copies a shape.
         shapes.addCopy(rectangle, 7, 0, 7, 0);
```

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| sourceShape | [Shape](../../com.aspose.cells/shape) | Kaynak şekil. |
| üstSatır | int | Üst satır indeksi. |
| üst | int | Üst satırından dikey offseti temsil eder, birim olarak piksel. |
| leftColumn | int | Sol sütun indeksi. |
| sol | int | Sol sütunundan yatay offseti temsil eder, birim olarak piksel. |

**Returns:**
[Shape](../../com.aspose.cells/shape) - The new [Shape](../../com.aspose.cells/shape) object.
### addCopy(Shape sourceShape, int topRow, int top, int leftColumn, int left, CopyOptions copyOptions) {#addCopy-com.aspose.cells.Shape-int-int-int-int-com.aspose.cells.CopyOptions-}
```
public Shape addCopy(Shape sourceShape, int topRow, int top, int leftColumn, int left, CopyOptions copyOptions)
```


Çalışma sayfasına bir şekil ekler ve kopyalar.

**Example**

```
         //add a shape
         RectangleShape rectangle = shapes.addRectangle(2, 0, 2, 0, 130, 130);
         //Adds and copies a shape.
         shapes.addCopy(rectangle, 7, 0, 7, 0);
```

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| sourceShape | [Shape](../../com.aspose.cells/shape) | Kaynak şekil. |
| üstSatır | int | Üst satır indeksi. |
| üst | int | Üst satırından dikey offseti temsil eder, birim olarak piksel. |
| leftColumn | int | Sol sütun indeksi. |
| sol | int | Sol sütunundan yatay offseti temsil eder, birim olarak piksel. |
| copyOptions | [CopyOptions](../../com.aspose.cells/copyoptions) | Şekilleri kopyalama seçenekleri. |

**Returns:**
[Shape](../../com.aspose.cells/shape) - The new [Shape](../../com.aspose.cells/shape) object.
### addEquation(int topRow, int top, int leftColumn, int left, int height, int width) {#addEquation-int-int-int-int-int-int-}
```
public TextBox addEquation(int topRow, int top, int leftColumn, int left, int height, int width)
```


Çalışma sayfasına bir denklem nesnesi ekler.

**Example**

```
         // Adds an equation object to the worksheet.
         TextBox textBox = shapes.addEquation(1, 0, 1, 0, 100, 300);
 
         // Gets the starting node of the equation object
         EquationNode mathNode = textBox.getEquationParagraph().getChild(0);
 
         // Inserts a fractional equation.
         FractionEquationNode node = (FractionEquationNode)mathNode.addChild(EquationNodeType.FRACTION);
         node.setFractionType(EquationFractionType.SKEWED);
 
         String str1 = "A";
         EquationComponentNode numerator = (EquationComponentNode)node.addChild(EquationNodeType.NUMERATOR);
         TextRunEquationNode TR = (TextRunEquationNode)(numerator.addChild(EquationNodeType.TEXT));
         TR.setText(str1);
 
         String str2 = "B";
         EquationComponentNode denominator = (EquationComponentNode)node.addChild(EquationNodeType.DENOMINATOR);
         TR = (TextRunEquationNode) (denominator.addChild(EquationNodeType.TEXT));
         TR.setText(str2);
```

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| üstSatır | int | Üst satır indeksi. |
| üst | int | Üst satırının dikey offseti, birim olarak piksel. |
| leftColumn | int | Sol sütun indeksi. |
| sol | int | Sol sütunundan yatay offseti, birim olarak piksel. |
| yükseklik | int | Denklemin yüksekliği, birim olarak piksel. |
| genişlik | int | Denklemin genişliği, birim olarak piksel. |

**Returns:**
[TextBox](../../com.aspose.cells/textbox) - 
### addFreeFloatingShape(int type, int top, int left, int height, int width, byte[] imageData, boolean isOriginalSize) {#addFreeFloatingShape-int-int-int-int-int-byte---boolean-}
```
public Shape addFreeFloatingShape(int type, int top, int left, int height, int width, byte[] imageData, boolean isOriginalSize)
```


Çalışma sayfasına serbest yüzen bir şekil ekler. Yalnızca çizgi/görsel şekil için geçerlidir.

**Example**

```
         //add a line
         Shape floatingShape_Line = shapes.addFreeFloatingShape(MsoDrawingType.LINE, 100, 100, 100, 50, null, false);
         //add a picture
         byte[] imageData = null;
         FileInputStream fs = new FileInputStream("image.jpg");
         try //JAVA: was using
         {
             int len = (int)fs.available();
             imageData = new byte[len];
             fs.read(imageData, 0, len);
         }
         finally { if (fs != null) fs.close(); }
         Shape floatingShape_Picture = shapes.addFreeFloatingShape(MsoDrawingType.PICTURE, 200, 100, 100, 50, imageData, false);
```

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| type | int | [MsoDrawingType](../../com.aspose.cells/msodrawingtype). Şekil türü. |
| üst | int | Şeklin çalışma sayfasının üst satırından dikey offsetini temsil eder, birim olarak piksel. |
| sol | int | Şeklin çalışma sayfasının sol sütunundan yatay offsetini temsil eder, birim olarak piksel. |
| yükseklik | int | LineShape yüksekliğini temsil eder, birim olarak piksel. |
| genişlik | int | LineShape genişliğini temsil eder, birim olarak piksel. |
| imageData | byte[] | Görüntü verisi, yalnızca resim için geçerlidir. |
| isOriginalSize | boolean | Şekil bir resim ise orijinal boyutu kullanıp kullanmayacağını belirtir. |

**Returns:**
[Shape](../../com.aspose.cells/shape) - 
### addFreeform(int topRow, int top, int leftColumn, int left, int height, int width, ShapePath[] paths) {#addFreeform-int-int-int-int-int-int-com.aspose.cells.ShapePath---}
```
public Shape addFreeform(int topRow, int top, int leftColumn, int left, int height, int width, ShapePath[] paths)
```


Çalışma sayfasına serbest biçimli bir şekil ekler.

**Remarks**

Uyarı: Parametrelerdeki genişlik ve yükseklik, ShapePath dizisinin \\u9225\\u6a96aths' tarafından belirtilen toplam genişlik ve yükseklik değil, herhangi bir pozitif tam sayı değeri olabilir. Aralarındaki ilişki bir ölçek-doldurma ilişkisidir, yani her ShapePath nesnesi genişlik ve yüksekliğe göre ölçeklenecektir. Bu nedenle, 'paths' içinde birden fazla nesne olduğunda, her ShapePath nesnesi beklentileri karşılayacak şekilde makul olarak tasarlanmalıdır. Yalnızca bir ShapePath nesnesi olduğunda ve başka gereksinim yoksa, nesnenin genişlik ve yüksekliğini parametre değerleri olarak \\u9225\\u5b27\\u20ac\\u5a94s geçirmek iyi bir çözümdür.

**Example**

```
         //Custom figure
         ShapePath shapePath = new ShapePath();
         shapePath.moveTo(60, 45);
         shapePath.arcTo(25, 25, 0, 270);
         shapePath.close();
 
         shapePath.moveTo(60, 20);
         shapePath.lineTo(110, 70);
         shapePath.lineTo(125, 155.5f);
         shapePath.arcTo(35.5f, 35.5f, 0, 270);
         shapePath.close();
 
         shapePath.moveTo(150, 45);
         shapePath.arcTo(25, 25, 0, 270);
 
         int shapePathW = shapePath.getWidthPixel();
         int shapePathH = shapePath.getHeightPixel();
 
         ShapePath shapePath1 = new ShapePath();
         shapePath1.moveTo(0, 0);
         shapePath1.cubicBezierTo(48.24997f, 0.6844f,
                             96.5f, -7.148871f,
                             130, 11.517795f);
         shapePath1.cubicBezierTo(163.5f, 30.18446f,
                             182.24997f, 75.351f,
                             201, 120.517795f);
         shapePath1.moveTo(150, 80);
         shapePath1.arcTo(25, 25, 0, 270);
 
         if (shapePath1.getWidthPixel() > shapePathW)
             {
         shapePathW = shapePath1.getWidthPixel();
         }
 
         if (shapePath1.getHeightPixel() > shapePathH)
         {
         shapePathH = shapePath1.getHeightPixel();
         }
 
         //Notice: shapePathH and shapePathH can be any positive integer values, here we just simply set them.
 
         //Insert custom figure into worksheet
         shapes.addFreeform(1, 0, 1, 0, shapePathH, shapePathW, new ShapePath[] { shapePath, shapePath1});
```

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| üstSatır | int | Üst sol satır indeksi. |
| üst | int | Serbest şeklin sol satırından dikey offsetini temsil eder, birim olarak piksel. |
| leftColumn | int | Üst sol sütun indeksi. |
| sol | int | Serbest şeklin sol sütunundan yatay offsetini temsil eder, birim olarak piksel. |
| yükseklik | int | Serbest şeklin yüksekliğini temsil eder, birim olarak piksel. |
| genişlik | int | Serbest şeklin genişliğini temsil eder, birim olarak piksel. |
| paths | [ShapePath\[\]](../../com.aspose.cells/shapepath) | Kullanıcı tanımlı bir yolu temsil eder |

**Returns:**
[Shape](../../com.aspose.cells/shape) - A freeform shape.
### addGroupBox(int topRow, int top, int leftColumn, int left, int height, int width) {#addGroupBox-int-int-int-int-int-int-}
```
public GroupBox addGroupBox(int topRow, int top, int leftColumn, int left, int height, int width)
```


Çalışma sayfasına bir GroupBox ekler.

**Example**

```
         //add a group box
         GroupBox groupBox = shapes.addGroupBox(1, 0, 1, 0, 100, 50);
```

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| üstSatır | int | Üst sol satır indeksi. |
| üst | int | GroupBox'ın sol satırından dikey ofseti, piksel biriminde temsil eder. |
| leftColumn | int | Üst sol sütun indeksi. |
| sol | int | GroupBox'ın sol sütunundan yatay ofseti, piksel biriminde temsil eder. |
| yükseklik | int | GroupBox'ın yüksekliğini piksel biriminde temsil eder. |
| genişlik | int | GroupBox'ın genişliğini piksel biriminde temsil eder. |

**Returns:**
[GroupBox](../../com.aspose.cells/groupbox) - A GroupBox object.
### addIcons(int topRow, int top, int leftColumn, int left, int height, int width, byte[] imageByteData, byte[] compatibleImageData) {#addIcons-int-int-int-int-int-int-byte---byte---}
```
public Picture addIcons(int topRow, int top, int leftColumn, int left, int height, int width, byte[] imageByteData, byte[] compatibleImageData)
```


SVG görüntüsü ekler.

**Example**

```
         //add icon
         FileInputStream fs = new FileInputStream("icon.svg");
         try //JAVA: was using
         {
             int len = (int)fs.available();
             byte[] imageData = new byte[len];
             fs.read(imageData, 0, len);
             Picture picture = shapes.addIcons(4, 0, 5, 0, -1, -1, imageData, null);
         }
         finally { if (fs != null) fs.close(); }
```

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| üstSatır | int | Üst sol satır indeksi. |
| üst | int | Şeklin sol satırından dikey ofseti, piksel biriminde temsil eder. |
| leftColumn | int | Üst sol sütun indeksi. |
| sol | int | Şeklin sol sütunundan yatay ofseti, piksel biriminde. |
| yükseklik | int | Şeklin yüksekliği, piksel biriminde. |
| genişlik | int | Şeklin genişliği, piksel biriminde. |
| imageByteData | byte[] | Görüntü bayt verisi. |
| compatibleImageData | byte[] | Excel 2016 veya daha düşük sürümlerle uyumlu olması için svg'den dönüştürülmüş görüntü verisi. |

**Returns:**
[Picture](../../com.aspose.cells/picture) - 
### addLaTeXEquation(int topRow, int top, int leftColumn, int left, int height, int width, String latex) {#addLaTeXEquation-int-int-int-int-int-int-java.lang.String-}
```
public TextBox addLaTeXEquation(int topRow, int top, int leftColumn, int left, int height, int width, String latex)
```


Çalışma sayfasına LaTeX biçimindeki dizgileri kullanarak bir denklem nesnesi ekler.

**Example**

```
         // LaTeX format string.
         String latex = "\\alpha +  \\frac{\\partial^2}{\\partial x_1\\partial x_2}y - \\left ( a + b \\right )+_{a}^{b}\\beta";
         // Adds an equation object to the worksheet.
         TextBox textBox = shapes.addLaTeXEquation(1, 0, 1, 0, 100, 300, latex);
```

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| üstSatır | int | Üst satır indeksi. |
| üst | int | Üst satırının dikey offseti, birim olarak piksel. |
| leftColumn | int | Sol sütun indeksi. |
| sol | int | Sol sütunundan yatay offseti, birim olarak piksel. |
| yükseklik | int | Denklemin yüksekliği, birim olarak piksel. |
| genişlik | int | Denklemin genişliği, birim olarak piksel. |
| latex | java.lang.String | LaTeX format dizesi |

**Returns:**
[TextBox](../../com.aspose.cells/textbox) - 
### addLabel(int topRow, int top, int leftColumn, int left, int height, int width) {#addLabel-int-int-int-int-int-int-}
```
public Label addLabel(int topRow, int top, int leftColumn, int left, int height, int width)
```


Çalışma sayfasına bir Etiket ekler.

**Example**

```
         //add a label
         Label label = shapes.addLabel(1, 0, 1, 0, 100, 50);
```

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| üstSatır | int | Üst sol satır indeksi. |
| üst | int | Label'ın sol satırından dikey ofseti, piksel biriminde temsil eder. |
| leftColumn | int | Üst sol sütun indeksi. |
| sol | int | Label'ın sol sütunundan yatay ofseti, piksel biriminde temsil eder. |
| yükseklik | int | Label'ın yüksekliğini piksel biriminde temsil eder. |
| genişlik | int | Label'ın genişliğini piksel biriminde temsil eder. |

**Returns:**
[Label](../../com.aspose.cells/label) - A Label object.
### addLabelInChart(int top, int left, int height, int width) {#addLabelInChart-int-int-int-int-}
```
public Label addLabelInChart(int top, int left, int height, int width)
```


Grafiğe bir etiket ekler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| üst | int | label'in sol üst köşesinden dikey ofseti, grafik alanının 1/4000 biriminde temsil eder. |
| sol | int | label'in sol üst köşesinden dikey ofseti, grafik alanının 1/4000 biriminde temsil eder. |
| yükseklik | int | label'in yüksekliğini, grafik alanının 1/4000 biriminde temsil eder. |
| genişlik | int | label'in genişliğini, grafik alanının 1/4000 biriminde temsil eder. |

**Returns:**
[Label](../../com.aspose.cells/label) - A new Label object.
### addLine(int topRow, int top, int leftColumn, int left, int height, int width) {#addLine-int-int-int-int-int-int-}
```
public LineShape addLine(int topRow, int top, int leftColumn, int left, int height, int width)
```


Çalışma sayfasına bir LineShape ekler.

**Example**

```
         // add a line object
         LineShape lineShape = shapes.addLine(1, 0, 1, 0, 100, 50);
```

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| üstSatır | int | Üst sol satır indeksi. |
| üst | int | LineShape'in sol satırından dikey ofseti, piksel biriminde temsil eder. |
| leftColumn | int | Üst sol sütun indeksi. |
| sol | int | LineShape'in sol sütunundan yatay ofseti, piksel biriminde temsil eder. |
| yükseklik | int | LineShape yüksekliğini temsil eder, birim olarak piksel. |
| genişlik | int | LineShape genişliğini temsil eder, birim olarak piksel. |

**Returns:**
[LineShape](../../com.aspose.cells/lineshape) - A LineShape object.
### addLinkedPicture(int topRow, int leftColumn, int height, int width, String sourceFullName) {#addLinkedPicture-int-int-int-int-java.lang.String-}
```
public Picture addLinkedPicture(int topRow, int leftColumn, int height, int width, String sourceFullName)
```


Bağlantılı bir resim ekle.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| üstSatır | int | Üst sol satır indeksi. |
| leftColumn | int | Üst sol sütun indeksi. |
| yükseklik | int | Şeklin yüksekliği. Piksel biriminde |
| genişlik | int | Şeklin genişliği. Piksel biriminde |
| sourceFullName | java.lang.String | Bağlantılı görüntü için kaynak dosyanın yolu ve adı |

**Returns:**
[Picture](../../com.aspose.cells/picture) - [Picture](../../com.aspose.cells/picture) Picture object.
### addListBox(int topRow, int top, int leftColumn, int left, int height, int width) {#addListBox-int-int-int-int-int-int-}
```
public ListBox addListBox(int topRow, int top, int leftColumn, int left, int height, int width)
```


Çalışma sayfasına bir ListBox ekler.

**Example**

```
         //add a list box
         ListBox listBox = shapes.addListBox(1, 0, 1, 0, 100, 50);
```

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| üstSatır | int | Üst sol satır indeksi. |
| üst | int | ListBox'ın sol satırından dikey kaymasını temsil eder, piksel biriminde. |
| leftColumn | int | Üst sol sütun indeksi. |
| sol | int | ListBox'ın sol sütunundan yatay kaymasını temsil eder, piksel biriminde. |
| yükseklik | int | ListBox'ın yüksekliğini temsil eder, piksel biriminde. |
| genişlik | int | ListBox'ın genişliğini temsil eder, piksel biriminde. |

**Returns:**
[ListBox](../../com.aspose.cells/listbox) - A ListBox object.
### addOleObject(int topRow, int top, int leftColumn, int left, int height, int width, byte[] imageData) {#addOleObject-int-int-int-int-int-int-byte---}
```
public OleObject addOleObject(int topRow, int top, int leftColumn, int left, int height, int width, byte[] imageData)
```


Bir OleObject ekler.

**Example**

```
         FileInputStream fs = new FileInputStream("image.jpg");
         try //JAVA: was using
         {
             int len = (int)fs.available();
             byte[] imageData = new byte[len];
             fs.read(imageData, 0, len);
             OleObject oleObject = shapes.addOleObject(4, 0, 5, 0, 300, 500, imageData);
         }
         finally { if (fs != null) fs.close(); }
```

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| üstSatır | int |  |
| üst | int |  |
| leftColumn | int |  |
| sol | int |  |
| yükseklik | int |  |
| genişlik | int |  |
| imageData | byte[] |  |

**Returns:**
[OleObject](../../com.aspose.cells/oleobject) - 
### addOleObjectWithLinkedImage(int topRow, int leftColumn, int height, int width, String sourceFullName) {#addOleObjectWithLinkedImage-int-int-int-int-java.lang.String-}
```
public OleObject addOleObjectWithLinkedImage(int topRow, int leftColumn, int height, int width, String sourceFullName)
```


Bağlantılı bir resim ekle.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| üstSatır | int | Üst sol satır indeksi. |
| leftColumn | int | Üst sol sütun indeksi. |
| yükseklik | int | Şeklin yüksekliği. Piksel biriminde |
| genişlik | int | Şeklin genişliği. Piksel biriminde |
| sourceFullName | java.lang.String | Bağlantılı görüntü için kaynak dosyanın yolu ve adı |

**Returns:**
[OleObject](../../com.aspose.cells/oleobject) - [Picture](../../com.aspose.cells/picture) Picture object.
### addOval(int topRow, int top, int leftColumn, int left, int height, int width) {#addOval-int-int-int-int-int-int-}
```
public Oval addOval(int topRow, int top, int leftColumn, int left, int height, int width)
```


Çalışma sayfasına bir Oval ekler.

**Example**

```
         //add a oval
         Oval oval = shapes.addOval(1, 0, 1, 0, 50, 50);
```

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| üstSatır | int | Üst sol satır indeksi. |
| üst | int | Oval'ın sol satırından dikey kaymasını temsil eder, piksel biriminde. |
| leftColumn | int | Üst sol sütun indeksi. |
| sol | int | Oval'ın sol sütunundan yatay kaymasını temsil eder, piksel biriminde. |
| yükseklik | int | Oval'ın yüksekliğini temsil eder, piksel biriminde. |
| genişlik | int | Oval'ın genişliğini temsil eder, piksel biriminde |

**Returns:**
[Oval](../../com.aspose.cells/oval) - A Oval object.
### addPicture(int topRow, int leftColumn, int bottomRow, int rightColumn, InputStream stream) {#addPicture-int-int-int-int-java.io.InputStream-}
```
public Picture addPicture(int topRow, int leftColumn, int bottomRow, int rightColumn, InputStream stream)
```


Koleksiyona bir resim ekler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| üstSatır | int | Üst sol satır indeksi. |
| leftColumn | int | Üst sol sütun indeksi. |
| bottomRow | int | Alt sağ satır indeksi |
| rightColumn | int | Alt sağ sütun indeksi |
| stream | java.io.InputStream | Görüntü verilerini içeren akış nesnesi. |

**Returns:**
[Picture](../../com.aspose.cells/picture) - [Picture](../../com.aspose.cells/picture) Picture object.
### addPicture(int topRow, int leftColumn, InputStream stream, int widthScale, int heightScale) {#addPicture-int-int-java.io.InputStream-int-int-}
```
public Picture addPicture(int topRow, int leftColumn, InputStream stream, int widthScale, int heightScale)
```


Koleksiyona bir resim ekler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| üstSatır | int | Üst sol satır indeksi. |
| leftColumn | int | Üst sol sütun indeksi. |
| stream | java.io.InputStream | Görüntü verilerini içeren akış nesnesi. |
| widthScale | int | Görüntü genişliğinin ölçeği, yüzde olarak. |
| heightScale | int | Görüntü yüksekliğinin ölçeği, yüzde olarak. |

**Returns:**
[Picture](../../com.aspose.cells/picture) - [Picture](../../com.aspose.cells/picture) Picture object.
### addPictureInChart(int top, int left, InputStream stream, int widthScale, int heightScale) {#addPictureInChart-int-int-java.io.InputStream-int-int-}
```
public Picture addPictureInChart(int top, int left, InputStream stream, int widthScale, int heightScale)
```


Grafiğe bir resim ekler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| üst | int | Şeklin sol üst köşesinden dikey kaymasını, grafik alanının 1/4000 birimiyle temsil eder. |
| sol | int | Şeklin sol üst köşesinden yatay kaymasını, grafik alanının 1/4000 birimiyle temsil eder. |
| stream | java.io.InputStream | Görüntü verilerini içeren akış nesnesi. |
| widthScale | int | Görüntü genişliğinin ölçeği, yüzde olarak. |
| heightScale | int | Görüntü yüksekliğinin ölçeği, yüzde olarak. |

**Returns:**
[Picture](../../com.aspose.cells/picture) - Returns a Picture object.
### addRadioButton(int topRow, int top, int leftColumn, int left, int height, int width) {#addRadioButton-int-int-int-int-int-int-}
```
public RadioButton addRadioButton(int topRow, int top, int leftColumn, int left, int height, int width)
```


Çalışma sayfasına bir RadioButton ekler.

**Example**

```
         //add a radio button
         RadioButton radioButton = shapes.addRadioButton(1, 0, 1, 0, 100, 50);
```

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| üstSatır | int | Üst sol satır indeksi. |
| üst | int | RadioButton'ın sol satırından dikey kaymasını temsil eder, piksel biriminde. |
| leftColumn | int | Üst sol sütun indeksi. |
| sol | int | RadioButton'ın sol sütunundan yatay kaymasını temsil eder, piksel biriminde. |
| yükseklik | int | RadioButton'ın yüksekliğini temsil eder, piksel biriminde. |
| genişlik | int | RadioButton'ın genişliğini temsil eder, piksel biriminde. |

**Returns:**
[RadioButton](../../com.aspose.cells/radiobutton) - A RadioButton object.
### addRectangle(int topRow, int top, int leftColumn, int left, int height, int width) {#addRectangle-int-int-int-int-int-int-}
```
public RectangleShape addRectangle(int topRow, int top, int leftColumn, int left, int height, int width)
```


Çalışma sayfasına bir RectangleShape ekler.

**Example**

```
         // add a rectangle
         RectangleShape rectangleShape = shapes.addRectangle(2, 0, 2, 0, 130, 130);
```

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| üstSatır | int | Üst sol satır indeksi. |
| üst | int | RectangleShape'in sol satırından dikey kaymasını temsil eder, piksel biriminde. |
| leftColumn | int | Üst sol sütun indeksi. |
| sol | int | RectangleShape'in sol sütunundan yatay kaymasını temsil eder, piksel biriminde |
| yükseklik | int | RectangleShape yüksekliğini temsil eder, birim piksel olarak. |
| genişlik | int | RectangleShape genişliğini temsil eder, birim piksel olarak. |

**Returns:**
[RectangleShape](../../com.aspose.cells/rectangleshape) - A RectangleShape object.
### addScrollBar(int topRow, int top, int leftColumn, int left, int height, int width) {#addScrollBar-int-int-int-int-int-int-}
```
public ScrollBar addScrollBar(int topRow, int top, int leftColumn, int left, int height, int width)
```


Çalışma sayfasına bir ScrollBar ekler.

**Example**

```
         //add a scroll bar
         ScrollBar scrollBar = shapes.addScrollBar(1, 0, 1, 0, 100, 20);
```

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| üstSatır | int | Üst sol satır indeksi. |
| üst | int | ScrollBar'ın sol satırından dikey ofseti temsil eder, birim piksel olarak. |
| leftColumn | int | Üst sol sütun indeksi. |
| sol | int | ScrollBar'ın sol sütunundan yatay ofseti temsil eder, birim piksel olarak. |
| yükseklik | int | ScrollBar yüksekliğini temsil eder, birim piksel olarak. |
| genişlik | int | ScrollBar genişliğini temsil eder, birim piksel olarak. |

**Returns:**
[ScrollBar](../../com.aspose.cells/scrollbar) - A ScrollBar object.
### addShape(int type, int topRow, int top, int leftColumn, int left, int height, int width) {#addShape-int-int-int-int-int-int-int-}
```
public Shape addShape(int type, int topRow, int top, int leftColumn, int left, int height, int width)
```


Çalışma sayfasına bir Shape ekler.

**Remarks**

Tür, Chart/Comment/Picture/OleObject/Polygon/DialogBox olamaz

**Example**

```
         //Add a shape of the specified type
         Shape shapeByType = shapes.addShape(MsoDrawingType.CELLS_DRAWING, 1, 0, 1, 0, 100, 50);
```

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| type | int | [MsoDrawingType](../../com.aspose.cells/msodrawingtype). Mso çizim türü. |
| üstSatır | int | Üst sol satır indeksi. |
| üst | int | Şeklin sol satırından dikey ofsetini, piksel biriminde temsil eder. |
| leftColumn | int | Üst sol sütun indeksi. |
| sol | int | Şeklin sol sütunundan yatay ofsetini, piksel biriminde temsil eder. |
| yükseklik | int | Şeklin yüksekliğini, piksel biriminde temsil eder. |
| genişlik | int | Şeklin genişliğini, piksel biriminde temsil eder. |

**Returns:**
[Shape](../../com.aspose.cells/shape) - A Shape object.
### addShapeInChart(int type, int placement, int left, int top, int right, int bottom) {#addShapeInChart-int-int-int-int-int-int-}
```
public Shape addShapeInChart(int type, int placement, int left, int top, int right, int bottom)
```


Grafiğe bir şekil ekle. Tüm birim, grafik alanının 1/4000'idir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| type | int | [MsoDrawingType](../../com.aspose.cells/msodrawingtype). Çizim türü. |
| placement | int | [PlacementType](../../com.aspose.cells/placementtype). yerleştirme türü. |
| sol | int | Birim olarak 1/4000 grafik alanı genişliği. |
| üst | int | Birim olarak 1/4000 grafik alanı yüksekliği. |
| sağ | int | Birim olarak 1/4000 grafik alanı genişliği. |
| alt | int | Birim olarak 1/4000 grafik alanı yüksekliği. |

**Returns:**
[Shape](../../com.aspose.cells/shape)
### addShapeInChart(int type, int placement, int left, int top, int right, int bottom, byte[] imageData) {#addShapeInChart-int-int-int-int-int-int-byte---}
```
public Shape addShapeInChart(int type, int placement, int left, int top, int right, int bottom, byte[] imageData)
```


Grafiğe bir şekil ekle. Tüm birim, grafik alanının 1/4000'idir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| type | int | [MsoDrawingType](../../com.aspose.cells/msodrawingtype). Çizim türü. |
| placement | int | [PlacementType](../../com.aspose.cells/placementtype). yerleştirme türü. |
| sol | int | Birim olarak 1/4000 grafik alanı genişliği. |
| üst | int | Birim olarak 1/4000 grafik alanı yüksekliği. |
| sağ | int | Birim olarak 1/4000 grafik alanı genişliği. |
| alt | int | Birim olarak 1/4000 grafik alanı yüksekliği. |
| imageData | byte[] | Şekil bir resim veya ole nesnesi değilse,imageData null olmalıdır. |

**Returns:**
[Shape](../../com.aspose.cells/shape)
### addShapeInChartByScale(int type, int placement, double left, double top, double right, double bottom) {#addShapeInChartByScale-int-int-double-double-double-double-}
```
public Shape addShapeInChartByScale(int type, int placement, double left, double top, double right, double bottom)
```


Grafiğe bir şekil ekleyin. Tüm birimler grafik alanının yüzde ölçeğidir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| type | int | [MsoDrawingType](../../com.aspose.cells/msodrawingtype). Çizim türü. |
| placement | int | [PlacementType](../../com.aspose.cells/placementtype). yerleştirme türü. |
| sol | double | Birim, grafik alanı genişliğinin yüzde ölçeğidir. |
| üst | double | Birim, grafik alanı yüksekliğinin yüzde ölçeğidir. |
| sağ | double | Birim, grafik alanı genişliğinin yüzde ölçeğidir. |
| alt | double | Birim, grafik alanı yüksekliğinin yüzde ölçeğidir. |

**Returns:**
[Shape](../../com.aspose.cells/shape)
### addShapeInChartByScale(int type, int placement, double left, double top, double right, double bottom, byte[] imageData) {#addShapeInChartByScale-int-int-double-double-double-double-byte---}
```
public Shape addShapeInChartByScale(int type, int placement, double left, double top, double right, double bottom, byte[] imageData)
```


Grafiğe bir şekil ekle. Tüm birim, grafik alanının 1/4000'idir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| type | int | [MsoDrawingType](../../com.aspose.cells/msodrawingtype). Çizim türü. |
| placement | int | [PlacementType](../../com.aspose.cells/placementtype). yerleştirme türü. |
| sol | double | Birim, grafik alanı genişliğinin yüzde ölçeğidir. |
| üst | double | Birim, grafik alanı yüksekliğinin yüzde ölçeğidir. |
| sağ | double | Birim, grafik alanı genişliğinin yüzde ölçeğidir. |
| alt | double | Birim, grafik alanı yüksekliğinin yüzde ölçeğidir. |
| imageData | byte[] | Şekil bir resim veya ole nesnesi değilse,imageData null olmalıdır. |

**Returns:**
[Shape](../../com.aspose.cells/shape)
### addSignatureLine(int topRow, int leftColumn, SignatureLine signatureLine) {#addSignatureLine-int-int-com.aspose.cells.SignatureLine-}
```
public Picture addSignatureLine(int topRow, int leftColumn, SignatureLine signatureLine)
```


Çalışma sayfasına bir Signature Line ekler.

**Example**

```
         SignatureLine wSignatureLine = new SignatureLine();
         wSignatureLine.setAllowComments(true);
         wSignatureLine.setEmail("example@example.com");
         wSignatureLine.setInstructions("Sign to confirm the excel content.");
         wSignatureLine.setLine(true);
         wSignatureLine.setShowSignedDate(true);
         wSignatureLine.setSigner("User");
         wSignatureLine.setTitle("tester");
         //wSignatureLine.SignatureLineType = SignatureType.Stamp;
         Picture signatureLine1 = shapes.addSignatureLine(0, 0, wSignatureLine);
```

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| üstSatır | int | Üst sol satır indeksi. |
| leftColumn | int | Üst sol sütun indeksi. |
| signatureLine | [SignatureLine](../../com.aspose.cells/signatureline) | Bir imza satırı nesnesini temsil eder. |

**Returns:**
[Picture](../../com.aspose.cells/picture) - 
### addSpinner(int topRow, int top, int leftColumn, int left, int height, int width) {#addSpinner-int-int-int-int-int-int-}
```
public Spinner addSpinner(int topRow, int top, int leftColumn, int left, int height, int width)
```


Çalışma sayfasına bir Spinner ekler.

**Example**

```
         //add a spinner
         Spinner spinner = shapes.addSpinner(1, 0, 1, 0, 100, 50);
```

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| üstSatır | int | Üst sol satır indeksi. |
| üst | int | Spinner'ın sol satırından dikey ofseti temsil eder, birim piksel olarak. |
| leftColumn | int | Üst sol sütun indeksi. |
| sol | int | Spinner'ın sol sütunundan yatay ofseti temsil eder, birim piksel olarak. |
| yükseklik | int | Spinner yüksekliğini temsil eder, birim piksel olarak. |
| genişlik | int | Spinner genişliğini temsil eder, birim piksel olarak. |

**Returns:**
[Spinner](../../com.aspose.cells/spinner) - A Spinner object.
### addSvg(int topRow, int top, int leftColumn, int left, int height, int width, byte[] svgData, byte[] compatibleImageData) {#addSvg-int-int-int-int-int-int-byte---byte---}
```
public Picture addSvg(int topRow, int top, int leftColumn, int left, int height, int width, byte[] svgData, byte[] compatibleImageData)
```


SVG görüntüsü ekler.

**Example**

```
         // add a svg
         FileInputStream fs = new FileInputStream("image.svg");
         try //JAVA: was using
         {
             int len = (int)fs.available();
             byte[] imageData = new byte[len];
             fs.read(imageData, 0, len);
             Picture picture = shapes.addSvg(4, 0, 5, 0, -1, -1, imageData, null);
         }
         finally { if (fs != null) fs.close(); }
```

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| üstSatır | int | Üst sol satır indeksi. |
| üst | int | Şeklin sol satırından dikey ofseti, piksel biriminde temsil eder. |
| leftColumn | int | Üst sol sütun indeksi. |
| sol | int | Şeklin sol sütunundan yatay ofseti, piksel biriminde. |
| yükseklik | int | Şeklin yüksekliği, piksel biriminde. |
| genişlik | int | Şeklin genişliği, piksel biriminde. |
| svgData | byte[] | Svg görüntü verisi. |
| compatibleImageData | byte[] | Excel 2016 veya daha düşük sürümlerle uyumlu olması için svg'den dönüştürülmüş görüntü verisi. |

**Returns:**
[Picture](../../com.aspose.cells/picture) - 
### addTextBox(int topRow, int top, int leftColumn, int left, int height, int width) {#addTextBox-int-int-int-int-int-int-}
```
public TextBox addTextBox(int topRow, int top, int leftColumn, int left, int height, int width)
```


Çalışma sayfasına bir metin kutusu ekler.

**Example**

```
         //add a TextBox
         TextBox textBox = shapes.addTextBox(1, 0, 1, 0, 100, 50);
```

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| üstSatır | int | Üst sol satır indeksi. |
| üst | int | textbox'ın üst satırından dikey ofseti temsil eder, birim piksel olarak. |
| leftColumn | int | Üst sol sütun indeksi. |
| sol | int | Metin kutusunun sol sütunundan yatay ofsetini, piksel biriminde temsil eder. |
| yükseklik | int | Metin kutusunun yüksekliğini temsil eder, piksel biriminde. |
| genişlik | int | Metin kutusunun genişliğini temsil eder, piksel biriminde. |

**Returns:**
[TextBox](../../com.aspose.cells/textbox) - A [TextBox](../../com.aspose.cells/textbox) object.
### addTextBoxInChart(int top, int left, int height, int width) {#addTextBoxInChart-int-int-int-int-}
```
public TextBox addTextBoxInChart(int top, int left, int height, int width)
```


Grafiğe bir metin kutusu ekler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| üst | int | Metin kutusunun sol üst köşesinden dikey ofsetini, grafik alanının 1/4000 biriminde temsil eder. |
| sol | int | Metin kutusunun sol üst köşesinden dikey ofsetini, grafik alanının 1/4000 biriminde temsil eder. |
| yükseklik | int | Metin kutusunun yüksekliğini, grafik alanının 1/4000 biriminde temsil eder. |
| genişlik | int | Metin kutusunun genişliğini, grafik alanının 1/4000 biriminde temsil eder. |

**Returns:**
[TextBox](../../com.aspose.cells/textbox) - A TextBox object.
### addTextEffect(int effect, String text, String fontName, int size, boolean fontBold, boolean fontItalic, int topRow, int top, int leftColumn, int left, int height, int width) {#addTextEffect-int-java.lang.String-java.lang.String-int-boolean-boolean-int-int-int-int-int-int-}
```
public Shape addTextEffect(int effect, String text, String fontName, int size, boolean fontBold, boolean fontItalic, int topRow, int top, int leftColumn, int left, int height, int width)
```


Bir WordArt nesnesi ekler.

**Example**

```
         //add a WordArt
         Shape wordArt1 = shapes.addTextEffect(MsoPresetTextEffect.TEXT_EFFECT_10, "WordArt", "arial", 18, false, false, 3, 0, 3, 0, 200, 50);
```

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| effect | int | [MsoPresetTextEffect](../../com.aspose.cells/msopresettexteffect). mso ön ayarlı metin efekti türü. |
| metin | java.lang.String | WordArt metni. |
| fontName | java.lang.String | Yazı tipi adı. |
| boyut | int | Yazı tipi boyutu |
| fontBold | boolean | Yazı tipinin kalın olup olmadığını gösterir. |
| fontItalic | boolean | Yazı tipinin italik olup olmadığını gösterir. |
| üstSatır | int | Üst sol satır indeksi. |
| üst | int | Şeklin sol satırından dikey ofseti, piksel biriminde temsil eder. |
| leftColumn | int | Üst sol sütun indeksi. |
| sol | int | Şeklin sol sütunundan yatay ofsetini temsil eder, piksel biriminde. |
| yükseklik | int | Şeklin yüksekliğini piksel biriminde temsil eder. |
| genişlik | int | Şeklin genişliğini temsil eder, piksel biriminde. |

**Returns:**
[Shape](../../com.aspose.cells/shape) - Returns a Shape object that represents the new WordArt object.
### addTextEffectInChart(int effect, String text, String fontName, int size, boolean fontBold, boolean fontItalic, int top, int left, int height, int width) {#addTextEffectInChart-int-java.lang.String-java.lang.String-int-boolean-boolean-int-int-int-int-}
```
public Shape addTextEffectInChart(int effect, String text, String fontName, int size, boolean fontBold, boolean fontItalic, int top, int left, int height, int width)
```


Grafiğe bir WordArt nesnesi ekler

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| effect | int | [MsoPresetTextEffect](../../com.aspose.cells/msopresettexteffect). mso ön ayarlı metin efekti türü. |
| metin | java.lang.String | WordArt metni. |
| fontName | java.lang.String | Yazı tipi adı. |
| boyut | int | Yazı tipi boyutu |
| fontBold | boolean | Yazı tipinin kalın olup olmadığını gösterir. |
| fontItalic | boolean | Yazı tipinin italik olup olmadığını gösterir. |
| üst | int | Şeklin sol üst köşesinden dikey kaymasını, grafik alanının 1/4000 birimiyle temsil eder. |
| sol | int | Şeklin sol üst köşesinden dikey kaymasını, grafik alanının 1/4000 birimiyle temsil eder. |
| yükseklik | int | Şeklin yüksekliğini, grafik alanının 1/4000 birimi cinsinden temsil eder. |
| genişlik | int | Şeklin genişliğini, grafik alanının 1/4000 birimi cinsinden temsil eder. |

**Returns:**
[Shape](../../com.aspose.cells/shape) - Returns a Shape object that represents the new WordArt object.
### addWordArt(int style, String text, int topRow, int top, int leftColumn, int left, int height, int width) {#addWordArt-int-java.lang.String-int-int-int-int-int-int-}
```
public Shape addWordArt(int style, String text, int topRow, int top, int leftColumn, int left, int height, int width)
```


Excel 2007'den beri önceden tanımlı WordArt ekler.s

**Example**

```
         //add a WordArt
         Shape wordArt2 = shapes.addWordArt(PresetWordArtStyle.WORD_ART_STYLE_1, "WordArt", 3, 0, 3, 0, 50, 200);
```

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| style | int | [PresetWordArtStyle](../../com.aspose.cells/presetwordartstyle). ön ayarlı WordArt Stili. |
| metin | java.lang.String | Metin. |
| üstSatır | int | Üst sol satır indeksi. |
| üst | int | Şeklin sol satırından dikey ofseti, piksel biriminde temsil eder. |
| leftColumn | int | Üst sol sütun indeksi. |
| sol | int | Şeklin sol sütunundan yatay ofsetini temsil eder, piksel biriminde. |
| yükseklik | int | Şeklin yüksekliğini piksel biriminde temsil eder. |
| genişlik | int | Şeklin genişliğini temsil eder, piksel biriminde. |

**Returns:**
[Shape](../../com.aspose.cells/shape) - 
### clear() {#clear--}
```
public void clear()
```


Çalışma sayfasındaki tüm şekilleri temizle.

**Example**

```
         if (shapes.getCount() > 0)
         {
             shapes.clear();
         }
```

### contains(Object o) {#contains-java.lang.Object-}
```
public boolean contains(Object o)
```


Örneğin bu nesneyi içerip içermediğini döndürür

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| o | java.lang.Object | test nesnesi |

**Returns:**
boolean - Örneğin bu nesneyi içerip içermediği
### copyCommentsInRange(ShapeCollection shapes, CellArea ca, int destRow, int destColumn) {#copyCommentsInRange-com.aspose.cells.ShapeCollection-com.aspose.cells.CellArea-int-int-}
```
public void copyCommentsInRange(ShapeCollection shapes, CellArea ca, int destRow, int destColumn)
```


Aralıktaki tüm yorumları kopyala.

**Example**

```
         CommentCollection comments = workbook.getWorksheets().get(0).getComments();
 
         //Add comment to cell A1
         int commentIndex = comments.add(0, 0);
         Comment comment = comments.get(commentIndex);
         comment.setNote("First note.");
         comment.getFont().setName("Times New Roman");
 
         //Add comment to cell B2
         comments.add("B2");
         comment = comments.get("B2");
         comment.setNote("Second note.");
 
         CellArea area1 = new CellArea();
         area1.StartColumn = 1;
         area1.StartRow = 1;
         area1.EndColumn = 5;
         area1.EndRow = 4;
 
         //copy
         shapes.copyCommentsInRange(shapes, area1, 5, 1);
```

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| shapes | [ShapeCollection](../../com.aspose.cells/shapecollection) | Kaynak şekiller. |
| ca | [CellArea](../../com.aspose.cells/cellarea) | Kaynak aralık. |
| destRow | int | Hedef aralık başlangıç satırı. |
| destColumn | int | Hedef aralık başlangıç sütunu. |

### copyInRange(ShapeCollection sourceShapes, CellArea ca, int destRow, int destColumn, boolean isContained) {#copyInRange-com.aspose.cells.ShapeCollection-com.aspose.cells.CellArea-int-int-boolean-}
```
public void copyInRange(ShapeCollection sourceShapes, CellArea ca, int destRow, int destColumn, boolean isContained)
```


Aralıktaki şekilleri hedef aralığa kopyala.

**Example**

```
         //add a shape
         shapes.addRectangle(2, 0, 2, 0, 130, 130);
         CellArea area2 = new CellArea();
         area2.StartColumn = 1;
         area2.StartRow = 1;
         area2.EndColumn = 5;
         area2.EndRow = 11;
 
         //copy
         shapes.copyInRange(shapes, area2, 12, 1, false);
```

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| sourceShapes | [ShapeCollection](../../com.aspose.cells/shapecollection) | Kaynak şekiller. |
| ca | [CellArea](../../com.aspose.cells/cellarea) | Kaynak aralık. |
| destRow | int | Hedef aralığın satır indeksi. |
| destColumn | int | Hedef aralığın sütunu. |
| isContained | boolean | Yalnızca aralık içinde bulunan şekilleri kopyalayıp kopyalamayacağını belirtir. Doğru ise, yalnızca aralıktaki şekilleri kopyalar. Aksi takdirde, MS Office gibi çalışır. |

### deleteInRange(CellArea ca) {#deleteInRange-com.aspose.cells.CellArea-}
```
public void deleteInRange(CellArea ca)
```


Aralıktaki şekilleri sil. Yorum şekilleri silinmeyecek.

**Example**

```
         //add first shape
         shapes.addRectangle(2, 0, 2, 0, 50, 50);
         //add second shape
         shapes.addRectangle(6, 0, 2, 0, 30, 30);
 
         CellArea area3 = new CellArea();
         area3.StartColumn = 0;
         area3.StartRow = 5;
         area3.EndColumn = 5;
         area3.EndRow = 8;
 
         //del
         shapes.deleteInRange(area3);
```

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| ca | [CellArea](../../com.aspose.cells/cellarea) | Aralık. Şekiller aralık içinde bulunuyorsa, kaldırılacak. |

### deleteShape(Shape shape) {#deleteShape-com.aspose.cells.Shape-}
```
public void deleteShape(Shape shape)
```


Bir şekli sil. Şekil grup içinde ise veya yorum şekli ise, silinmeyecek.

**Example**

```
         //add first shape
         Shape firstShape = shapes.addRectangle(2, 0, 2, 0, 50, 50);
         //add second shape
         Shape secondShape = shapes.addRectangle(6, 0, 2, 0, 30, 30);
         //del
         shapes.deleteShape(firstShape);
```

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| shape | [Shape](../../com.aspose.cells/shape) |  |

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
### find(String what, int previous, FindOptions findOptions) {#find-java.lang.String-int-com.aspose.cells.FindOptions-}
```
public int find(String what, int previous, FindOptions findOptions)
```


Şekli metne göre bul

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| ne | java.lang.String | Aranacak metin. |
| önceki | int | Aynı metni içeren önceki şeklin indeksi. Başlangıçtan arama yapılıyorsa -1. |
| findOptions | [FindOptions](../../com.aspose.cells/findoptions) | Bulma seçenekleri |

**Returns:**
int - Bulunan şeklin indeksi, şekil bulunamazsa -1.
### get(int index) {#get-int-}
```
public Shape get(int index)
```


Listedeki belirli indeksteki [Shape](../../com.aspose.cells/shape) nesnesini al.

**Example**

```
         //get the first shape
         Shape shape = shapes.get(0);
```

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| dizin | int | İndeks. |

**Returns:**
[Shape](../../com.aspose.cells/shape) - 
### get(String name) {#get-java.lang.String-}
```
public Shape get(String name)
```


Şeklin adıyla [Shape](../../com.aspose.cells/shape) nesnesini al.

**Example**

```
         //add a shape
         shapes.addRectangle(2, 0, 2, 0, 130, 130);
         //get the shape by the name.
         Shape shape1 = shapes.get("Rectangle 1");
         if(shape1 != null)
         {
             //Got the shape named 'Rectangle 1'.
         }
```

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| ad | java.lang.String | Şeklin adı. |

**Returns:**
[Shape](../../com.aspose.cells/shape) - 
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getCount() {#getCount--}
```
public int getCount()
```


CollectionBase örneğinde bulunan eleman sayısını alır.

**Returns:**
int - CollectionBase örneğinde bulunan eleman sayısı.
### group(Shape[] groupItems) {#group-com.aspose.cells.Shape---}
```
public GroupShape group(Shape[] groupItems)
```


Şekilleri grupla.

**Remarks**

groupItems içindeki şekil gruplanmamalıdır. Şekil bu Shapes koleksiyonunda olmalıdır.

**Example**

```
         //add first shape
         shapes.addRectangle(2, 0, 2, 0, 50, 50);
         //add second shape
         shapes.addRectangle(6, 0, 2, 0, 30, 30);
 
         Shape[] shapesArr = new Shape[] { shapes.get(0), shapes.get(1) };
         GroupShape groupShape = shapes.group(shapesArr);
```

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| groupItems | [Shape\[\]](../../com.aspose.cells/shape) | grup öğeleri. |

**Returns:**
[GroupShape](../../com.aspose.cells/groupshape) - Returns the group shape.
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### indexOf(Object o) {#indexOf-java.lang.Object-}
```
public int indexOf(Object o)
```


CollectionBase örneğindeki belirli bir öğenin dizinini belirler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| o | java.lang.Object | CollectionBase örneğindeki belirli bir öğenin dizinini belirler. |

**Returns:**
int - Değer listede bulunursa dizini; aksi takdirde -1.
### iterator() {#iterator--}
```
public Iterator iterator()
```


CollectionBase örneği üzerinde yineleme yapan bir enumerator döndürür.

**Returns:**
java.util.Iterator - CollectionBase örneği için bir iterator.
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### remove(Shape shape) {#remove-com.aspose.cells.Shape-}
```
public void remove(Shape shape)
```


Şekli kaldır.

**Example**

```
         //add first shape
         shapes.addRectangle(2, 0, 2, 0, 50, 50);
         //add second shape
         shapes.addRectangle(6, 0, 2, 0, 30, 30);
 
         //get the shape
         Shape s = shapes.get("Rectangle 1");// or shapes[0];
         if (s != null)
         {
             //remove 
             shapes.remove(s);
         }
```

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| shape | [Shape](../../com.aspose.cells/shape) |  |

### removeAt(int index) {#removeAt-int-}
```
public void removeAt(int index)
```


Şekli kaldır.

**Example**

```
         //add first shape
         shapes.addRectangle(2, 0, 2, 0, 50, 50);
         //add second shape
         shapes.addRectangle(6, 0, 2, 0, 30, 30);
 
         //remove 
         shapes.removeAt(0);
```

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| dizin | int | Şeklin indeksi. |

### toString() {#toString--}
```
public String toString()
```




**Returns:**
java.lang.String
### ungroup(GroupShape group) {#ungroup-com.aspose.cells.GroupShape-}
```
public void ungroup(GroupShape group)
```


Şekil öğelerinin grubunu çöz.

**Remarks**

Grup şekli başka bir grup şekli tarafından gruplanmışsa, hiçbir şey yapılmaz.

**Example**

```
         //add first shape
         shapes.addRectangle(2, 0, 2, 0, 50, 50);
         //add second shape
         shapes.addRectangle(6, 0, 2, 0, 30, 30);
 
         //group
         Shape[] shapesArr = new Shape[] { shapes.get(0), shapes.get(1) };
         GroupShape groupShape = shapes.group(shapesArr);
 
         //ungroup
         shapes.ungroup(groupShape);
```

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| group | [GroupShape](../../com.aspose.cells/groupshape) | Grup şekli. |

### updateSelectedValue() {#updateSelectedValue--}
```
public void updateSelectedValue()
```


Şeklin bağlı hücre veya aralığının değeriyle seçili değeri güncelle.

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

