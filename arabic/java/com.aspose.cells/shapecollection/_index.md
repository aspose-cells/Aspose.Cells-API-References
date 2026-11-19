---
title: "ShapeCollection"
second_title: "Aspose.Cells for Java API Reference"
description: "يمثل جميع الأشكال في ورقة العمل/المخطط."
type: docs
url: /ar/java/com.aspose.cells/shapecollection/
---

**Inheritance:**
java.lang.Object، [com.aspose.cells.CollectionBase](../../com.aspose.cells/collectionbase)
```
public class ShapeCollection extends CollectionBase
```

يمثل جميع الأشكال في ورقة العمل/المخطط.

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
## الطرق

| طريقة | الوصف |
| --- | --- |
| [add(Object o)](#add-java.lang.Object-) | يضيف عنصرًا إلى مثيل CollectionBase. |
| [addActiveXControl(int type, int topRow, int top, int leftColumn, int left, int width, int height)](#addActiveXControl-int-int-int-int-int-int-int-) | ينشئ عنصر تحكم Activex. |
| [addArc(int topRow, int top, int leftColumn, int left, int height, int width)](#addArc-int-int-int-int-int-int-) | يضيف ArcShape إلى ورقة العمل. |
| [addAutoShape(int type, int topRow, int top, int leftColumn, int left, int height, int width)](#addAutoShape-int-int-int-int-int-int-int-) | يضيف AutoShape إلى ورقة العمل. |
| [addAutoShapeInChart(int type, int top, int left, int height, int width)](#addAutoShapeInChart-int-int-int-int-int-) | يضيف AutoShape إلى المخطط. |
| [addButton(int topRow, int top, int leftColumn, int left, int height, int width)](#addButton-int-int-int-int-int-int-) | يضيف زر Button إلى ورقة العمل. |
| [addCheckBox(int topRow, int top, int leftColumn, int left, int height, int width)](#addCheckBox-int-int-int-int-int-int-) | يضيف خانة اختيار إلى ورقة العمل. |
| [addComboBox(int topRow, int top, int leftColumn, int left, int height, int width)](#addComboBox-int-int-int-int-int-int-) | يضيف مربع اختيار ComboBox إلى ورقة العمل. |
| [addCopy(Shape sourceShape, int topRow, int top, int leftColumn, int left)](#addCopy-com.aspose.cells.Shape-int-int-int-int-) | يضيف وينسخ شكلًا إلى ورقة العمل. |
| [addCopy(Shape sourceShape, int topRow, int top, int leftColumn, int left, CopyOptions copyOptions)](#addCopy-com.aspose.cells.Shape-int-int-int-int-com.aspose.cells.CopyOptions-) | يضيف وينسخ شكلًا إلى ورقة العمل. |
| [addEquation(int topRow, int top, int leftColumn, int left, int height, int width)](#addEquation-int-int-int-int-int-int-) | يضيف كائن معادلة إلى ورقة العمل. |
| [addFreeFloatingShape(int type, int top, int left, int height, int width, byte[] imageData, boolean isOriginalSize)](#addFreeFloatingShape-int-int-int-int-int-byte---boolean-) | يضيف شكلًا عائمًا حرًا إلى ورقة العمل.ينطبق فقط على شكل الخط/الصورة. |
| [addFreeform(int topRow, int top, int leftColumn, int left, int height, int width, ShapePath[] paths)](#addFreeform-int-int-int-int-int-int-com.aspose.cells.ShapePath---) | يضيف شكلًا حر الشكل إلى ورقة العمل. |
| [addGroupBox(int topRow, int top, int leftColumn, int left, int height, int width)](#addGroupBox-int-int-int-int-int-int-) | يضيف مجموعة GroupBox إلى ورقة العمل. |
| [addIcons(int topRow, int top, int leftColumn, int left, int height, int width, byte[] imageByteData, byte[] compatibleImageData)](#addIcons-int-int-int-int-int-int-byte---byte---) | يضيف صورة svg. |
| [addLaTeXEquation(int topRow, int top, int leftColumn, int left, int height, int width, String latex)](#addLaTeXEquation-int-int-int-int-int-int-java.lang.String-) | يضيف كائن معادلة إلى ورقة العمل باستخدام سلاسل تنسيق LaTeX. |
| [addLabel(int topRow, int top, int leftColumn, int left, int height, int width)](#addLabel-int-int-int-int-int-int-) | يضيف تسمية Label إلى ورقة العمل. |
| [addLabelInChart(int top, int left, int height, int width)](#addLabelInChart-int-int-int-int-) | يضيف تسمية إلى المخطط. |
| [addLine(int topRow, int top, int leftColumn, int left, int height, int width)](#addLine-int-int-int-int-int-int-) | يضيف شكل خط LineShape إلى ورقة العمل. |
| [addLinkedPicture(int topRow, int leftColumn, int height, int width, String sourceFullName)](#addLinkedPicture-int-int-int-int-java.lang.String-) | أضف صورة مرتبطة. |
| [addListBox(int topRow, int top, int leftColumn, int left, int height, int width)](#addListBox-int-int-int-int-int-int-) | يضيف مربع قائمة ListBox إلى ورقة العمل. |
| [addOleObject(int topRow, int top, int leftColumn, int left, int height, int width, byte[] imageData)](#addOleObject-int-int-int-int-int-int-byte---) | يضيف كائن OleObject. |
| [addOleObjectWithLinkedImage(int topRow, int leftColumn, int height, int width, String sourceFullName)](#addOleObjectWithLinkedImage-int-int-int-int-java.lang.String-) | أضف صورة مرتبطة. |
| [addOval(int topRow, int top, int leftColumn, int left, int height, int width)](#addOval-int-int-int-int-int-int-) | يضيف شكل بيضاوي Oval إلى ورقة العمل. |
| [addPicture(int topRow, int leftColumn, int bottomRow, int rightColumn, InputStream stream)](#addPicture-int-int-int-int-java.io.InputStream-) | يضيف صورة إلى المجموعة. |
| [addPicture(int topRow, int leftColumn, InputStream stream, int widthScale, int heightScale)](#addPicture-int-int-java.io.InputStream-int-int-) | يضيف صورة إلى المجموعة. |
| [addPictureInChart(int top, int left, InputStream stream, int widthScale, int heightScale)](#addPictureInChart-int-int-java.io.InputStream-int-int-) | يضيف صورة إلى المخطط. |
| [addRadioButton(int topRow, int top, int leftColumn, int left, int height, int width)](#addRadioButton-int-int-int-int-int-int-) | يضيف زر اختيار RadioButton إلى ورقة العمل. |
| [addRectangle(int topRow, int top, int leftColumn, int left, int height, int width)](#addRectangle-int-int-int-int-int-int-) | يضيف RectangleShape إلى ورقة العمل. |
| [addScrollBar(int topRow, int top, int leftColumn, int left, int height, int width)](#addScrollBar-int-int-int-int-int-int-) | يضيف ScrollBar إلى ورقة العمل. |
| [addShape(int type, int topRow, int top, int leftColumn, int left, int height, int width)](#addShape-int-int-int-int-int-int-int-) | يضيف Shape إلى ورقة العمل. |
| [addShapeInChart(int type, int placement, int left, int top, int right, int bottom)](#addShapeInChart-int-int-int-int-int-int-) | أضف شكلًا إلى المخطط. كل وحدة هي 1/4000 من مساحة المخطط. |
| [addShapeInChart(int type, int placement, int left, int top, int right, int bottom, byte[] imageData)](#addShapeInChart-int-int-int-int-int-int-byte---) | أضف شكلًا إلى المخطط. كل وحدة هي 1/4000 من مساحة المخطط. |
| [addShapeInChartByScale(int type, int placement, double left, double top, double right, double bottom)](#addShapeInChartByScale-int-int-double-double-double-double-) | أضف شكلًا إلى المخطط. |
| [addShapeInChartByScale(int type, int placement, double left, double top, double right, double bottom, byte[] imageData)](#addShapeInChartByScale-int-int-double-double-double-double-byte---) | أضف شكلًا إلى المخطط. كل وحدة هي 1/4000 من مساحة المخطط. |
| [addSignatureLine(int topRow, int leftColumn, SignatureLine signatureLine)](#addSignatureLine-int-int-com.aspose.cells.SignatureLine-) | يضيف سطر توقيع إلى ورقة العمل. |
| [addSpinner(int topRow, int top, int leftColumn, int left, int height, int width)](#addSpinner-int-int-int-int-int-int-) | يضيف Spinner إلى ورقة العمل. |
| [addSvg(int topRow, int top, int leftColumn, int left, int height, int width, byte[] svgData, byte[] compatibleImageData)](#addSvg-int-int-int-int-int-int-byte---byte---) | يضيف صورة svg. |
| [addTextBox(int topRow, int top, int leftColumn, int left, int height, int width)](#addTextBox-int-int-int-int-int-int-) | يضيف مربع نص إلى ورقة العمل. |
| [addTextBoxInChart(int top, int left, int height, int width)](#addTextBoxInChart-int-int-int-int-) | يضيف مربع نص إلى المخطط. |
| [addTextEffect(int effect, String text, String fontName, int size, boolean fontBold, boolean fontItalic, int topRow, int top, int leftColumn, int left, int height, int width)](#addTextEffect-int-java.lang.String-java.lang.String-int-boolean-boolean-int-int-int-int-int-int-) | يدرج كائن WordArt. |
| [addTextEffectInChart(int effect, String text, String fontName, int size, boolean fontBold, boolean fontItalic, int top, int left, int height, int width)](#addTextEffectInChart-int-java.lang.String-java.lang.String-int-boolean-boolean-int-int-int-int-) | يدرج كائن WordArt إلى المخطط. |
| [addWordArt(int style, String text, int topRow, int top, int leftColumn, int left, int height, int width)](#addWordArt-int-java.lang.String-int-int-int-int-int-int-) | يضيف WordArt مسبق الإعداد منذ Excel 2007. |
| [clear()](#clear--) | امسح جميع الأشكال في ورقة العمل. |
| [contains(Object o)](#contains-java.lang.Object-) | إرجاع ما إذا كان المثيل يحتوي على هذا الكائن |
| [copyCommentsInRange(ShapeCollection shapes, CellArea ca, int destRow, int destColumn)](#copyCommentsInRange-com.aspose.cells.ShapeCollection-com.aspose.cells.CellArea-int-int-) | انسخ جميع التعليقات في النطاق. |
| [copyInRange(ShapeCollection sourceShapes, CellArea ca, int destRow, int destColumn, boolean isContained)](#copyInRange-com.aspose.cells.ShapeCollection-com.aspose.cells.CellArea-int-int-boolean-) | انسخ الأشكال في النطاق إلى النطاق الوجهة. |
| [deleteInRange(CellArea ca)](#deleteInRange-com.aspose.cells.CellArea-) | احذف الأشكال في النطاق. لن يتم حذف أشكال التعليق. |
| [deleteShape(Shape shape)](#deleteShape-com.aspose.cells.Shape-) | احذف شكلًا. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [find(String what, int previous, FindOptions findOptions)](#find-java.lang.String-int-com.aspose.cells.FindOptions-) | ابحث عن شكل بالنص. |
| [get(int index)](#get-int-) | يحصل على كائن [Shape](../../com.aspose.cells/shape) في الفهرس المحدد في القائمة. |
| [get(String name)](#get-java.lang.String-) | يحصل على كائن [Shape](../../com.aspose.cells/shape) حسب اسم الشكل. |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | يحصل على عدد العناصر الموجودة في مثيل CollectionBase. |
| [group(Shape[] groupItems)](#group-com.aspose.cells.Shape---) | قم بتجميع الأشكال. |
| [hashCode()](#hashCode--) |  |
| [indexOf(Object o)](#indexOf-java.lang.Object-) | يحدد فهرس عنصر محدد في مثيل CollectionBase. |
| [iterator()](#iterator--) | يرجع كائن تعداد يتنقل عبر مثيل CollectionBase. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [remove(Shape shape)](#remove-com.aspose.cells.Shape-) | أزل الشكل. |
| [removeAt(int index)](#removeAt-int-) | أزل الشكل. |
| [toString()](#toString--) |  |
| [ungroup(GroupShape group)](#ungroup-com.aspose.cells.GroupShape-) | افك تجميع عناصر الشكل. |
| [updateSelectedValue()](#updateSelectedValue--) | حدّث القيمة المحددة بقيمة الخلية المرتبطة أو نطاق الشكل. |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### add(Object o) {#add-java.lang.Object-}
```
public int add(Object o)
```


يضيف عنصرًا إلى مثيل CollectionBase.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| o | java.lang.Object | الكائن لإضافته إلى مثيل CollectionBase. |

**Returns:**
int - الموضع الذي تم إدراج العنصر الجديد فيه.
### addActiveXControl(int type, int topRow, int top, int leftColumn, int left, int width, int height) {#addActiveXControl-int-int-int-int-int-int-int-}
```
public Shape addActiveXControl(int type, int topRow, int top, int leftColumn, int left, int width, int height)
```


ينشئ عنصر تحكم Activex.

**Example**

```
         //add an ActiveX control
         Shape activeXControl = shapes.addActiveXControl(com.aspose.cells.ControlType.CHECK_BOX, 1, 0, 1, 0, 100, 50);
```

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| type | int | [ControlType](../../com.aspose.cells/controltype). نوع التحكم. |
| topRow | int | فهرس الصف العلوي الأيسر. |
| أعلى | int | يمثل الإزاحة العمودية للـShape من صفه الأيسر، بوحدة البكسل. |
| leftColumn | int | فهرس العمود العلوي الأيسر. |
| يسار | int | يمثل الإزاحة الأفقية للـShape من عموده الأيسر، بوحدة البكسل. |
| العرض | int | يمثل عرض الـShape، بوحدة البكسل. |
| الارتفاع | int | يمثل ارتفاع الـShape، بوحدة البكسل. |

**Returns:**
[Shape](../../com.aspose.cells/shape) - 
### addArc(int topRow, int top, int leftColumn, int left, int height, int width) {#addArc-int-int-int-int-int-int-}
```
public ArcShape addArc(int topRow, int top, int leftColumn, int left, int height, int width)
```


يضيف ArcShape إلى ورقة العمل.

**Example**

```
         //add a arc
         ArcShape arcShape = shapes.addArc(1, 0, 1, 0, 100, 50);
```

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| topRow | int | فهرس الصف العلوي الأيسر. |
| أعلى | int | يمثل الإزاحة العمودية للـArcShape من صفه الأيسر، بوحدة البكسل. |
| leftColumn | int | فهرس العمود العلوي الأيسر. |
| يسار | int | يمثل الإزاحة الأفقية للـArcShape من عموده الأيسر، بوحدة البكسل. |
| الارتفاع | int | يمثل ارتفاع الـArcShape، بوحدة البكسل. |
| العرض | int | يمثل عرض الـArcShape، بوحدة البكسل. |

**Returns:**
[ArcShape](../../com.aspose.cells/arcshape) - A ArcShape object.
### addAutoShape(int type, int topRow, int top, int leftColumn, int left, int height, int width) {#addAutoShape-int-int-int-int-int-int-int-}
```
public Shape addAutoShape(int type, int topRow, int top, int leftColumn, int left, int height, int width)
```


يضيف AutoShape إلى ورقة العمل.

**Remarks**

لا يمكن أن يكون النوع Chart/Comment/Picture/OleObject/Polygon/DialogBox

**Example**

```
         //Adds a AutoShape to the worksheet.
         Shape autoShape = shapes.addAutoShape(AutoShapeType.CUBE, 1, 0, 1, 0, 100, 50);
```

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| type | int | [AutoShapeType](../../com.aspose.cells/autoshapetype). نوع الشكل التلقائي. |
| topRow | int | فهرس الصف العلوي الأيسر. |
| أعلى | int | يمثل الإزاحة العمودية للـShape من صفه الأيسر، بوحدة البكسل. |
| leftColumn | int | فهرس العمود العلوي الأيسر. |
| يسار | int | يمثل الإزاحة الأفقية للـShape من عموده الأيسر، بوحدة البكسل. |
| الارتفاع | int | يمثل ارتفاع الـShape، بوحدة البكسل. |
| العرض | int | يمثل عرض الـShape، بوحدة البكسل. |

**Returns:**
[Shape](../../com.aspose.cells/shape) - A Shape object.
### addAutoShapeInChart(int type, int top, int left, int height, int width) {#addAutoShapeInChart-int-int-int-int-int-}
```
public Shape addAutoShapeInChart(int type, int top, int left, int height, int width)
```


يضيف AutoShape إلى المخطط.

**Remarks**

لا يمكن أن يكون النوع Chart/Comment/Picture/OleObject/Polygon/DialogBox

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| type | int | [AutoShapeType](../../com.aspose.cells/autoshapetype). نوع الشكل التلقائي. |
| أعلى | int | يمثل الإزاحة العمودية للـtextbox من الزاوية العلوية اليسرى بوحدات 1/4000 من مساحة المخطط. |
| يسار | int | يمثل الإزاحة العمودية للـtextbox من الزاوية العلوية اليسرى بوحدات 1/4000 من مساحة المخطط. |
| الارتفاع | int | يمثل ارتفاع الـtextbox، بوحدات 1/4000 من مساحة المخطط. |
| العرض | int | يمثل عرض الـtextbox، بوحدات 1/4000 من مساحة المخطط. |

**Returns:**
[Shape](../../com.aspose.cells/shape) - Returns a shape object.
### addButton(int topRow, int top, int leftColumn, int left, int height, int width) {#addButton-int-int-int-int-int-int-}
```
public Button addButton(int topRow, int top, int leftColumn, int left, int height, int width)
```


يضيف زر Button إلى ورقة العمل.

**Example**

```
         //add a button
         Button button = shapes.addButton(1, 0, 1, 0, 100, 50);
```

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| topRow | int | فهرس الصف العلوي الأيسر. |
| أعلى | int | يمثل الإزاحة العمودية للـButton من صفه الأيسر، بوحدة البكسل. |
| leftColumn | int | فهرس العمود العلوي الأيسر. |
| يسار | int | يمثل الإزاحة الأفقية للـButton من عموده الأيسر، بوحدة البكسل. |
| الارتفاع | int | يمثل ارتفاع الـButton، بوحدة البكسل. |
| العرض | int | يمثل عرض الـButton، بوحدة البكسل. |

**Returns:**
[Button](../../com.aspose.cells/button) - A Button object.
### addCheckBox(int topRow, int top, int leftColumn, int left, int height, int width) {#addCheckBox-int-int-int-int-int-int-}
```
public CheckBox addCheckBox(int topRow, int top, int leftColumn, int left, int height, int width)
```


يضيف خانة اختيار إلى ورقة العمل.

**Example**

```
         //add a CheckBox
         CheckBox checkBox = shapes.addCheckBox(1, 0, 1, 0, 100, 50);
```

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| topRow | int | فهرس الصف العلوي الأيسر. |
| أعلى | int | يمثل الإزاحة العمودية للـcheckbox من صفه العلوي، بوحدة البكسل. |
| leftColumn | int | فهرس العمود العلوي الأيسر. |
| يسار | int | يمثل الإزاحة الأفقية للـtextbox من عموده الأيسر، بوحدة البكسل. |
| الارتفاع | int | ارتفاع الـtextbox، بوحدة البكسل. |
| العرض | int | عرض الـtextbox، بوحدة البكسل. |

**Returns:**
[CheckBox](../../com.aspose.cells/checkbox) - The new CheckBox object index.
### addComboBox(int topRow, int top, int leftColumn, int left, int height, int width) {#addComboBox-int-int-int-int-int-int-}
```
public ComboBox addComboBox(int topRow, int top, int leftColumn, int left, int height, int width)
```


يضيف مربع اختيار ComboBox إلى ورقة العمل.

**Example**

```
         //add a combo box
         ComboBox comboBox = shapes.addComboBox(1, 0, 1, 0, 100, 50);
```

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| topRow | int | فهرس الصف العلوي الأيسر. |
| أعلى | int | يمثل الإزاحة العمودية للـComboBox من صفه الأيسر، بوحدة البكسل. |
| leftColumn | int | فهرس العمود العلوي الأيسر. |
| يسار | int | يمثل الإزاحة الأفقية للـComboBox من عموده الأيسر، بوحدة البكسل. |
| الارتفاع | int | يمثل ارتفاع ComboBox، بوحدة البكسل. |
| العرض | int | يمثل عرض ComboBox، بوحدة البكسل. |

**Returns:**
[ComboBox](../../com.aspose.cells/combobox) - A ComboBox object.
### addCopy(Shape sourceShape, int topRow, int top, int leftColumn, int left) {#addCopy-com.aspose.cells.Shape-int-int-int-int-}
```
public Shape addCopy(Shape sourceShape, int topRow, int top, int leftColumn, int left)
```


يضيف وينسخ شكلًا إلى ورقة العمل.

**Example**

```
         //add a shape
         RectangleShape rectangle = shapes.addRectangle(2, 0, 2, 0, 130, 130);
         //Adds and copies a shape.
         shapes.addCopy(rectangle, 7, 0, 7, 0);
```

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| sourceShape | [Shape](../../com.aspose.cells/shape) | الشكل المصدر. |
| topRow | int | فهرس الصف العلوي. |
| أعلى | int | يمثل الإزاحة العمودية من صفه العلوي، بوحدة البكسل. |
| leftColumn | int | فهرس العمود الأيسر. |
| يسار | int | يمثل الإزاحة الأفقية من عموده الأيسر، بوحدة البكسل. |

**Returns:**
[Shape](../../com.aspose.cells/shape) - The new [Shape](../../com.aspose.cells/shape) object.
### addCopy(Shape sourceShape, int topRow, int top, int leftColumn, int left, CopyOptions copyOptions) {#addCopy-com.aspose.cells.Shape-int-int-int-int-com.aspose.cells.CopyOptions-}
```
public Shape addCopy(Shape sourceShape, int topRow, int top, int leftColumn, int left, CopyOptions copyOptions)
```


يضيف وينسخ شكلًا إلى ورقة العمل.

**Example**

```
         //add a shape
         RectangleShape rectangle = shapes.addRectangle(2, 0, 2, 0, 130, 130);
         //Adds and copies a shape.
         shapes.addCopy(rectangle, 7, 0, 7, 0);
```

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| sourceShape | [Shape](../../com.aspose.cells/shape) | الشكل المصدر. |
| topRow | int | فهرس الصف العلوي. |
| أعلى | int | يمثل الإزاحة العمودية من صفه العلوي، بوحدة البكسل. |
| leftColumn | int | فهرس العمود الأيسر. |
| يسار | int | يمثل الإزاحة الأفقية من عموده الأيسر، بوحدة البكسل. |
| copyOptions | [CopyOptions](../../com.aspose.cells/copyoptions) | خيارات نسخ الأشكال. |

**Returns:**
[Shape](../../com.aspose.cells/shape) - The new [Shape](../../com.aspose.cells/shape) object.
### addEquation(int topRow, int top, int leftColumn, int left, int height, int width) {#addEquation-int-int-int-int-int-int-}
```
public TextBox addEquation(int topRow, int top, int leftColumn, int left, int height, int width)
```


يضيف كائن معادلة إلى ورقة العمل.

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
| معامل | نوع | الوصف |
| --- | --- | --- |
| topRow | int | فهرس الصف العلوي. |
| أعلى | int | الإزاحة العمودية صفه العلوي، بوحدة البكسل. |
| leftColumn | int | فهرس العمود الأيسر. |
| يسار | int | الإزاحة الأفقية من عموده الأيسر، بوحدة البكسل. |
| الارتفاع | int | ارتفاع المعادلة، بوحدة البكسل. |
| العرض | int | عرض المعادلة، بوحدة البكسل. |

**Returns:**
[TextBox](../../com.aspose.cells/textbox) - 
### addFreeFloatingShape(int type, int top, int left, int height, int width, byte[] imageData, boolean isOriginalSize) {#addFreeFloatingShape-int-int-int-int-int-byte---boolean-}
```
public Shape addFreeFloatingShape(int type, int top, int left, int height, int width, byte[] imageData, boolean isOriginalSize)
```


يضيف شكلًا عائمًا حرًا إلى ورقة العمل.ينطبق فقط على شكل الخط/الصورة.

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
| معامل | نوع | الوصف |
| --- | --- | --- |
| type | int | [MsoDrawingType](../../com.aspose.cells/msodrawingtype). نوع الشكل. |
| أعلى | int | يمثل الإزاحة العمودية للشكل من الصف العلوي للورقة، بوحدة البكسل. |
| يسار | int | يمثل الإزاحة الأفقية للشكل من العمود الأيسر للورقة، بوحدة البكسل. |
| الارتفاع | int | يمثل ارتفاع LineShape، بوحدة البكسل. |
| العرض | int | يمثل عرض LineShape، بوحدة البكسل. |
| imageData | byte[] | بيانات الصورة، تنطبق فقط على الصورة. |
| isOriginalSize | boolean | ما إذا كان الشكل يستخدم الحجم الأصلي إذا كان الشكل صورة. |

**Returns:**
[Shape](../../com.aspose.cells/shape) - 
### addFreeform(int topRow, int top, int leftColumn, int left, int height, int width, ShapePath[] paths) {#addFreeform-int-int-int-int-int-int-com.aspose.cells.ShapePath---}
```
public Shape addFreeform(int topRow, int top, int leftColumn, int left, int height, int width, ShapePath[] paths)
```


يضيف شكلًا حر الشكل إلى ورقة العمل.

**Remarks**

ملاحظة: أن العرض والارتفاع في المعلمات يمكن أن يكونا أي قيم صحيحة موجبة، وليس العرض والارتفاع الكلي لمصفوفة ShapePath المحددة بـ \\u9225\\u6a96aths'. العلاقة بينهما هي علاقة ملء-مقياس، أي أن كل كائن ShapePath سيتم تحجيمه وفقًا للعرض والارتفاع. لذلك، عندما توجد عدة كائنات في 'paths'، يجب تصميم كل كائن ShapePath بشكل معقول لتلبية التوقعات. عندما يكون هناك كائن ShapePath واحد فقط ولا توجد متطلبات أخرى، فإن تمرير عرض وارتفاع الكائن كقيم للمعامل \\u9225\\u5b27\\u20ac\\u5a94s حل جيد.

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
| معامل | نوع | الوصف |
| --- | --- | --- |
| topRow | int | فهرس الصف العلوي الأيسر. |
| أعلى | int | يمثل الإزاحة العمودية للشكل الحر من صفه الأيسر، بوحدة البكسل. |
| leftColumn | int | فهرس العمود العلوي الأيسر. |
| يسار | int | يمثل الإزاحة الأفقية للشكل الحر من عموده الأيسر، بوحدة البكسل. |
| الارتفاع | int | يمثل ارتفاع الشكل الحر، بوحدة البكسل. |
| العرض | int | يمثل عرض الشكل الحر، بوحدة البكسل. |
| paths | [ShapePath\[\]](../../com.aspose.cells/shapepath) | يمثل مسارًا معرفًا من قبل المستخدم |

**Returns:**
[Shape](../../com.aspose.cells/shape) - A freeform shape.
### addGroupBox(int topRow, int top, int leftColumn, int left, int height, int width) {#addGroupBox-int-int-int-int-int-int-}
```
public GroupBox addGroupBox(int topRow, int top, int leftColumn, int left, int height, int width)
```


يضيف مجموعة GroupBox إلى ورقة العمل.

**Example**

```
         //add a group box
         GroupBox groupBox = shapes.addGroupBox(1, 0, 1, 0, 100, 50);
```

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| topRow | int | فهرس الصف العلوي الأيسر. |
| أعلى | int | يمثل الإزاحة العمودية لـ GroupBox من صفه الأيسر، بوحدة البكسل. |
| leftColumn | int | فهرس العمود العلوي الأيسر. |
| يسار | int | يمثل الإزاحة الأفقية لـ GroupBox من عموده الأيسر، بوحدة البكسل. |
| الارتفاع | int | يمثل ارتفاع GroupBox، بوحدة البكسل. |
| العرض | int | يمثل عرض GroupBox، بوحدة البكسل. |

**Returns:**
[GroupBox](../../com.aspose.cells/groupbox) - A GroupBox object.
### addIcons(int topRow, int top, int leftColumn, int left, int height, int width, byte[] imageByteData, byte[] compatibleImageData) {#addIcons-int-int-int-int-int-int-byte---byte---}
```
public Picture addIcons(int topRow, int top, int leftColumn, int left, int height, int width, byte[] imageByteData, byte[] compatibleImageData)
```


يضيف صورة svg.

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
| معامل | نوع | الوصف |
| --- | --- | --- |
| topRow | int | فهرس الصف العلوي الأيسر. |
| أعلى | int | يمثل الإزاحة العمودية للشكل من صفه الأيسر، بوحدة البكسل. |
| leftColumn | int | فهرس العمود العلوي الأيسر. |
| يسار | int | الإزاحة الأفقية للشكل من عموده الأيسر، بوحدة البكسل. |
| الارتفاع | int | ارتفاع الشكل، بوحدة البكسل. |
| العرض | int | عرض الشكل، بوحدة البكسل. |
| imageByteData | byte[] | بيانات البايت للصورة. |
| compatibleImageData | byte[] | بيانات الصورة المحولة من SVG لتكون متوافقة مع Excel 2016 أو الإصدارات الأقدم. |

**Returns:**
[Picture](../../com.aspose.cells/picture) - 
### addLaTeXEquation(int topRow, int top, int leftColumn, int left, int height, int width, String latex) {#addLaTeXEquation-int-int-int-int-int-int-java.lang.String-}
```
public TextBox addLaTeXEquation(int topRow, int top, int leftColumn, int left, int height, int width, String latex)
```


يضيف كائن معادلة إلى ورقة العمل باستخدام سلاسل تنسيق LaTeX.

**Example**

```
         // LaTeX format string.
         String latex = "\\alpha +  \\frac{\\partial^2}{\\partial x_1\\partial x_2}y - \\left ( a + b \\right )+_{a}^{b}\\beta";
         // Adds an equation object to the worksheet.
         TextBox textBox = shapes.addLaTeXEquation(1, 0, 1, 0, 100, 300, latex);
```

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| topRow | int | فهرس الصف العلوي. |
| أعلى | int | الإزاحة العمودية صفه العلوي، بوحدة البكسل. |
| leftColumn | int | فهرس العمود الأيسر. |
| يسار | int | الإزاحة الأفقية من عموده الأيسر، بوحدة البكسل. |
| الارتفاع | int | ارتفاع المعادلة، بوحدة البكسل. |
| العرض | int | عرض المعادلة، بوحدة البكسل. |
| latex | java.lang.String | سلسلة تنسيق LaTeX |

**Returns:**
[TextBox](../../com.aspose.cells/textbox) - 
### addLabel(int topRow, int top, int leftColumn, int left, int height, int width) {#addLabel-int-int-int-int-int-int-}
```
public Label addLabel(int topRow, int top, int leftColumn, int left, int height, int width)
```


يضيف تسمية Label إلى ورقة العمل.

**Example**

```
         //add a label
         Label label = shapes.addLabel(1, 0, 1, 0, 100, 50);
```

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| topRow | int | فهرس الصف العلوي الأيسر. |
| أعلى | int | يمثل الإزاحة العمودية لـ Label من صفه الأيسر، بوحدة البكسل. |
| leftColumn | int | فهرس العمود العلوي الأيسر. |
| يسار | int | يمثل الإزاحة الأفقية لـ Label من عموده الأيسر، بوحدة البكسل. |
| الارتفاع | int | يمثل ارتفاع Label، بوحدة البكسل. |
| العرض | int | يمثل عرض Label، بوحدة البكسل. |

**Returns:**
[Label](../../com.aspose.cells/label) - A Label object.
### addLabelInChart(int top, int left, int height, int width) {#addLabelInChart-int-int-int-int-}
```
public Label addLabelInChart(int top, int left, int height, int width)
```


يضيف تسمية إلى المخطط.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| أعلى | int | يمثل الإزاحة العمودية للعلامة من الزاوية العليا اليسرى بوحدات 1/4000 من مساحة المخطط. |
| يسار | int | يمثل الإزاحة العمودية للعلامة من الزاوية العليا اليسرى بوحدات 1/4000 من مساحة المخطط. |
| الارتفاع | int | يمثل ارتفاع العلامة بوحدات 1/4000 من مساحة المخطط. |
| العرض | int | يمثل عرض العلامة بوحدات 1/4000 من مساحة المخطط. |

**Returns:**
[Label](../../com.aspose.cells/label) - A new Label object.
### addLine(int topRow, int top, int leftColumn, int left, int height, int width) {#addLine-int-int-int-int-int-int-}
```
public LineShape addLine(int topRow, int top, int leftColumn, int left, int height, int width)
```


يضيف شكل خط LineShape إلى ورقة العمل.

**Example**

```
         // add a line object
         LineShape lineShape = shapes.addLine(1, 0, 1, 0, 100, 50);
```

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| topRow | int | فهرس الصف العلوي الأيسر. |
| أعلى | int | يمثل الإزاحة العمودية لـ LineShape من صفه الأيسر، بوحدة البكسل. |
| leftColumn | int | فهرس العمود العلوي الأيسر. |
| يسار | int | يمثل الإزاحة الأفقية لـ LineShape من عموده الأيسر، بوحدة البكسل. |
| الارتفاع | int | يمثل ارتفاع LineShape، بوحدة البكسل. |
| العرض | int | يمثل عرض LineShape، بوحدة البكسل. |

**Returns:**
[LineShape](../../com.aspose.cells/lineshape) - A LineShape object.
### addLinkedPicture(int topRow, int leftColumn, int height, int width, String sourceFullName) {#addLinkedPicture-int-int-int-int-java.lang.String-}
```
public Picture addLinkedPicture(int topRow, int leftColumn, int height, int width, String sourceFullName)
```


أضف صورة مرتبطة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| topRow | int | فهرس الصف العلوي الأيسر. |
| leftColumn | int | فهرس العمود العلوي الأيسر. |
| الارتفاع | int | ارتفاع الشكل. بوحدة البكسل. |
| العرض | int | عرض الشكل. بوحدة البكسل |
| sourceFullName | java.lang.String | المسار واسم ملف المصدر للصورة المرتبطة |

**Returns:**
[Picture](../../com.aspose.cells/picture) - [Picture](../../com.aspose.cells/picture) Picture object.
### addListBox(int topRow, int top, int leftColumn, int left, int height, int width) {#addListBox-int-int-int-int-int-int-}
```
public ListBox addListBox(int topRow, int top, int leftColumn, int left, int height, int width)
```


يضيف مربع قائمة ListBox إلى ورقة العمل.

**Example**

```
         //add a list box
         ListBox listBox = shapes.addListBox(1, 0, 1, 0, 100, 50);
```

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| topRow | int | فهرس الصف العلوي الأيسر. |
| أعلى | int | يمثل الإزاحة العمودية لـ ListBox من صفه الأيسر، بوحدة البكسل. |
| leftColumn | int | فهرس العمود العلوي الأيسر. |
| يسار | int | يمثل الإزاحة الأفقية لـ ListBox من عموده الأيسر، بوحدة البكسل. |
| الارتفاع | int | يمثل ارتفاع ListBox، بوحدة البكسل. |
| العرض | int | يمثل عرض ListBox، بوحدة البكسل. |

**Returns:**
[ListBox](../../com.aspose.cells/listbox) - A ListBox object.
### addOleObject(int topRow, int top, int leftColumn, int left, int height, int width, byte[] imageData) {#addOleObject-int-int-int-int-int-int-byte---}
```
public OleObject addOleObject(int topRow, int top, int leftColumn, int left, int height, int width, byte[] imageData)
```


يضيف كائن OleObject.

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
| معامل | نوع | الوصف |
| --- | --- | --- |
| topRow | int |  |
| أعلى | int |  |
| leftColumn | int |  |
| يسار | int |  |
| الارتفاع | int |  |
| العرض | int |  |
| imageData | byte[] |  |

**Returns:**
[OleObject](../../com.aspose.cells/oleobject) - 
### addOleObjectWithLinkedImage(int topRow, int leftColumn, int height, int width, String sourceFullName) {#addOleObjectWithLinkedImage-int-int-int-int-java.lang.String-}
```
public OleObject addOleObjectWithLinkedImage(int topRow, int leftColumn, int height, int width, String sourceFullName)
```


أضف صورة مرتبطة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| topRow | int | فهرس الصف العلوي الأيسر. |
| leftColumn | int | فهرس العمود العلوي الأيسر. |
| الارتفاع | int | ارتفاع الشكل. بوحدة البكسل. |
| العرض | int | عرض الشكل. بوحدة البكسل |
| sourceFullName | java.lang.String | المسار واسم ملف المصدر للصورة المرتبطة |

**Returns:**
[OleObject](../../com.aspose.cells/oleobject) - [Picture](../../com.aspose.cells/picture) Picture object.
### addOval(int topRow, int top, int leftColumn, int left, int height, int width) {#addOval-int-int-int-int-int-int-}
```
public Oval addOval(int topRow, int top, int leftColumn, int left, int height, int width)
```


يضيف شكل بيضاوي Oval إلى ورقة العمل.

**Example**

```
         //add a oval
         Oval oval = shapes.addOval(1, 0, 1, 0, 50, 50);
```

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| topRow | int | فهرس الصف العلوي الأيسر. |
| أعلى | int | يمثل الإزاحة العمودية لـ Oval من صفه الأيسر، بوحدة البكسل. |
| leftColumn | int | فهرس العمود العلوي الأيسر. |
| يسار | int | يمثل الإزاحة الأفقية لـ Oval من عموده الأيسر، بوحدة البكسل. |
| الارتفاع | int | يمثل ارتفاع Oval، بوحدة البكسل. |
| العرض | int | يمثل عرض Oval، بوحدة البكسل. |

**Returns:**
[Oval](../../com.aspose.cells/oval) - A Oval object.
### addPicture(int topRow, int leftColumn, int bottomRow, int rightColumn, InputStream stream) {#addPicture-int-int-int-int-java.io.InputStream-}
```
public Picture addPicture(int topRow, int leftColumn, int bottomRow, int rightColumn, InputStream stream)
```


يضيف صورة إلى المجموعة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| topRow | int | فهرس الصف العلوي الأيسر. |
| leftColumn | int | فهرس العمود العلوي الأيسر. |
| bottomRow | int | فهرس الصف السفلي الأيمن. |
| rightColumn | int | فهرس العمود السفلي الأيمن. |
| stream | java.io.InputStream | كائن الدفق الذي يحتوي على بيانات الصورة. |

**Returns:**
[Picture](../../com.aspose.cells/picture) - [Picture](../../com.aspose.cells/picture) Picture object.
### addPicture(int topRow, int leftColumn, InputStream stream, int widthScale, int heightScale) {#addPicture-int-int-java.io.InputStream-int-int-}
```
public Picture addPicture(int topRow, int leftColumn, InputStream stream, int widthScale, int heightScale)
```


يضيف صورة إلى المجموعة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| topRow | int | فهرس الصف العلوي الأيسر. |
| leftColumn | int | فهرس العمود العلوي الأيسر. |
| stream | java.io.InputStream | كائن الدفق الذي يحتوي على بيانات الصورة. |
| widthScale | int | مقياس عرض الصورة، كنسبة مئوية. |
| heightScale | int | مقياس ارتفاع الصورة، كنسبة مئوية. |

**Returns:**
[Picture](../../com.aspose.cells/picture) - [Picture](../../com.aspose.cells/picture) Picture object.
### addPictureInChart(int top, int left, InputStream stream, int widthScale, int heightScale) {#addPictureInChart-int-int-java.io.InputStream-int-int-}
```
public Picture addPictureInChart(int top, int left, InputStream stream, int widthScale, int heightScale)
```


يضيف صورة إلى المخطط.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| أعلى | int | يمثل الإزاحة العمودية للشكل من الزاوية العلوية اليسرى بوحدات 1/4000 من مساحة المخطط. |
| يسار | int | يمثل الإزاحة الأفقية للشكل من الزاوية العلوية اليسرى بوحدات 1/4000 من مساحة المخطط. |
| stream | java.io.InputStream | كائن الدفق الذي يحتوي على بيانات الصورة. |
| widthScale | int | مقياس عرض الصورة، كنسبة مئوية. |
| heightScale | int | مقياس ارتفاع الصورة، كنسبة مئوية. |

**Returns:**
[Picture](../../com.aspose.cells/picture) - Returns a Picture object.
### addRadioButton(int topRow, int top, int leftColumn, int left, int height, int width) {#addRadioButton-int-int-int-int-int-int-}
```
public RadioButton addRadioButton(int topRow, int top, int leftColumn, int left, int height, int width)
```


يضيف زر اختيار RadioButton إلى ورقة العمل.

**Example**

```
         //add a radio button
         RadioButton radioButton = shapes.addRadioButton(1, 0, 1, 0, 100, 50);
```

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| topRow | int | فهرس الصف العلوي الأيسر. |
| أعلى | int | يمثل الإزاحة العمودية لـ RadioButton من صفه الأيسر، بوحدة البكسل. |
| leftColumn | int | فهرس العمود العلوي الأيسر. |
| يسار | int | يمثل الإزاحة الأفقية لـ RadioButton من عموده الأيسر، بوحدة البكسل. |
| الارتفاع | int | يمثل ارتفاع RadioButton، بوحدة البكسل. |
| العرض | int | يمثل عرض RadioButton، بوحدة البكسل. |

**Returns:**
[RadioButton](../../com.aspose.cells/radiobutton) - A RadioButton object.
### addRectangle(int topRow, int top, int leftColumn, int left, int height, int width) {#addRectangle-int-int-int-int-int-int-}
```
public RectangleShape addRectangle(int topRow, int top, int leftColumn, int left, int height, int width)
```


يضيف RectangleShape إلى ورقة العمل.

**Example**

```
         // add a rectangle
         RectangleShape rectangleShape = shapes.addRectangle(2, 0, 2, 0, 130, 130);
```

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| topRow | int | فهرس الصف العلوي الأيسر. |
| أعلى | int | يمثل الإزاحة العمودية لـ RectangleShape من صفه الأيسر، بوحدة البكسل. |
| leftColumn | int | فهرس العمود العلوي الأيسر. |
| يسار | int | يمثل الإزاحة الأفقية لـ RectangleShape من عموده الأيسر، بوحدة البكسل. |
| الارتفاع | int | يمثل ارتفاع RectangleShape بوحدة البكسل. |
| العرض | int | يمثل عرض RectangleShape بوحدة البكسل. |

**Returns:**
[RectangleShape](../../com.aspose.cells/rectangleshape) - A RectangleShape object.
### addScrollBar(int topRow, int top, int leftColumn, int left, int height, int width) {#addScrollBar-int-int-int-int-int-int-}
```
public ScrollBar addScrollBar(int topRow, int top, int leftColumn, int left, int height, int width)
```


يضيف ScrollBar إلى ورقة العمل.

**Example**

```
         //add a scroll bar
         ScrollBar scrollBar = shapes.addScrollBar(1, 0, 1, 0, 100, 20);
```

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| topRow | int | فهرس الصف العلوي الأيسر. |
| أعلى | int | يمثل الإزاحة الرأسية لشريط التمرير من صفه الأيسر بوحدة البكسل. |
| leftColumn | int | فهرس العمود العلوي الأيسر. |
| يسار | int | يمثل الإزاحة الأفقية لشريط التمرير من عموده الأيسر بوحدة البكسل. |
| الارتفاع | int | يمثل ارتفاع شريط التمرير بوحدة البكسل. |
| العرض | int | يمثل عرض شريط التمرير بوحدة البكسل. |

**Returns:**
[ScrollBar](../../com.aspose.cells/scrollbar) - A ScrollBar object.
### addShape(int type, int topRow, int top, int leftColumn, int left, int height, int width) {#addShape-int-int-int-int-int-int-int-}
```
public Shape addShape(int type, int topRow, int top, int leftColumn, int left, int height, int width)
```


يضيف Shape إلى ورقة العمل.

**Remarks**

لا يمكن أن يكون النوع Chart/Comment/Picture/OleObject/Polygon/DialogBox

**Example**

```
         //Add a shape of the specified type
         Shape shapeByType = shapes.addShape(MsoDrawingType.CELLS_DRAWING, 1, 0, 1, 0, 100, 50);
```

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| type | int | [MsoDrawingType](../../com.aspose.cells/msodrawingtype). نوع رسم Mso. |
| topRow | int | فهرس الصف العلوي الأيسر. |
| أعلى | int | يمثل الإزاحة العمودية للـShape من صفه الأيسر، بوحدة البكسل. |
| leftColumn | int | فهرس العمود العلوي الأيسر. |
| يسار | int | يمثل الإزاحة الأفقية للـShape من عموده الأيسر، بوحدة البكسل. |
| الارتفاع | int | يمثل ارتفاع الـShape، بوحدة البكسل. |
| العرض | int | يمثل عرض الـShape، بوحدة البكسل. |

**Returns:**
[Shape](../../com.aspose.cells/shape) - A Shape object.
### addShapeInChart(int type, int placement, int left, int top, int right, int bottom) {#addShapeInChart-int-int-int-int-int-int-}
```
public Shape addShapeInChart(int type, int placement, int left, int top, int right, int bottom)
```


أضف شكلًا إلى المخطط. كل وحدة هي 1/4000 من مساحة المخطط.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| type | int | [MsoDrawingType](../../com.aspose.cells/msodrawingtype). نوع الرسم. |
| placement | int | [PlacementType](../../com.aspose.cells/placementtype). نوع التوضع. |
| يسار | int | بوحدة 1/4000 من عرض مساحة المخطط. |
| أعلى | int | بوحدة 1/4000 من ارتفاع مساحة المخطط. |
| يمين | int | بوحدة 1/4000 من عرض مساحة المخطط. |
| أسفل | int | بوحدة 1/4000 من ارتفاع مساحة المخطط. |

**Returns:**
[Shape](../../com.aspose.cells/shape)
### addShapeInChart(int type, int placement, int left, int top, int right, int bottom, byte[] imageData) {#addShapeInChart-int-int-int-int-int-int-byte---}
```
public Shape addShapeInChart(int type, int placement, int left, int top, int right, int bottom, byte[] imageData)
```


أضف شكلًا إلى المخطط. كل وحدة هي 1/4000 من مساحة المخطط.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| type | int | [MsoDrawingType](../../com.aspose.cells/msodrawingtype). نوع الرسم. |
| placement | int | [PlacementType](../../com.aspose.cells/placementtype). نوع التوضع. |
| يسار | int | بوحدة 1/4000 من عرض مساحة المخطط. |
| أعلى | int | بوحدة 1/4000 من ارتفاع مساحة المخطط. |
| يمين | int | بوحدة 1/4000 من عرض مساحة المخطط. |
| أسفل | int | بوحدة 1/4000 من ارتفاع مساحة المخطط. |
| imageData | byte[] | إذا لم يكن الشكل صورة أو كائن ole، يجب أن تكون imageData فارغة. |

**Returns:**
[Shape](../../com.aspose.cells/shape)
### addShapeInChartByScale(int type, int placement, double left, double top, double right, double bottom) {#addShapeInChartByScale-int-int-double-double-double-double-}
```
public Shape addShapeInChartByScale(int type, int placement, double left, double top, double right, double bottom)
```


أضف شكلاً إلى المخطط. جميع الوحدات هي نسبة مئوية من مساحة المخطط.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| type | int | [MsoDrawingType](../../com.aspose.cells/msodrawingtype). نوع الرسم. |
| placement | int | [PlacementType](../../com.aspose.cells/placementtype). نوع التوضع. |
| يسار | double | الوحدة هي نسبة مئوية من عرض مساحة المخطط. |
| أعلى | double | الوحدة هي نسبة مئوية من ارتفاع مساحة المخطط. |
| يمين | double | الوحدة هي نسبة مئوية من عرض مساحة المخطط. |
| أسفل | double | الوحدة هي نسبة مئوية من ارتفاع مساحة المخطط. |

**Returns:**
[Shape](../../com.aspose.cells/shape)
### addShapeInChartByScale(int type, int placement, double left, double top, double right, double bottom, byte[] imageData) {#addShapeInChartByScale-int-int-double-double-double-double-byte---}
```
public Shape addShapeInChartByScale(int type, int placement, double left, double top, double right, double bottom, byte[] imageData)
```


أضف شكلًا إلى المخطط. كل وحدة هي 1/4000 من مساحة المخطط.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| type | int | [MsoDrawingType](../../com.aspose.cells/msodrawingtype). نوع الرسم. |
| placement | int | [PlacementType](../../com.aspose.cells/placementtype). نوع التوضع. |
| يسار | double | الوحدة هي نسبة مئوية من عرض مساحة المخطط. |
| أعلى | double | الوحدة هي نسبة مئوية من ارتفاع مساحة المخطط. |
| يمين | double | الوحدة هي نسبة مئوية من عرض مساحة المخطط. |
| أسفل | double | الوحدة هي نسبة مئوية من ارتفاع مساحة المخطط. |
| imageData | byte[] | إذا لم يكن الشكل صورة أو كائن ole، يجب أن تكون imageData فارغة. |

**Returns:**
[Shape](../../com.aspose.cells/shape)
### addSignatureLine(int topRow, int leftColumn, SignatureLine signatureLine) {#addSignatureLine-int-int-com.aspose.cells.SignatureLine-}
```
public Picture addSignatureLine(int topRow, int leftColumn, SignatureLine signatureLine)
```


يضيف سطر توقيع إلى ورقة العمل.

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
| معامل | نوع | الوصف |
| --- | --- | --- |
| topRow | int | فهرس الصف العلوي الأيسر. |
| leftColumn | int | فهرس العمود العلوي الأيسر. |
| signatureLine | [SignatureLine](../../com.aspose.cells/signatureline) | يمثل كائن خط التوقيع. |

**Returns:**
[Picture](../../com.aspose.cells/picture) - 
### addSpinner(int topRow, int top, int leftColumn, int left, int height, int width) {#addSpinner-int-int-int-int-int-int-}
```
public Spinner addSpinner(int topRow, int top, int leftColumn, int left, int height, int width)
```


يضيف Spinner إلى ورقة العمل.

**Example**

```
         //add a spinner
         Spinner spinner = shapes.addSpinner(1, 0, 1, 0, 100, 50);
```

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| topRow | int | فهرس الصف العلوي الأيسر. |
| أعلى | int | يمثل الإزاحة الرأسية للدوار من صفه الأيسر بوحدة البكسل. |
| leftColumn | int | فهرس العمود العلوي الأيسر. |
| يسار | int | يمثل الإزاحة الأفقية للدوار من عموده الأيسر بوحدة البكسل. |
| الارتفاع | int | يمثل ارتفاع الدوار بوحدة البكسل. |
| العرض | int | يمثل عرض الدوار بوحدة البكسل. |

**Returns:**
[Spinner](../../com.aspose.cells/spinner) - A Spinner object.
### addSvg(int topRow, int top, int leftColumn, int left, int height, int width, byte[] svgData, byte[] compatibleImageData) {#addSvg-int-int-int-int-int-int-byte---byte---}
```
public Picture addSvg(int topRow, int top, int leftColumn, int left, int height, int width, byte[] svgData, byte[] compatibleImageData)
```


يضيف صورة svg.

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
| معامل | نوع | الوصف |
| --- | --- | --- |
| topRow | int | فهرس الصف العلوي الأيسر. |
| أعلى | int | يمثل الإزاحة العمودية للشكل من صفه الأيسر، بوحدة البكسل. |
| leftColumn | int | فهرس العمود العلوي الأيسر. |
| يسار | int | الإزاحة الأفقية للشكل من عموده الأيسر، بوحدة البكسل. |
| الارتفاع | int | ارتفاع الشكل، بوحدة البكسل. |
| العرض | int | عرض الشكل، بوحدة البكسل. |
| svgData | byte[] | بيانات صورة svg. |
| compatibleImageData | byte[] | بيانات الصورة المحولة من SVG لتكون متوافقة مع Excel 2016 أو الإصدارات الأقدم. |

**Returns:**
[Picture](../../com.aspose.cells/picture) - 
### addTextBox(int topRow, int top, int leftColumn, int left, int height, int width) {#addTextBox-int-int-int-int-int-int-}
```
public TextBox addTextBox(int topRow, int top, int leftColumn, int left, int height, int width)
```


يضيف مربع نص إلى ورقة العمل.

**Example**

```
         //add a TextBox
         TextBox textBox = shapes.addTextBox(1, 0, 1, 0, 100, 50);
```

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| topRow | int | فهرس الصف العلوي الأيسر. |
| أعلى | int | يمثل الإزاحة الرأسية لمربع النص من صفه العلوي بوحدة البكسل. |
| leftColumn | int | فهرس العمود العلوي الأيسر. |
| يسار | int | يمثل الإزاحة الأفقية للـtextbox من عموده الأيسر، بوحدة البكسل. |
| الارتفاع | int | يمثل ارتفاع مربع النص، بوحدة البكسل. |
| العرض | int | يمثل عرض مربع النص، بوحدة البكسل. |

**Returns:**
[TextBox](../../com.aspose.cells/textbox) - A [TextBox](../../com.aspose.cells/textbox) object.
### addTextBoxInChart(int top, int left, int height, int width) {#addTextBoxInChart-int-int-int-int-}
```
public TextBox addTextBoxInChart(int top, int left, int height, int width)
```


يضيف مربع نص إلى المخطط.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| أعلى | int | يمثل الإزاحة العمودية للـtextbox من الزاوية العلوية اليسرى بوحدات 1/4000 من مساحة المخطط. |
| يسار | int | يمثل الإزاحة العمودية للـtextbox من الزاوية العلوية اليسرى بوحدات 1/4000 من مساحة المخطط. |
| الارتفاع | int | يمثل ارتفاع الـtextbox، بوحدات 1/4000 من مساحة المخطط. |
| العرض | int | يمثل عرض الـtextbox، بوحدات 1/4000 من مساحة المخطط. |

**Returns:**
[TextBox](../../com.aspose.cells/textbox) - A TextBox object.
### addTextEffect(int effect, String text, String fontName, int size, boolean fontBold, boolean fontItalic, int topRow, int top, int leftColumn, int left, int height, int width) {#addTextEffect-int-java.lang.String-java.lang.String-int-boolean-boolean-int-int-int-int-int-int-}
```
public Shape addTextEffect(int effect, String text, String fontName, int size, boolean fontBold, boolean fontItalic, int topRow, int top, int leftColumn, int left, int height, int width)
```


يدرج كائن WordArt.

**Example**

```
         //add a WordArt
         Shape wordArt1 = shapes.addTextEffect(MsoPresetTextEffect.TEXT_EFFECT_10, "WordArt", "arial", 18, false, false, 3, 0, 3, 0, 200, 50);
```

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| effect | int | [MsoPresetTextEffect](../../com.aspose.cells/msopresettexteffect). نوع تأثير النص المسبق mso. |
| نص | java.lang.String | نص WordArt. |
| fontName | java.lang.String | اسم الخط. |
| الحجم | int | حجم الخط |
| fontBold | boolean | يشير إلى ما إذا كان الخط عريضًا. |
| fontItalic | boolean | يشير إلى ما إذا كان الخط مائلًا. |
| topRow | int | فهرس الصف العلوي الأيسر. |
| أعلى | int | يمثل الإزاحة العمودية للشكل من صفه الأيسر، بوحدة البكسل. |
| leftColumn | int | فهرس العمود العلوي الأيسر. |
| يسار | int | يمثل الإزاحة الأفقية للشكل من عموده الأيسر، بوحدة البكسل. |
| الارتفاع | int | يمثل ارتفاع الشكل، بوحدة البكسل. |
| العرض | int | يمثل عرض الشكل، بوحدة البكسل. |

**Returns:**
[Shape](../../com.aspose.cells/shape) - Returns a Shape object that represents the new WordArt object.
### addTextEffectInChart(int effect, String text, String fontName, int size, boolean fontBold, boolean fontItalic, int top, int left, int height, int width) {#addTextEffectInChart-int-java.lang.String-java.lang.String-int-boolean-boolean-int-int-int-int-}
```
public Shape addTextEffectInChart(int effect, String text, String fontName, int size, boolean fontBold, boolean fontItalic, int top, int left, int height, int width)
```


يدرج كائن WordArt إلى المخطط.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| effect | int | [MsoPresetTextEffect](../../com.aspose.cells/msopresettexteffect). نوع تأثير النص المسبق mso. |
| نص | java.lang.String | نص WordArt. |
| fontName | java.lang.String | اسم الخط. |
| الحجم | int | حجم الخط |
| fontBold | boolean | يشير إلى ما إذا كان الخط عريضًا. |
| fontItalic | boolean | يشير إلى ما إذا كان الخط مائلًا. |
| أعلى | int | يمثل الإزاحة العمودية للشكل من الزاوية العلوية اليسرى بوحدات 1/4000 من مساحة المخطط. |
| يسار | int | يمثل الإزاحة العمودية للشكل من الزاوية العلوية اليسرى بوحدات 1/4000 من مساحة المخطط. |
| الارتفاع | int | يمثل ارتفاع الشكل، بوحدات 1/4000 من مساحة المخطط. |
| العرض | int | يمثل عرض الشكل، بوحدات 1/4000 من مساحة المخطط. |

**Returns:**
[Shape](../../com.aspose.cells/shape) - Returns a Shape object that represents the new WordArt object.
### addWordArt(int style, String text, int topRow, int top, int leftColumn, int left, int height, int width) {#addWordArt-int-java.lang.String-int-int-int-int-int-int-}
```
public Shape addWordArt(int style, String text, int topRow, int top, int leftColumn, int left, int height, int width)
```


يضيف WordArt مسبق الإعداد منذ Excel 2007.

**Example**

```
         //add a WordArt
         Shape wordArt2 = shapes.addWordArt(PresetWordArtStyle.WORD_ART_STYLE_1, "WordArt", 3, 0, 3, 0, 50, 200);
```

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| style | int | [PresetWordArtStyle](../../com.aspose.cells/presetwordartstyle). نمط WordArt المسبق. |
| نص | java.lang.String | النص. |
| topRow | int | فهرس الصف العلوي الأيسر. |
| أعلى | int | يمثل الإزاحة العمودية للشكل من صفه الأيسر، بوحدة البكسل. |
| leftColumn | int | فهرس العمود العلوي الأيسر. |
| يسار | int | يمثل الإزاحة الأفقية للشكل من عموده الأيسر، بوحدة البكسل. |
| الارتفاع | int | يمثل ارتفاع الشكل، بوحدة البكسل. |
| العرض | int | يمثل عرض الشكل، بوحدة البكسل. |

**Returns:**
[Shape](../../com.aspose.cells/shape) - 
### clear() {#clear--}
```
public void clear()
```


امسح جميع الأشكال في ورقة العمل.

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


إرجاع ما إذا كان المثيل يحتوي على هذا الكائن

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| o | java.lang.Object | كائن اختبار |

**Returns:**
boolean - ما إذا كان المثيل يحتوي على هذا الكائن
### copyCommentsInRange(ShapeCollection shapes, CellArea ca, int destRow, int destColumn) {#copyCommentsInRange-com.aspose.cells.ShapeCollection-com.aspose.cells.CellArea-int-int-}
```
public void copyCommentsInRange(ShapeCollection shapes, CellArea ca, int destRow, int destColumn)
```


انسخ جميع التعليقات في النطاق.

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
| معامل | نوع | الوصف |
| --- | --- | --- |
| shapes | [ShapeCollection](../../com.aspose.cells/shapecollection) | الأشكال المصدر. |
| ca | [CellArea](../../com.aspose.cells/cellarea) | النطاق المصدر. |
| destRow | int | صف بداية النطاق الوجهة. |
| destColumn | int | عمود بداية النطاق الوجهة. |

### copyInRange(ShapeCollection sourceShapes, CellArea ca, int destRow, int destColumn, boolean isContained) {#copyInRange-com.aspose.cells.ShapeCollection-com.aspose.cells.CellArea-int-int-boolean-}
```
public void copyInRange(ShapeCollection sourceShapes, CellArea ca, int destRow, int destColumn, boolean isContained)
```


انسخ الأشكال في النطاق إلى النطاق الوجهة.

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
| معامل | نوع | الوصف |
| --- | --- | --- |
| sourceShapes | [ShapeCollection](../../com.aspose.cells/shapecollection) | الأشكال المصدر. |
| ca | [CellArea](../../com.aspose.cells/cellarea) | النطاق المصدر. |
| destRow | int | فهرس صف الوجهة للنطاق الوجهة. |
| destColumn | int | عمود الوجهة للنطاق الوجهة. |
| isContained | boolean | ما إذا كان سيتم نسخ الأشكال الموجودة فقط داخل النطاق. إذا كان صحيحًا، ينسخ فقط الأشكال داخل النطاق. وإلا، يعمل كما في MS Office. |

### deleteInRange(CellArea ca) {#deleteInRange-com.aspose.cells.CellArea-}
```
public void deleteInRange(CellArea ca)
```


احذف الأشكال في النطاق. لن يتم حذف أشكال التعليق.

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
| معامل | نوع | الوصف |
| --- | --- | --- |
| ca | [CellArea](../../com.aspose.cells/cellarea) | النطاق. إذا كانت الأشكال موجودة داخل النطاق، سيتم إزالتها. |

### deleteShape(Shape shape) {#deleteShape-com.aspose.cells.Shape-}
```
public void deleteShape(Shape shape)
```


احذف شكلاً. إذا كان الشكل داخل المجموعة أو كان شكلاً تعليقًا، لن يتم حذفه.

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
| معامل | نوع | الوصف |
| --- | --- | --- |
| shape | [Shape](../../com.aspose.cells/shape) |  |

### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| arg0 | java.lang.Object |  |

**Returns:**
boolean
### find(String what, int previous, FindOptions findOptions) {#find-java.lang.String-int-com.aspose.cells.FindOptions-}
```
public int find(String what, int previous, FindOptions findOptions)
```


ابحث عن شكل بالنص.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| ما | java.lang.String | النص للبحث عنه. |
| السابق | int | فهرس الشكل السابق الذي يحتوي على نفس النص. -1 إذا كان البحث من البداية. |
| findOptions | [FindOptions](../../com.aspose.cells/findoptions) | خيارات البحث |

**Returns:**
int - فهرس الشكل الموجود، -1 إذا لم يتم العثور على أي شكل.
### get(int index) {#get-int-}
```
public Shape get(int index)
```


يحصل على كائن [Shape](../../com.aspose.cells/shape) في الفهرس المحدد في القائمة.

**Example**

```
         //get the first shape
         Shape shape = shapes.get(0);
```

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| الفهرس | int | الفهرس. |

**Returns:**
[Shape](../../com.aspose.cells/shape) - 
### get(String name) {#get-java.lang.String-}
```
public Shape get(String name)
```


يحصل على كائن [Shape](../../com.aspose.cells/shape) حسب اسم الشكل.

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
| معامل | نوع | الوصف |
| --- | --- | --- |
| name | java.lang.String | اسم الشكل. |

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


يحصل على عدد العناصر الموجودة في مثيل CollectionBase.

**Returns:**
int - عدد العناصر الموجودة في مثيل CollectionBase.
### group(Shape[] groupItems) {#group-com.aspose.cells.Shape---}
```
public GroupShape group(Shape[] groupItems)
```


قم بتجميع الأشكال.

**Remarks**

يجب ألا يكون الشكل في groupItems مُجمَّعًا. يجب أن يكون الشكل في مجموعة Shapes هذه.

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
| معامل | نوع | الوصف |
| --- | --- | --- |
| groupItems | [Shape\[\]](../../com.aspose.cells/shape) | عناصر المجموعة. |

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


يحدد فهرس عنصر محدد في مثيل CollectionBase.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| o | java.lang.Object | يحدد فهرس عنصر محدد في مثيل CollectionBase. |

**Returns:**
int - فهرس القيمة إذا وجد في القائمة؛ وإلا -1.
### iterator() {#iterator--}
```
public Iterator iterator()
```


يرجع كائن تعداد يتنقل عبر مثيل CollectionBase.

**Returns:**
java.util.Iterator - كائن تكرار لمثيل CollectionBase.
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


أزل الشكل.

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
| معامل | نوع | الوصف |
| --- | --- | --- |
| shape | [Shape](../../com.aspose.cells/shape) |  |

### removeAt(int index) {#removeAt-int-}
```
public void removeAt(int index)
```


أزل الشكل.

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
| معامل | نوع | الوصف |
| --- | --- | --- |
| الفهرس | int | فهرس الشكل. |

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


افك تجميع عناصر الشكل.

**Remarks**

إذا كان الشكل الجماعي مُجمَّعًا بواسطة شكل جماعي آخر، لن يتم تنفيذ أي شيء.

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
| معامل | نوع | الوصف |
| --- | --- | --- |
| group | [GroupShape](../../com.aspose.cells/groupshape) | الشكل الجماعي. |

### updateSelectedValue() {#updateSelectedValue--}
```
public void updateSelectedValue()
```


حدّث القيمة المحددة بقيمة الخلية المرتبطة أو نطاق الشكل.

### wait() {#wait--}
```
public final void wait()
```




### wait(long arg0) {#wait-long-}
```
public final native void wait(long arg0)
```




**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

