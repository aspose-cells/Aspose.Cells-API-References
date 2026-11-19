---
title: "GridPicture"
second_title: "Aspose.Cells for Java API Reference"
description: "يحتوي على الكائن الذي يمثل صورة واحدة في جدول بيانات."
type: docs
url: /ar/java/com.aspose.gridweb/gridpicture/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
com.aspose.gridweb.IGridSave
```
public class GridPicture implements IGridSave
```

يحتوي على الكائن الذي يمثل صورة واحدة في جدول بيانات.
## الطرق

| طريقة | الوصف |
| --- | --- |
| [addHyperlink(String address)](#addHyperlink-java.lang.String-) | يضيف ارتباطًا تشعبيًا إلى الشكل. |
| [alignTopRightCorner(int topRow, int rightColumn)](#alignTopRightCorner-int-int-) | ينقل الصورة إلى الزاوية العليا اليمنى. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAlternativeText()](#getAlternativeText--) | إرجاع أو تعيين سلسلة النص الوصفية (البديلة) لكائن [GridShape](../../com.aspose.gridweb/gridshape). |
| [getBorderLineColor()](#getBorderLineColor--) | يمثل [Color](../../com.aspose.cells/color) لخط حدود الصورة. |
| [getBorderWeight()](#getBorderWeight--) | يحصل على وزن خط حدود الصورة بوحدات pt. |
| [getBottom()](#getBottom--) | يمثل عرض الإزاحة العمودية للشكل من صف زاوية أسفله السفلية، بوحدة البكسل. |
| [getClass()](#getClass--) |  |
| [getData()](#getData--) | يحصل على بيانات الصورة. |
| [getHeight()](#getHeight--) | يمثل ارتفاع الشكل، بوحدة البكسل. |
| [getHeightCM()](#getHeightCM--) | يمثل ارتفاع الشكل، بوحدة البوصة. |
| [getHeightInch()](#getHeightInch--) | يمثل ارتفاع الشكل، بوحدة البوصة. |
| [getHeightPt()](#getHeightPt--) | يمثل ارتفاع الشكل، بوحدة النقاط. |
| [getHeightScale()](#getHeightScale--) | يحصل على مقياس الارتفاع، بوحدة النسبة المئوية من ارتفاع الصورة الأصلي. |
| [getHtmlText()](#getHtmlText--) | يحصل على سلسلة HTML التي تحتوي على البيانات وبعض التنسيقات في هذا textbox. |
| [getHyperlink()](#getHyperlink--) | يحصل على الارتباط التشعبي للشكل. |
| [getID()](#getID--) | يحصل على / يعيّن معرف الصورة. |
| [getImageFormat()](#getImageFormat--) | يحصل على تنسيق الصورة. |
| [getLeft()](#getLeft--) | يمثل الإزاحة الأفقية للشكل من عموده الأيسر، بوحدة البكسل. |
| [getLeftCM()](#getLeftCM--) | يمثل الإزاحة الأفقية للشكل من عموده الأيسر، بوحدة السنتيمتر. |
| [getLeftInch()](#getLeftInch--) | يمثل الإزاحة الأفقية للشكل من عموده الأيسر، بوحدة البوصة. |
| [getLeftToCorner()](#getLeftToCorner--) | يمثل الإزاحة الأفقية للشكل من الحافة اليسرى لورقة العمل، بوحدة البكسل. |
| [getLinkedCell()](#getLinkedCell--) | يحصل على نطاق ورقة العمل المرتبط بقيمة التحكم. |
| [getLowerDeltaX()](#getLowerDeltaX--) | يحصل على الإزاحة الأفقية للشكل من عمود زاويةه السفلية اليمنى. |
| [getLowerDeltaY()](#getLowerDeltaY--) | يحصل على الإزاحة العمودية للشكل من صف زاويةه السفلية اليمنى. |
| [getLowerRightColumn()](#getLowerRightColumn--) | يمثل فهرس عمود الزاوية السفلية اليمنى. |
| [getLowerRightRow()](#getLowerRightRow--) | يمثل فهرس صف الزاوية السفلية اليمنى. |
| [getName()](#getName--) | يحصل على اسم الشكل. |
| [getOriginalHeight()](#getOriginalHeight--) | يحصل على الارتفاع الأصلي للصورة. |
| [getOriginalHeightCM()](#getOriginalHeightCM--) | يحصل على الارتفاع الأصلي للصورة، بوحدة السنتيمتر. |
| [getOriginalHeightInch()](#getOriginalHeightInch--) | يحصل على الارتفاع الأصلي للصورة، بوحدة البوصة. |
| [getOriginalWidth()](#getOriginalWidth--) | يحصل على العرض الأصلي للصورة. |
| [getOriginalWidthCM()](#getOriginalWidthCM--) | يحصل على العرض الأصلي للصورة، بوحدة السنتيمتر. |
| [getOriginalWidthInch()](#getOriginalWidthInch--) | يحصل على العرض الأصلي للصورة، بوحدة البوصة. |
| [getRelativeToOriginalPictureSize()](#getRelativeToOriginalPictureSize--) | يشير إلى ما إذا كان الشكل نسبيًا لحجم الصورة الأصلي. |
| [getRight()](#getRight--) | يمثل عرض الإزاحة الأفقية للشكل من عمود زاويةه السفلية اليمنى، بوحدة البكسل. |
| [getRotationAngle()](#getRotationAngle--) | يحصل على دوران الشكل. |
| [getSourceFullName()](#getSourceFullName--) | يحصل على المسار واسم ملف المصدر للصورة المرتبطة. |
| [getText()](#getText--) | يمثل السلسلة في كائن TextBox هذا. |
| [getTitle()](#getTitle--) | يحدد العنوان (التسمية) لكائن الشكل الحالي. |
| [getTop()](#getTop--) | يمثل الإزاحة العمودية للشكل من صفه العلوي، بوحدة البكسل. |
| [getTopCM()](#getTopCM--) | يمثل الإزاحة العمودية للشكل من صفه العلوي، بوحدة السنتيمتر. |
| [getTopInch()](#getTopInch--) | يمثل الإزاحة العمودية للشكل من صفه العلوي، بوحدة البوصة. |
| [getTopToCorner()](#getTopToCorner--) | يمثل الإزاحة العمودية للشكل من الحافة العلوية لورقة العمل، بوحدة البكسل. |
| [getUpperDeltaX()](#getUpperDeltaX--) | يحصل على الإزاحة الأفقية للشكل من عمود الزاوية العلوية اليسرى. |
| [getUpperDeltaY()](#getUpperDeltaY--) | يحصل على الإزاحة العمودية للشكل من صف الزاوية العلوية اليسرى. |
| [getUpperLeftColumn()](#getUpperLeftColumn--) | يمثل فهرس عمود الزاوية العلوية اليسرى. |
| [getUpperLeftRow()](#getUpperLeftRow--) | يمثل فهرس الصف للزاوية العلوية اليسرى. |
| [getWidth()](#getWidth--) | يمثل عرض الشكل، بوحدة البكسل. |
| [getWidthCM()](#getWidthCM--) | يمثل عرض الشكل، بوحدة السنتيمتر. |
| [getWidthInch()](#getWidthInch--) | يمثل عرض الشكل، بوحدة البوصة. |
| [getWidthPt()](#getWidthPt--) | يمثل عرض الشكل، بوحدة النقطة. |
| [getWidthScale()](#getWidthScale--) | يحصل على مقياس العرض، بوحدة النسبة المئوية من عرض الصورة الأصلي. |
| [getX()](#getX--) | يحصل على الإزاحة الأفقية للشكل من الحافة اليسرى لورقة العمل، بوحدة البكسل. |
| [getY()](#getY--) | يحصل على الإزاحة العمودية للشكل من الحد العلوي للورقة، بوحدة البكسل. |
| [getZOrderPosition()](#getZOrderPosition--) | يعيد موضع الشكل في ترتيب z. |
| [hasLine()](#hasLine--) | يحصل على ما إذا كان حد الخط للشكل مرئيًا. |
| [hashCode()](#hashCode--) |  |
| [isFlippedVertically()](#isFlippedVertically--) | يحصل على ما إذا كان الشكل مقلوبًا عموديًا. |
| [isGroup()](#isGroup--) | يشير إلى ما إذا كان الشكل مجموعة. |
| [isHidden()](#isHidden--) | يشير إلى ما إذا كان الكائن مرئيًا. |
| [isLockAspectRatio()](#isLockAspectRatio--) | True يعني عدم السماح بتغيّر نسبة العرض إلى الارتفاع. |
| [isLocked()](#isLocked--) | True إذا كان الكائن مقفلاً، False إذا كان يمكن تعديل الكائن عندما تكون الورقة محمية. |
| [isTextWrapped()](#isTextWrapped--) | يحصل على نوع التفاف النص للشكل الذي يحتوي على نص. |
| [move(int upperLeftRow, int upperLeftColumn)](#move-int-int-) | ينقل الصورة إلى موقع محدد. |
| [moveToRange(int upperLeftRow, int upperLeftColumn, int lowerRightRow, int lowerRightColumn)](#moveToRange-int-int-int-int-) | ينقل الشكل إلى نطاق محدد. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [removeHyperlink()](#removeHyperlink--) | إزالة الارتباط التشعبي للشكل. |
| [saveToImage(InputStream s)](#saveToImage-java.io.InputStream-) | ينشئ الصورة ويحفظها إلى تدفق. |
| [setAlternativeText(String value)](#setAlternativeText-java.lang.String-) | إرجاع أو تعيين سلسلة النص الوصفية (البديلة) لكائن [GridShape](../../com.aspose.gridweb/gridshape). |
| [setBorderLineColor(Color value)](#setBorderLineColor-com.aspose.gridweb.Color-) | يمثل [Color](../../com.aspose.cells/color) لخط حدود الصورة. |
| [setBorderWeight(double value)](#setBorderWeight-double-) | يضبط وزن خط الحدود للصورة بوحدات النقاط (pt). |
| [setBottom(int value)](#setBottom-int-) | يمثل عرض الإزاحة العمودية للشكل من صف زاوية أسفله السفلية، بوحدة البكسل. |
| [setData(byte[] value)](#setData-byte---) | يحصل على بيانات الصورة. |
| [setFlippedVertically(boolean value)](#setFlippedVertically-boolean-) | يضبط ما إذا كان الشكل مقلوبًا عموديًا. |
| [setHasLine(boolean value)](#setHasLine-boolean-) | يضبط ظهور حد الخط للشكل. |
| [setHeight(int value)](#setHeight-int-) | يمثل ارتفاع الشكل، بوحدة البكسل. |
| [setHeightCM(double value)](#setHeightCM-double-) | يمثل ارتفاع الشكل، بوحدة البوصة. |
| [setHeightInch(double value)](#setHeightInch-double-) | يمثل ارتفاع الشكل، بوحدة البوصة. |
| [setHeightPt(double value)](#setHeightPt-double-) | يمثل ارتفاع الشكل، بوحدة النقاط. |
| [setHeightScale(int value)](#setHeightScale-int-) | يضبط مقياس الارتفاع، بوحدة النسبة المئوية لارتفاع الصورة الأصلية. |
| [setHidden(boolean value)](#setHidden-boolean-) | يشير إلى ما إذا كان الكائن مرئيًا. |
| [setHtmlText(String value)](#setHtmlText-java.lang.String-) | يضبط سلسلة HTML التي تحتوي على البيانات وبعض التنسيقات في هذا مربع النص. |
| [setID(String value)](#setID-java.lang.String-) | يحصل على / يعيّن معرف الصورة. |
| [setLeft(int value)](#setLeft-int-) | يمثل الإزاحة الأفقية للشكل من عموده الأيسر، بوحدة البكسل. |
| [setLeftCM(double value)](#setLeftCM-double-) | يمثل الإزاحة الأفقية للشكل من عموده الأيسر، بوحدة السنتيمتر. |
| [setLeftInch(double value)](#setLeftInch-double-) | يمثل الإزاحة الأفقية للشكل من عموده الأيسر، بوحدة البوصة. |
| [setLeftToCorner(int value)](#setLeftToCorner-int-) | يمثل الإزاحة الأفقية للشكل من الحافة اليسرى لورقة العمل، بوحدة البكسل. |
| [setLinkedCell(String value)](#setLinkedCell-java.lang.String-) | يضبط نطاق ورقة العمل المرتبط بقيمة عنصر التحكم. |
| [setLockAspectRatio(boolean value)](#setLockAspectRatio-boolean-) | True يعني عدم السماح بتغيّر نسبة العرض إلى الارتفاع. |
| [setLocked(boolean value)](#setLocked-boolean-) | True إذا كان الكائن مقفلاً، False إذا كان يمكن تعديل الكائن عندما تكون الورقة محمية. |
| [setLowerDeltaX(int value)](#setLowerDeltaX-int-) | يضبط الإزاحة الأفقية للشكل من عمود زاويته السفلية اليمنى. |
| [setLowerDeltaY(int value)](#setLowerDeltaY-int-) | يضبط الإزاحة العمودية للشكل من صف زاويته السفلية اليمنى. |
| [setLowerRightColumn(int value)](#setLowerRightColumn-int-) | يمثل فهرس عمود الزاوية السفلية اليمنى. |
| [setLowerRightRow(int value)](#setLowerRightRow-int-) | يمثل فهرس صف الزاوية السفلية اليمنى. |
| [setName(String value)](#setName-java.lang.String-) | يضبط اسم الشكل. |
| [setRelativeToOriginalPictureSize(boolean value)](#setRelativeToOriginalPictureSize-boolean-) | يشير إلى ما إذا كان الشكل نسبيًا لحجم الصورة الأصلي. |
| [setRight(int value)](#setRight-int-) | يمثل عرض الإزاحة الأفقية للشكل من عمود زاويةه السفلية اليمنى، بوحدة البكسل. |
| [setRotationAngle(double value)](#setRotationAngle-double-) | يضبط دوران الشكل. |
| [setSourceFullName(String value)](#setSourceFullName-java.lang.String-) | يضبط المسار واسم ملف المصدر للصورة المرتبطة. |
| [setText(String value)](#setText-java.lang.String-) | يمثل السلسلة في كائن TextBox هذا. |
| [setTextWrapped(boolean value)](#setTextWrapped-boolean-) | يضبط نوع التفاف النص للشكل الذي يحتوي على نص. |
| [setTitle(String value)](#setTitle-java.lang.String-) | يحدد العنوان (التسمية) لكائن الشكل الحالي. |
| [setTop(int value)](#setTop-int-) | يمثل الإزاحة العمودية للشكل من صفه العلوي، بوحدة البكسل. |
| [setTopCM(double value)](#setTopCM-double-) | يمثل الإزاحة العمودية للشكل من صفه العلوي، بوحدة السنتيمتر. |
| [setTopInch(double value)](#setTopInch-double-) | يمثل الإزاحة العمودية للشكل من صفه العلوي، بوحدة البوصة. |
| [setTopToCorner(int value)](#setTopToCorner-int-) | يمثل الإزاحة العمودية للشكل من الحافة العلوية لورقة العمل، بوحدة البكسل. |
| [setUpperDeltaX(int value)](#setUpperDeltaX-int-) | يضبط الإزاحة الأفقية للشكل من عمود زاويته العلوية اليسرى. |
| [setUpperDeltaY(int value)](#setUpperDeltaY-int-) | يضبط الإزاحة العمودية للشكل من صف زاويته العلوية اليسرى. |
| [setUpperLeftColumn(int value)](#setUpperLeftColumn-int-) | يمثل فهرس عمود الزاوية العلوية اليسرى. |
| [setUpperLeftRow(int value)](#setUpperLeftRow-int-) | يمثل فهرس الصف للزاوية العلوية اليسرى. |
| [setWidth(int value)](#setWidth-int-) | يمثل عرض الشكل، بوحدة البكسل. |
| [setWidthCM(double value)](#setWidthCM-double-) | يمثل عرض الشكل، بوحدة السنتيمتر. |
| [setWidthInch(double value)](#setWidthInch-double-) | يمثل عرض الشكل، بوحدة البوصة. |
| [setWidthPt(double value)](#setWidthPt-double-) | يمثل عرض الشكل، بوحدة النقطة. |
| [setWidthScale(int value)](#setWidthScale-int-) | يضبط مقياس العرض، بوحدة النسبة المئوية لعرض الصورة الأصلي. |
| [setX(int value)](#setX-int-) | يضبط الإزاحة الأفقية للشكل من الحد الأيسر للورقة، بوحدة البكسل. |
| [setY(int value)](#setY-int-) | يضبط الإزاحة العمودية للشكل من الحد العلوي لورقة العمل، بوحدة البكسل. |
| [setZOrderPosition(int value)](#setZOrderPosition-int-) | يعيد موضع الشكل في ترتيب z. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### addHyperlink(String address) {#addHyperlink-java.lang.String-}
```
public GridHyperlink addHyperlink(String address)
```


يضيف ارتباطًا تشعبيًا إلى الشكل.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| العنوان | java.lang.String | عنوان الارتباط التشعبي. |

**Returns:**
[GridHyperlink](../../com.aspose.gridweb/gridhyperlink) - Return the new hyperlink object.
### alignTopRightCorner(int topRow, int rightColumn) {#alignTopRightCorner-int-int-}
```
public void alignTopRightCorner(int topRow, int rightColumn)
```


ينقل الصورة إلى الزاوية العليا اليمنى.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| topRow | int | فهرس الصف. |
| rightColumn | int | فهرس العمود. |

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
### getAlternativeText() {#getAlternativeText--}
```
public String getAlternativeText()
```


إرجاع أو تعيين سلسلة النص الوصفية (البديلة) لكائن [GridShape](../../com.aspose.gridweb/gridshape).

**Returns:**
java.lang.String
### getBorderLineColor() {#getBorderLineColor--}
```
public Color getBorderLineColor()
```


يمثل [Color](../../com.aspose.cells/color) لخط حدود الصورة.

**Returns:**
[Color](../../com.aspose.gridweb/color)
### getBorderWeight() {#getBorderWeight--}
```
public double getBorderWeight()
```


يحصل على وزن خط حدود الصورة بوحدات pt.

**Returns:**
double
### getBottom() {#getBottom--}
```
public int getBottom()
```


يمثل عرض الإزاحة العمودية للشكل من صف زاوية أسفله السفلية، بوحدة البكسل.

**Returns:**
int
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getData() {#getData--}
```
public byte[] getData()
```


يحصل على بيانات الصورة.

**Returns:**
byte[]
### getHeight() {#getHeight--}
```
public int getHeight()
```


يمثل ارتفاع الشكل، بوحدة البكسل.

**Returns:**
int
### getHeightCM() {#getHeightCM--}
```
public double getHeightCM()
```


يمثل ارتفاع الشكل، بوحدة البوصة.

**Returns:**
double
### getHeightInch() {#getHeightInch--}
```
public double getHeightInch()
```


يمثل ارتفاع الشكل، بوحدة البوصة.

**Returns:**
double
### getHeightPt() {#getHeightPt--}
```
public double getHeightPt()
```


يمثل ارتفاع الشكل، بوحدة النقاط.

**Returns:**
double
### getHeightScale() {#getHeightScale--}
```
public int getHeightScale()
```


يحصل على مقياس الارتفاع، بوحدة النسبة المئوية لارتفاع الصورة الأصلي. إذا لم يكن الشكل صورة، فإن خاصية HeightScale تُعيد فقط 100؛

**Returns:**
int
### getHtmlText() {#getHtmlText--}
```
public String getHtmlText()
```


يحصل على سلسلة HTML التي تحتوي على البيانات وبعض التنسيقات في هذا textbox.

**Returns:**
java.lang.String
### getHyperlink() {#getHyperlink--}
```
public GridHyperlink getHyperlink()
```


يحصل على الارتباط التشعبي للشكل.

**Returns:**
[GridHyperlink](../../com.aspose.gridweb/gridhyperlink)
### getID() {#getID--}
```
public String getID()
```


يحصل على / يعيّن معرف الصورة.

**Returns:**
java.lang.String
### getImageFormat() {#getImageFormat--}
```
public int getImageFormat()
```


يحصل على تنسيق الصورة.

انظر [GridImageType](../../com.aspose.gridweb/gridimagetype).

**Returns:**
int
### getLeft() {#getLeft--}
```
public int getLeft()
```


يمثل الإزاحة الأفقية للشكل من عموده الأيسر، بوحدة البكسل.

**Returns:**
int
### getLeftCM() {#getLeftCM--}
```
public double getLeftCM()
```


يمثل الإزاحة الأفقية للشكل من عموده الأيسر، بوحدة السنتيمتر.

**Returns:**
double
### getLeftInch() {#getLeftInch--}
```
public double getLeftInch()
```


يمثل الإزاحة الأفقية للشكل من عموده الأيسر، بوحدة البوصة.

**Returns:**
double
### getLeftToCorner() {#getLeftToCorner--}
```
public int getLeftToCorner()
```


يمثل الإزاحة الأفقية للشكل من الحافة اليسرى لورقة العمل، بوحدة البكسل.

**Returns:**
int
### getLinkedCell() {#getLinkedCell--}
```
public String getLinkedCell()
```


يحصل على نطاق ورقة العمل المرتبط بقيمة التحكم.

**Returns:**
java.lang.String
### getLowerDeltaX() {#getLowerDeltaX--}
```
public int getLowerDeltaX()
```


يحصل على الإزاحة الأفقية للشكل من عمود زاويةه السفلية اليمنى. النطاق القيمي هو من 0 إلى 1024.

**Returns:**
int
### getLowerDeltaY() {#getLowerDeltaY--}
```
public int getLowerDeltaY()
```


يحصل على الإزاحة العمودية للشكل من صف زاويةه السفلية اليمنى. النطاق القيمي هو من 0 إلى 256.

**Returns:**
int
### getLowerRightColumn() {#getLowerRightColumn--}
```
public int getLowerRightColumn()
```


يمثل فهرس عمود الزاوية السفلية اليمنى.

**Returns:**
int
### getLowerRightRow() {#getLowerRightRow--}
```
public int getLowerRightRow()
```


يمثل فهرس صف الزاوية السفلية اليمنى.

**Returns:**
int
### getName() {#getName--}
```
public String getName()
```


يحصل على اسم الشكل.

**Returns:**
java.lang.String
### getOriginalHeight() {#getOriginalHeight--}
```
public int getOriginalHeight()
```


يحصل على الارتفاع الأصلي للصورة.

**Returns:**
int
### getOriginalHeightCM() {#getOriginalHeightCM--}
```
public double getOriginalHeightCM()
```


يحصل على الارتفاع الأصلي للصورة، بوحدة السنتيمتر.

**Returns:**
double
### getOriginalHeightInch() {#getOriginalHeightInch--}
```
public double getOriginalHeightInch()
```


يحصل على الارتفاع الأصلي للصورة، بوحدة البوصة.

**Returns:**
double
### getOriginalWidth() {#getOriginalWidth--}
```
public int getOriginalWidth()
```


يحصل على العرض الأصلي للصورة.

**Returns:**
int
### getOriginalWidthCM() {#getOriginalWidthCM--}
```
public double getOriginalWidthCM()
```


يحصل على العرض الأصلي للصورة، بوحدة السنتيمتر.

**Returns:**
double
### getOriginalWidthInch() {#getOriginalWidthInch--}
```
public double getOriginalWidthInch()
```


يحصل على العرض الأصلي للصورة، بوحدة البوصة.

**Returns:**
double
### getRelativeToOriginalPictureSize() {#getRelativeToOriginalPictureSize--}
```
public boolean getRelativeToOriginalPictureSize()
```


يشير إلى ما إذا كان الشكل نسبيًا لحجم الصورة الأصلي.

**Returns:**
boolean
### getRight() {#getRight--}
```
public int getRight()
```


يمثل عرض الإزاحة الأفقية للشكل من عمود زاويةه السفلية اليمنى، بوحدة البكسل.

**Returns:**
int
### getRotationAngle() {#getRotationAngle--}
```
public double getRotationAngle()
```


يحصل على دوران الشكل.

**Returns:**
double
### getSourceFullName() {#getSourceFullName--}
```
public String getSourceFullName()
```


يحصل على المسار واسم ملف المصدر للصورة المرتبطة.

**Remarks**

القيمة الافتراضية هي سلسلة فارغة. إذا لم يكن SourceFullName سلسلة فارغة، فإن الصورة تكون مرتبطة. إذا لم يكن SourceFullName سلسلة فارغة، ولكن Data يساوي null، فإن الصورة تكون مرتبطة ولا تُخزن في الملف.

**Returns:**
java.lang.String
### getText() {#getText--}
```
public String getText()
```


يمثل السلسلة في كائن TextBox هذا.

**Returns:**
java.lang.String
### getTitle() {#getTitle--}
```
public String getTitle()
```


يحدد العنوان (التسمية) لكائن الشكل الحالي.

**Returns:**
java.lang.String
### getTop() {#getTop--}
```
public int getTop()
```


يمثل الإزاحة العمودية للشكل من صفه العلوي، بوحدة البكسل.

**Remarks**

إذا كان الشكل داخل المخطط، يمثل الإزاحة العمودية للشكل من حدّه العلوي.

**Returns:**
int
### getTopCM() {#getTopCM--}
```
public double getTopCM()
```


يمثل الإزاحة العمودية للشكل من صفه العلوي، بوحدة السنتيمتر.

**Returns:**
double
### getTopInch() {#getTopInch--}
```
public double getTopInch()
```


يمثل الإزاحة العمودية للشكل من صفه العلوي، بوحدة البوصة.

**Returns:**
double
### getTopToCorner() {#getTopToCorner--}
```
public int getTopToCorner()
```


يمثل الإزاحة العمودية للشكل من الحافة العلوية لورقة العمل، بوحدة البكسل.

**Returns:**
int
### getUpperDeltaX() {#getUpperDeltaX--}
```
public int getUpperDeltaX()
```


يحصل على الإزاحة الأفقية للشكل من عمود زاويةه العلوية اليسرى. النطاق القيمي هو من 0 إلى 1024.

**Returns:**
int
### getUpperDeltaY() {#getUpperDeltaY--}
```
public int getUpperDeltaY()
```


يحصل على الإزاحة العمودية للشكل من صف زاويةه العلوية اليسرى. النطاق القيمي هو من 0 إلى 256.

**Returns:**
int
### getUpperLeftColumn() {#getUpperLeftColumn--}
```
public int getUpperLeftColumn()
```


يمثل فهرس عمود الزاوية العلوية اليسرى.

**Returns:**
int
### getUpperLeftRow() {#getUpperLeftRow--}
```
public int getUpperLeftRow()
```


يمثل فهرس الصف للزاوية العلوية اليسرى.

**Remarks**

إذا كان الشكل داخل شكل آخر أو داخل مجموعة، سيتم تجاهل UpperLeftRow.

**Returns:**
int
### getWidth() {#getWidth--}
```
public int getWidth()
```


يمثل عرض الشكل، بوحدة البكسل.

**Returns:**
int
### getWidthCM() {#getWidthCM--}
```
public double getWidthCM()
```


يمثل عرض الشكل، بوحدة السنتيمتر.

**Returns:**
double
### getWidthInch() {#getWidthInch--}
```
public double getWidthInch()
```


يمثل عرض الشكل، بوحدة البوصة.

**Returns:**
double
### getWidthPt() {#getWidthPt--}
```
public double getWidthPt()
```


يمثل عرض الشكل، بوحدة النقطة.

**Returns:**
double
### getWidthScale() {#getWidthScale--}
```
public int getWidthScale()
```


يحصل على مقياس العرض، بوحدة النسبة المئوية لعرض الصورة الأصلي. إذا لم يكن الشكل صورة، فإن خاصية WidthScale تُعيد فقط 100؛

**Returns:**
int
### getX() {#getX--}
```
public int getX()
```


يحصل على الإزاحة الأفقية للشكل من الحافة اليسرى لورقة العمل، بوحدة البكسل.

**Returns:**
int
### getY() {#getY--}
```
public int getY()
```


يحصل على الإزاحة العمودية للشكل من الحد العلوي للورقة، بوحدة البكسل.

**Returns:**
int
### getZOrderPosition() {#getZOrderPosition--}
```
public int getZOrderPosition()
```


يعيد موضع الشكل في ترتيب z.

**Returns:**
int
### hasLine() {#hasLine--}
```
public boolean hasLine()
```


يحصل على ما إذا كان حد الخط للشكل مرئيًا.

**Returns:**
boolean
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isFlippedVertically() {#isFlippedVertically--}
```
public boolean isFlippedVertically()
```


يحصل على ما إذا كان الشكل مقلوبًا عموديًا.

**Returns:**
boolean
### isGroup() {#isGroup--}
```
public boolean isGroup()
```


يشير إلى ما إذا كان الشكل مجموعة.

**Returns:**
boolean
### isHidden() {#isHidden--}
```
public boolean isHidden()
```


يشير إلى ما إذا كان الكائن مرئيًا.

**Returns:**
boolean
### isLockAspectRatio() {#isLockAspectRatio--}
```
public boolean isLockAspectRatio()
```


True يعني عدم السماح بتغيّر نسبة العرض إلى الارتفاع.

**Returns:**
boolean
### isLocked() {#isLocked--}
```
public boolean isLocked()
```


True إذا كان الكائن مقفلاً، False إذا كان يمكن تعديل الكائن عندما تكون الورقة محمية.

**Returns:**
boolean
### isTextWrapped() {#isTextWrapped--}
```
public boolean isTextWrapped()
```


يحصل على نوع التفاف النص للشكل الذي يحتوي على نص.

**Returns:**
boolean
### move(int upperLeftRow, int upperLeftColumn) {#move-int-int-}
```
public void move(int upperLeftRow, int upperLeftColumn)
```


ينقل الصورة إلى موقع محدد.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| upperLeftRow | int | فهرس الصف العلوي الأيسر. |
| upperLeftColumn | int | فهرس العمود العلوي الأيسر. |

### moveToRange(int upperLeftRow, int upperLeftColumn, int lowerRightRow, int lowerRightColumn) {#moveToRange-int-int-int-int-}
```
public void moveToRange(int upperLeftRow, int upperLeftColumn, int lowerRightRow, int lowerRightColumn)
```


ينقل الشكل إلى نطاق محدد.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| upperLeftRow | int | فهرس الصف العلوي الأيسر. |
| upperLeftColumn | int | فهرس العمود العلوي الأيسر. |
| lowerRightRow | int | فهرس الصف السفلي الأيمن. |
| lowerRightColumn | int | فهرس العمود السفلي الأيمن. |

### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### removeHyperlink() {#removeHyperlink--}
```
public void removeHyperlink()
```


إزالة الارتباط التشعبي للشكل.

### saveToImage(InputStream s) {#saveToImage-java.io.InputStream-}
```
public void saveToImage(InputStream s)
```


ينشئ الصورة ويحفظها إلى تدفق.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| s | java.io.InputStream |  |

### setAlternativeText(String value) {#setAlternativeText-java.lang.String-}
```
public void setAlternativeText(String value)
```


إرجاع أو تعيين سلسلة النص الوصفية (البديلة) لكائن [GridShape](../../com.aspose.gridweb/gridshape).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

### setBorderLineColor(Color value) {#setBorderLineColor-com.aspose.gridweb.Color-}
```
public void setBorderLineColor(Color value)
```


يمثل [Color](../../com.aspose.cells/color) لخط حدود الصورة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | [Color](../../com.aspose.gridweb/color) |  |

### setBorderWeight(double value) {#setBorderWeight-double-}
```
public void setBorderWeight(double value)
```


يضبط وزن خط الحدود للصورة بوحدات النقاط (pt).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | double |  |

### setBottom(int value) {#setBottom-int-}
```
public void setBottom(int value)
```


يمثل عرض الإزاحة العمودية للشكل من صف زاوية أسفله السفلية، بوحدة البكسل.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setData(byte[] value) {#setData-byte---}
```
public void setData(byte[] value)
```


يحصل على بيانات الصورة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | byte[] |  |

### setFlippedVertically(boolean value) {#setFlippedVertically-boolean-}
```
public void setFlippedVertically(boolean value)
```


يضبط ما إذا كان الشكل مقلوبًا عموديًا.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setHasLine(boolean value) {#setHasLine-boolean-}
```
public void setHasLine(boolean value)
```


يضبط ظهور حد الخط للشكل.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setHeight(int value) {#setHeight-int-}
```
public void setHeight(int value)
```


يمثل ارتفاع الشكل، بوحدة البكسل.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setHeightCM(double value) {#setHeightCM-double-}
```
public void setHeightCM(double value)
```


يمثل ارتفاع الشكل، بوحدة البوصة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | double |  |

### setHeightInch(double value) {#setHeightInch-double-}
```
public void setHeightInch(double value)
```


يمثل ارتفاع الشكل، بوحدة البوصة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | double |  |

### setHeightPt(double value) {#setHeightPt-double-}
```
public void setHeightPt(double value)
```


يمثل ارتفاع الشكل، بوحدة النقاط.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | double |  |

### setHeightScale(int value) {#setHeightScale-int-}
```
public void setHeightScale(int value)
```


يضبط مقياس الارتفاع، بوحدة النسبة المئوية من ارتفاع الصورة الأصلية. إذا لم يكن الشكل صورة، فإن الخاصية HeightScale تُعيد 100 فقط؛

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setHidden(boolean value) {#setHidden-boolean-}
```
public void setHidden(boolean value)
```


يشير إلى ما إذا كان الكائن مرئيًا.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setHtmlText(String value) {#setHtmlText-java.lang.String-}
```
public void setHtmlText(String value)
```


يضبط سلسلة HTML التي تحتوي على البيانات وبعض التنسيقات في هذا مربع النص.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

### setID(String value) {#setID-java.lang.String-}
```
public void setID(String value)
```


يحصل على / يعيّن معرف الصورة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

### setLeft(int value) {#setLeft-int-}
```
public void setLeft(int value)
```


يمثل الإزاحة الأفقية للشكل من عموده الأيسر، بوحدة البكسل.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setLeftCM(double value) {#setLeftCM-double-}
```
public void setLeftCM(double value)
```


يمثل الإزاحة الأفقية للشكل من عموده الأيسر، بوحدة السنتيمتر.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | double |  |

### setLeftInch(double value) {#setLeftInch-double-}
```
public void setLeftInch(double value)
```


يمثل الإزاحة الأفقية للشكل من عموده الأيسر، بوحدة البوصة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | double |  |

### setLeftToCorner(int value) {#setLeftToCorner-int-}
```
public void setLeftToCorner(int value)
```


يمثل الإزاحة الأفقية للشكل من الحافة اليسرى لورقة العمل، بوحدة البكسل.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setLinkedCell(String value) {#setLinkedCell-java.lang.String-}
```
public void setLinkedCell(String value)
```


يضبط نطاق ورقة العمل المرتبط بقيمة عنصر التحكم.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

### setLockAspectRatio(boolean value) {#setLockAspectRatio-boolean-}
```
public void setLockAspectRatio(boolean value)
```


True يعني عدم السماح بتغيّر نسبة العرض إلى الارتفاع.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setLocked(boolean value) {#setLocked-boolean-}
```
public void setLocked(boolean value)
```


True إذا كان الكائن مقفلاً، False إذا كان يمكن تعديل الكائن عندما تكون الورقة محمية.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setLowerDeltaX(int value) {#setLowerDeltaX-int-}
```
public void setLowerDeltaX(int value)
```


يضبط الإزاحة الأفقية للشكل من عمود زاويةه السفلية اليمنى. النطاق القيمي هو من 0 إلى 1024.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setLowerDeltaY(int value) {#setLowerDeltaY-int-}
```
public void setLowerDeltaY(int value)
```


يضبط الإزاحة العمودية للشكل من صف زاويةه السفلية اليمنى. النطاق القيمي هو من 0 إلى 256.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setLowerRightColumn(int value) {#setLowerRightColumn-int-}
```
public void setLowerRightColumn(int value)
```


يمثل فهرس عمود الزاوية السفلية اليمنى.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setLowerRightRow(int value) {#setLowerRightRow-int-}
```
public void setLowerRightRow(int value)
```


يمثل فهرس صف الزاوية السفلية اليمنى.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setName(String value) {#setName-java.lang.String-}
```
public void setName(String value)
```


يضبط اسم الشكل.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

### setRelativeToOriginalPictureSize(boolean value) {#setRelativeToOriginalPictureSize-boolean-}
```
public void setRelativeToOriginalPictureSize(boolean value)
```


يشير إلى ما إذا كان الشكل نسبيًا لحجم الصورة الأصلي.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setRight(int value) {#setRight-int-}
```
public void setRight(int value)
```


يمثل عرض الإزاحة الأفقية للشكل من عمود زاويةه السفلية اليمنى، بوحدة البكسل.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setRotationAngle(double value) {#setRotationAngle-double-}
```
public void setRotationAngle(double value)
```


يضبط دوران الشكل.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | double |  |

### setSourceFullName(String value) {#setSourceFullName-java.lang.String-}
```
public void setSourceFullName(String value)
```


يضبط المسار واسم ملف المصدر للصورة المرتبطة.

**Remarks**

القيمة الافتراضية هي سلسلة فارغة. إذا لم يكن SourceFullName سلسلة فارغة، فإن الصورة تكون مرتبطة. إذا لم يكن SourceFullName سلسلة فارغة، ولكن Data يساوي null، فإن الصورة تكون مرتبطة ولا تُخزن في الملف.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

### setText(String value) {#setText-java.lang.String-}
```
public void setText(String value)
```


يمثل السلسلة في كائن TextBox هذا.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

### setTextWrapped(boolean value) {#setTextWrapped-boolean-}
```
public void setTextWrapped(boolean value)
```


يضبط نوع التفاف النص للشكل الذي يحتوي على نص.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setTitle(String value) {#setTitle-java.lang.String-}
```
public void setTitle(String value)
```


يحدد العنوان (التسمية) لكائن الشكل الحالي.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

### setTop(int value) {#setTop-int-}
```
public void setTop(int value)
```


يمثل الإزاحة العمودية للشكل من صفه العلوي، بوحدة البكسل.

**Remarks**

إذا كان الشكل داخل المخطط، يمثل الإزاحة العمودية للشكل من حدّه العلوي.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setTopCM(double value) {#setTopCM-double-}
```
public void setTopCM(double value)
```


يمثل الإزاحة العمودية للشكل من صفه العلوي، بوحدة السنتيمتر.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | double |  |

### setTopInch(double value) {#setTopInch-double-}
```
public void setTopInch(double value)
```


يمثل الإزاحة العمودية للشكل من صفه العلوي، بوحدة البوصة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | double |  |

### setTopToCorner(int value) {#setTopToCorner-int-}
```
public void setTopToCorner(int value)
```


يمثل الإزاحة العمودية للشكل من الحافة العلوية لورقة العمل، بوحدة البكسل.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setUpperDeltaX(int value) {#setUpperDeltaX-int-}
```
public void setUpperDeltaX(int value)
```


يضبط الإزاحة الأفقية للشكل من عمود زاويةه العلوية اليسرى. النطاق القيمي هو من 0 إلى 1024.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setUpperDeltaY(int value) {#setUpperDeltaY-int-}
```
public void setUpperDeltaY(int value)
```


يضبط الإزاحة العمودية للشكل من صف زاويةه العلوية اليسرى. النطاق القيمي هو من 0 إلى 256.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setUpperLeftColumn(int value) {#setUpperLeftColumn-int-}
```
public void setUpperLeftColumn(int value)
```


يمثل فهرس عمود الزاوية العلوية اليسرى.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setUpperLeftRow(int value) {#setUpperLeftRow-int-}
```
public void setUpperLeftRow(int value)
```


يمثل فهرس الصف للزاوية العلوية اليسرى.

**Remarks**

إذا كان الشكل داخل شكل آخر أو داخل مجموعة، سيتم تجاهل UpperLeftRow.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setWidth(int value) {#setWidth-int-}
```
public void setWidth(int value)
```


يمثل عرض الشكل، بوحدة البكسل.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setWidthCM(double value) {#setWidthCM-double-}
```
public void setWidthCM(double value)
```


يمثل عرض الشكل، بوحدة السنتيمتر.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | double |  |

### setWidthInch(double value) {#setWidthInch-double-}
```
public void setWidthInch(double value)
```


يمثل عرض الشكل، بوحدة البوصة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | double |  |

### setWidthPt(double value) {#setWidthPt-double-}
```
public void setWidthPt(double value)
```


يمثل عرض الشكل، بوحدة النقطة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | double |  |

### setWidthScale(int value) {#setWidthScale-int-}
```
public void setWidthScale(int value)
```


يضبط مقياس العرض، بوحدة النسبة المئوية من عرض الصورة الأصلية. إذا لم يكن الشكل صورة، فإن الخاصية WidthScale تُعيد 100 فقط؛

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setX(int value) {#setX-int-}
```
public void setX(int value)
```


يضبط الإزاحة الأفقية للشكل من الحد الأيسر للورقة، بوحدة البكسل.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setY(int value) {#setY-int-}
```
public void setY(int value)
```


يضبط الإزاحة العمودية للشكل من الحد العلوي لورقة العمل، بوحدة البكسل.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setZOrderPosition(int value) {#setZOrderPosition-int-}
```
public void setZOrderPosition(int value)
```


يعيد موضع الشكل في ترتيب z.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

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

