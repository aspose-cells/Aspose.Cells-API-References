---
title: "TextBoxActiveXControl"
second_title: "Aspose.Cells for Java API Reference"
description: "يمثل عنصر تحكم ActiveX لمربع النص."
type: docs
url: /ar/java/com.aspose.cells/textboxactivexcontrol/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.ActiveXControlBase](../../com.aspose.cells/activexcontrolbase), [com.aspose.cells.ActiveXControl](../../com.aspose.cells/activexcontrol)
```
public class TextBoxActiveXControl extends ActiveXControl
```

يمثل عنصر تحكم ActiveX لمربع النص.

**Example**

```
         //Initialize a new workbook.
         Workbook book = new Workbook();
 
         //Add a TextBoxActiveXControl.
         Shape shape = book.getWorksheets().get(0).getShapes().addActiveXControl(ControlType.TEXT_BOX, 1, 0, 1, 0, 100, 50);
         TextBoxActiveXControl activeXControl = (TextBoxActiveXControl)shape.getActiveXControl();
 
         //do your business
 
         //Save the excel file.
         book.save("exmaple.xlsx");
```
## الطرق

| طريقة | الوصف |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getBackOleColor()](#getBackOleColor--) | يحصل على لون ole للخلفية. |
| [getBorderOleColor()](#getBorderOleColor--) | يحصل على لون ole للخلفية. |
| [getBorderStyle()](#getBorderStyle--) | يحصل على نوع الحد المستخدم من قبل التحكم. |
| [getClass()](#getClass--) |  |
| [getData()](#getData--) | يحصل على البيانات الثنائية للتحكم. |
| [getDropButtonStyle()](#getDropButtonStyle--) | يحدد الرمز المعروض على زر القائمة المنسدلة |
| [getEnterFieldBehavior()](#getEnterFieldBehavior--) | يحدد سلوك التحديد عند دخول التحكم. |
| [getEnterKeyBehavior()](#getEnterKeyBehavior--) | يحدد سلوك مفتاح ENTER. |
| [getFont()](#getFont--) | يمثل خط التحكم. |
| [getForeOleColor()](#getForeOleColor--) | يحصل على لون OLE للمقدمة. |
| [getHeight()](#getHeight--) | يحصل على ارتفاع التحكم بوحدة النقاط. |
| [getHideSelection()](#getHideSelection--) | يشير إلى ما إذا كان النص المحدد في التحكم يظهر مميزًا عندما لا يكون للتحكم تركيز. |
| [getIMEMode()](#getIMEMode--) | يحصل على وضع التشغيل الافتراضي لمحرر طريقة الإدخال للتحكم عند استلامه للتركيز. |
| [getIntegralHeight()](#getIntegralHeight--) | يشير إلى ما إذا كان التحكم سيظهر فقط أسطر النص الكاملة دون إظهار أي أسطر جزئية. |
| [getLinkedCell()](#getLinkedCell--) | يحصل على الخلية المرتبطة. |
| [getListFillRange()](#getListFillRange--) | يحصل على نطاق تعبئة القائمة. |
| [getMaxLength()](#getMaxLength--) | يحصل على الحد الأقصى لعدد الأحرف |
| [getMouseIcon()](#getMouseIcon--) | يحصل على أيقونة مخصصة لعرضها كمؤشر الفأرة للتحكم. |
| [getMousePointer()](#getMousePointer--) | يحصل على نوع الأيقونة المعروضة كمؤشر الفأرة للتحكم. |
| [getPasswordChar()](#getPasswordChar--) | يحصل على حرف يُعرض بدلاً من الأحرف التي تم إدخالها. |
| [getScrollBars()](#getScrollBars--) | يشير إلى ما إذا كان التحكم يحتوي على أشرطة تمرير عمودية، أشرطة تمرير أفقية، كلاهما، أو لا شيء. |
| [getShadow()](#getShadow--) | يشير إلى ما إذا كان يجب إظهار الظل. |
| [getShowDropButtonTypeWhen()](#getShowDropButtonTypeWhen--) | يحدد الرمز المعروض على زر القائمة المنسدلة |
| [getSpecialEffect()](#getSpecialEffect--) | يحصل على التأثير الخاص للتحكم. |
| [getTabKeyBehavior()](#getTabKeyBehavior--) | يشير إلى ما إذا كانت مسافات التبويب مسموحة في نص التحكم. |
| [getText()](#getText--) | يحصل على نص التحكم. |
| [getTextAlign()](#getTextAlign--) | يمثل طريقة محاذاة النص المستخدم في التحكم. |
| [getType()](#getType--) | يحصل على نوع عنصر التحكم ActiveX. |
| [getWidth()](#getWidth--) | يحصل على عرض التحكم بوحدة النقاط. |
| [getWorkbook()](#getWorkbook--) | يحصل على كائن [getWorkbook()](../../com.aspose.cells/activexcontrolbase\#getWorkbook--). |
| [hashCode()](#hashCode--) |  |
| [isAutoSize()](#isAutoSize--) | يشير إلى ما إذا كان التحكم سيعيد تحجيمه تلقائيًا لعرض محتوياته بالكامل. |
| [isAutoTab()](#isAutoTab--) | يشير إلى ما إذا كان التركيز سيتحرك تلقائيًا إلى التحكم التالي عندما يدخل المستخدم الحد الأقصى لعدد الأحرف. |
| [isAutoWordSelected()](#isAutoWordSelected--) | يحدد الوحدة الأساسية المستخدمة لتوسيع التحديد. |
| [isDragBehaviorEnabled()](#isDragBehaviorEnabled--) | يشير إلى ما إذا كان السحب والإفلات مفعلاً للتحكم. |
| [isEditable()](#isEditable--) | يشير إلى ما إذا كان المستخدم يمكنه الكتابة في التحكم. |
| [isEnabled()](#isEnabled--) | يشير إلى ما إذا كان التحكم يمكنه استلام التركيز والاستجابة للأحداث التي يولدها المستخدم. |
| [isLocked()](#isLocked--) | يشير إلى ما إذا كانت البيانات في التحكم مقفلة للتحرير. |
| [isMultiLine()](#isMultiLine--) | يشير إلى ما إذا كان التحكم يمكنه عرض أكثر من سطر نص واحد. |
| [isTransparent()](#isTransparent--) | يشير إلى ما إذا كان التحكم شفافًا. |
| [isVisible()](#isVisible--) | يشير إلى ما إذا كان هذا التحكم مرئيًا. |
| [isWordWrapped()](#isWordWrapped--) | يشير إلى ما إذا كانت محتويات العنصر تُلتف تلقائيًا في نهاية السطر. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAutoSize(boolean value)](#setAutoSize-boolean-) | يشير إلى ما إذا كان التحكم سيعيد تحجيمه تلقائيًا لعرض محتوياته بالكامل. |
| [setAutoTab(boolean value)](#setAutoTab-boolean-) | يشير إلى ما إذا كان التركيز سيتحرك تلقائيًا إلى التحكم التالي عندما يدخل المستخدم الحد الأقصى لعدد الأحرف. |
| [setAutoWordSelected(boolean value)](#setAutoWordSelected-boolean-) | يحدد الوحدة الأساسية المستخدمة لتوسيع التحديد. |
| [setBackOleColor(int value)](#setBackOleColor-int-) | يضبط لون OLE للخلفية. |
| [setBorderOleColor(int value)](#setBorderOleColor-int-) | يضبط لون OLE للخلفية. |
| [setBorderStyle(int value)](#setBorderStyle-int-) | يضبط نوع الحد المستخدم من قبل التحكم. |
| [setDragBehaviorEnabled(boolean value)](#setDragBehaviorEnabled-boolean-) | يشير إلى ما إذا كان السحب والإفلات مفعلاً للتحكم. |
| [setDropButtonStyle(int value)](#setDropButtonStyle-int-) | يحدد الرمز المعروض على زر القائمة المنسدلة |
| [setEditable(boolean value)](#setEditable-boolean-) | يشير إلى ما إذا كان المستخدم يمكنه الكتابة في التحكم. |
| [setEnabled(boolean value)](#setEnabled-boolean-) | يشير إلى ما إذا كان التحكم يمكنه استلام التركيز والاستجابة للأحداث التي يولدها المستخدم. |
| [setEnterFieldBehavior(boolean value)](#setEnterFieldBehavior-boolean-) | يحدد سلوك التحديد عند دخول التحكم. |
| [setEnterKeyBehavior(boolean value)](#setEnterKeyBehavior-boolean-) | يحدد سلوك مفتاح ENTER. |
| [setForeOleColor(int value)](#setForeOleColor-int-) | يضبط لون OLE للمقدمة. |
| [setHeight(double value)](#setHeight-double-) | يضبط ارتفاع التحكم بوحدة النقاط. |
| [setHideSelection(boolean value)](#setHideSelection-boolean-) | يشير إلى ما إذا كان النص المحدد في التحكم يظهر مميزًا عندما لا يكون للتحكم تركيز. |
| [setIMEMode(int value)](#setIMEMode-int-) | يضبط وضع التشغيل الافتراضي لمحرر طريقة الإدخال للتحكم عند استلامه للتركيز. |
| [setIntegralHeight(boolean value)](#setIntegralHeight-boolean-) | يشير إلى ما إذا كان التحكم سيظهر فقط أسطر النص الكاملة دون إظهار أي أسطر جزئية. |
| [setLinkedCell(String value)](#setLinkedCell-java.lang.String-) | يضبط الخلية المرتبطة. |
| [setListFillRange(String value)](#setListFillRange-java.lang.String-) | يضبط نطاق تعبئة القائمة. |
| [setLocked(boolean value)](#setLocked-boolean-) | يشير إلى ما إذا كانت البيانات في التحكم مقفلة للتحرير. |
| [setMaxLength(int value)](#setMaxLength-int-) | يضبط الحد الأقصى لعدد الأحرف |
| [setMouseIcon(byte[] value)](#setMouseIcon-byte---) | يضبط أيقونة مخصصة لتظهر كمؤشر الفأرة للتحكم. |
| [setMousePointer(int value)](#setMousePointer-int-) | يضبط نوع الأيقونة المعروضة كمؤشر الفأرة للتحكم. |
| [setMultiLine(boolean value)](#setMultiLine-boolean-) | يشير إلى ما إذا كان التحكم يمكنه عرض أكثر من سطر نص واحد. |
| [setPasswordChar(char value)](#setPasswordChar-char-) | يضبط حرفًا يُعرض بدلاً من الأحرف التي تم إدخالها. |
| [setScrollBars(int value)](#setScrollBars-int-) | يشير إلى ما إذا كان التحكم يحتوي على أشرطة تمرير عمودية، أشرطة تمرير أفقية، كلاهما، أو لا شيء. |
| [setShadow(boolean value)](#setShadow-boolean-) | يشير إلى ما إذا كان يجب إظهار الظل. |
| [setShowDropButtonTypeWhen(int value)](#setShowDropButtonTypeWhen-int-) | يحدد الرمز المعروض على زر القائمة المنسدلة |
| [setSpecialEffect(int value)](#setSpecialEffect-int-) | يضبط التأثير الخاص للتحكم. |
| [setTabKeyBehavior(boolean value)](#setTabKeyBehavior-boolean-) | يشير إلى ما إذا كانت مسافات التبويب مسموحة في نص التحكم. |
| [setText(String value)](#setText-java.lang.String-) | يضبط نص التحكم. |
| [setTextAlign(int value)](#setTextAlign-int-) | يمثل طريقة محاذاة النص المستخدم في التحكم. |
| [setTransparent(boolean value)](#setTransparent-boolean-) | يشير إلى ما إذا كان التحكم شفافًا. |
| [setVisible(boolean value)](#setVisible-boolean-) | يشير إلى ما إذا كان هذا التحكم مرئيًا. |
| [setWidth(double value)](#setWidth-double-) | يضبط عرض التحكم بوحدة النقاط. |
| [setWordWrapped(boolean value)](#setWordWrapped-boolean-) | يشير إلى ما إذا كانت محتويات العنصر تُلتف تلقائيًا في نهاية السطر. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
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
### getBackOleColor() {#getBackOleColor--}
```
public int getBackOleColor()
```


يحصل على لون ole للخلفية.

**Returns:**
int
### getBorderOleColor() {#getBorderOleColor--}
```
public int getBorderOleColor()
```


يحصل على لون ole للخلفية.

**Example**

```
         //excel default color system 12 or green(0x0000FF00)
         activeXControl.setBorderOleColor(/*unchecked*/((int)0x80000012L));
```

**Returns:**
int
### getBorderStyle() {#getBorderStyle--}
```
public int getBorderStyle()
```


يحصل على نوع الحد المستخدم من قبل التحكم.

انظر [ControlBorderType](../../com.aspose.cells/controlbordertype).

**Example**

```
         activeXControl.setBorderStyle(com.aspose.cells.ControlBorderType.SINGLE);
```

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


يحصل على البيانات الثنائية للتحكم.

**Returns:**
byte[]
### getDropButtonStyle() {#getDropButtonStyle--}
```
public int getDropButtonStyle()
```


يحدد الرمز المعروض على زر القائمة المنسدلة

انظر [DropButtonStyle](../../com.aspose.cells/dropbuttonstyle).

**Example**

```
         activeXControl.setDropButtonStyle(com.aspose.cells.DropButtonStyle.ARROW);
```

**Returns:**
int
### getEnterFieldBehavior() {#getEnterFieldBehavior--}
```
public boolean getEnterFieldBehavior()
```


يحدد سلوك التحديد عند دخول التحكم. True يحدد أن التحديد يبقى دون تغيير منذ آخر مرة كان فيها التحكم نشطًا. False يحدد أنه سيتم تحديد كل النص داخل التحكم عند دخول التحكم.

**Example**

```
         if(!activeXControl.getEnterFieldBehavior())
         {
             activeXControl.setEnterFieldBehavior(true);
         }
```

**Returns:**
boolean
### getEnterKeyBehavior() {#getEnterKeyBehavior--}
```
public boolean getEnterKeyBehavior()
```


يحدد سلوك مفتاح ENTER. true يعني أن الضغط على ENTER سيخلق سطرًا جديدًا. false يعني أن الضغط على ENTER سينقل التركيز إلى الكائن التالي في ترتيب التبويب.

**Example**

```
         if(!activeXControl.getEnterKeyBehavior())
         {
             activeXControl.setEnterKeyBehavior(true);
         }
```

**Returns:**
boolean
### getFont() {#getFont--}
```
public Font getFont()
```


يمثل خط التحكم.

**Returns:**
[Font](../../com.aspose.cells/font)
### getForeOleColor() {#getForeOleColor--}
```
public int getForeOleColor()
```


يحصل على لون OLE للمقدمة.

**Remarks**

لا ينطبق على التحكم بالصورة.

**Returns:**
int
### getHeight() {#getHeight--}
```
public double getHeight()
```


يحصل على ارتفاع التحكم بوحدة النقاط.

**Returns:**
double
### getHideSelection() {#getHideSelection--}
```
public boolean getHideSelection()
```


يشير إلى ما إذا كان النص المحدد في التحكم يظهر مميزًا عندما لا يكون للتحكم تركيز.

**Example**

```
         if(!activeXControl.getHideSelection())
         {
             activeXControl.setHideSelection(true);
         }
```

**Returns:**
boolean
### getIMEMode() {#getIMEMode--}
```
public int getIMEMode()
```


يحصل على وضع التشغيل الافتراضي لمحرر طريقة الإدخال للتحكم عند استلامه للتركيز.

انظر [InputMethodEditorMode](../../com.aspose.cells/inputmethodeditormode).

**Returns:**
int
### getIntegralHeight() {#getIntegralHeight--}
```
public boolean getIntegralHeight()
```


يشير إلى ما إذا كان التحكم سيظهر فقط أسطر النص الكاملة دون إظهار أي أسطر جزئية.

**Example**

```
         if(!activeXControl.getIntegralHeight())
         {
             activeXControl.setIntegralHeight(true);
         }
```

**Returns:**
boolean
### getLinkedCell() {#getLinkedCell--}
```
public String getLinkedCell()
```


يحصل على الخلية المرتبطة.

**Returns:**
java.lang.String
### getListFillRange() {#getListFillRange--}
```
public String getListFillRange()
```


يحصل على نطاق تعبئة القائمة.

**Returns:**
java.lang.String
### getMaxLength() {#getMaxLength--}
```
public int getMaxLength()
```


يحصل على الحد الأقصى لعدد الأحرف

**Example**

```
         if(activeXControl.getMaxLength() == 0)
         {
             activeXControl.setMaxLength(30);
         }
```

**Returns:**
int
### getMouseIcon() {#getMouseIcon--}
```
public byte[] getMouseIcon()
```


يحصل على أيقونة مخصصة لعرضها كمؤشر الفأرة للتحكم.

**Returns:**
byte[]
### getMousePointer() {#getMousePointer--}
```
public int getMousePointer()
```


يحصل على نوع الأيقونة المعروضة كمؤشر الفأرة للتحكم.

انظر [ControlMousePointerType](../../com.aspose.cells/controlmousepointertype).

**Returns:**
int
### getPasswordChar() {#getPasswordChar--}
```
public char getPasswordChar()
```


يحصل على حرف يُعرض بدلاً من الأحرف التي تم إدخالها.

**Example**

```
         activeXControl.setPasswordChar('a');
```

**Returns:**
char
### getScrollBars() {#getScrollBars--}
```
public int getScrollBars()
```


يشير إلى ما إذا كان التحكم يحتوي على أشرطة تمرير عمودية، أشرطة تمرير أفقية، كلاهما، أو لا شيء.

انظر [ControlScrollBarType](../../com.aspose.cells/controlscrollbartype).

**Example**

```
         activeXControl.setScrollBars(com.aspose.cells.ControlScrollBarType.BARS_VERTICAL);
```

**Returns:**
int
### getShadow() {#getShadow--}
```
public boolean getShadow()
```


يشير إلى ما إذا كان يجب إظهار الظل.

**Returns:**
boolean
### getShowDropButtonTypeWhen() {#getShowDropButtonTypeWhen--}
```
public int getShowDropButtonTypeWhen()
```


يحدد الرمز المعروض على زر القائمة المنسدلة

انظر [ShowDropButtonType](../../com.aspose.cells/showdropbuttontype).

**Example**

```
         activeXControl.setShowDropButtonTypeWhen(com.aspose.cells.ShowDropButtonType.FOCUS);
```

**Returns:**
int
### getSpecialEffect() {#getSpecialEffect--}
```
public int getSpecialEffect()
```


يحصل على التأثير الخاص للتحكم.

انظر [ControlSpecialEffectType](../../com.aspose.cells/controlspecialeffecttype).

**Example**

```
         activeXControl.setSpecialEffect(com.aspose.cells.ControlSpecialEffectType.BUMP);
```

**Returns:**
int
### getTabKeyBehavior() {#getTabKeyBehavior--}
```
public boolean getTabKeyBehavior()
```


يشير إلى ما إذا كانت مسافات التبويب مسموحة في نص التحكم.

**Example**

```
         if(!activeXControl.getTabKeyBehavior())
         {
             activeXControl.setTabKeyBehavior(true);
         }
```

**Returns:**
boolean
### getText() {#getText--}
```
public String getText()
```


يحصل على نص التحكم.

**Example**

```
         activeXControl.setText("This is a test.");
```

**Returns:**
java.lang.String
### getTextAlign() {#getTextAlign--}
```
public int getTextAlign()
```


يمثل طريقة محاذاة النص المستخدم في التحكم.

انظر [TextAlignmentType](../../com.aspose.cells/textalignmenttype).

**Returns:**
int
### getType() {#getType--}
```
public int getType()
```


يحصل على نوع عنصر التحكم ActiveX.

انظر [ControlType](../../com.aspose.cells/controltype).

**Example**

```
         /*Aspose.Cells.Drawing.ActiveXControls.ControlType*/int type = activeXControl.getType();
```

**Returns:**
int
### getWidth() {#getWidth--}
```
public double getWidth()
```


يحصل على عرض التحكم بوحدة النقاط.

**Returns:**
double
### getWorkbook() {#getWorkbook--}
```
public Workbook getWorkbook()
```


يحصل على كائن [getWorkbook()](../../com.aspose.cells/activexcontrolbase\#getWorkbook--).

**Returns:**
[Workbook](../../com.aspose.cells/workbook)
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isAutoSize() {#isAutoSize--}
```
public boolean isAutoSize()
```


يشير إلى ما إذا كان التحكم سيعيد تحجيمه تلقائيًا لعرض محتوياته بالكامل.

**Returns:**
boolean
### isAutoTab() {#isAutoTab--}
```
public boolean isAutoTab()
```


يشير إلى ما إذا كان التركيز سيتحرك تلقائيًا إلى التحكم التالي عندما يدخل المستخدم الحد الأقصى لعدد الأحرف.

**Example**

```
         if(!activeXControl.isAutoTab())
         {
             activeXControl.setAutoTab(true);
         }
```

**Returns:**
boolean
### isAutoWordSelected() {#isAutoWordSelected--}
```
public boolean isAutoWordSelected()
```


يحدد الوحدة الأساسية المستخدمة لتوسيع التحديد. True يحدد أن الوحدة الأساسية هي حرف واحد. false يحدد أن الوحدة الأساسية هي كلمة كاملة.

**Example**

```
         if(!activeXControl.isAutoWordSelected())
         {
             activeXControl.setAutoWordSelected(true);
         }
```

**Returns:**
boolean
### isDragBehaviorEnabled() {#isDragBehaviorEnabled--}
```
public boolean isDragBehaviorEnabled()
```


يشير إلى ما إذا كان السحب والإفلات مفعلاً للتحكم.

**Example**

```
         if(!activeXControl.isDragBehaviorEnabled())
         {
             activeXControl.setDragBehaviorEnabled(true);
         }
```

**Returns:**
boolean
### isEditable() {#isEditable--}
```
public boolean isEditable()
```


يشير إلى ما إذا كان المستخدم يمكنه الكتابة في التحكم.

**Example**

```
         if(!activeXControl.isEditable())
         {
             activeXControl.setEditable(true);
         }
```

**Returns:**
boolean
### isEnabled() {#isEnabled--}
```
public boolean isEnabled()
```


يشير إلى ما إذا كان التحكم يمكنه استلام التركيز والاستجابة للأحداث التي يولدها المستخدم.

**Returns:**
boolean
### isLocked() {#isLocked--}
```
public boolean isLocked()
```


يشير إلى ما إذا كانت البيانات في التحكم مقفلة للتحرير.

**Returns:**
boolean
### isMultiLine() {#isMultiLine--}
```
public boolean isMultiLine()
```


يشير إلى ما إذا كان التحكم يمكنه عرض أكثر من سطر نص واحد.

**Example**

```
         if(!activeXControl.isMultiLine())
         {
             activeXControl.setMultiLine(true);
         }
```

**Returns:**
boolean
### isTransparent() {#isTransparent--}
```
public boolean isTransparent()
```


يشير إلى ما إذا كان التحكم شفافًا.

**Returns:**
boolean
### isVisible() {#isVisible--}
```
public boolean isVisible()
```


يشير إلى ما إذا كان هذا التحكم مرئيًا.

**Returns:**
boolean
### isWordWrapped() {#isWordWrapped--}
```
public boolean isWordWrapped()
```


يشير إلى ما إذا كانت محتويات العنصر تُلتف تلقائيًا في نهاية السطر.

**Example**

```
         if(!activeXControl.isWordWrapped())
         {
             activeXControl.setWordWrapped(true);
         }
```

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




### setAutoSize(boolean value) {#setAutoSize-boolean-}
```
public void setAutoSize(boolean value)
```


يشير إلى ما إذا كان التحكم سيعيد تحجيمه تلقائيًا لعرض محتوياته بالكامل.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setAutoTab(boolean value) {#setAutoTab-boolean-}
```
public void setAutoTab(boolean value)
```


يشير إلى ما إذا كان التركيز سيتحرك تلقائيًا إلى التحكم التالي عندما يدخل المستخدم الحد الأقصى لعدد الأحرف.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setAutoWordSelected(boolean value) {#setAutoWordSelected-boolean-}
```
public void setAutoWordSelected(boolean value)
```


يحدد الوحدة الأساسية المستخدمة لتوسيع التحديد. True يحدد أن الوحدة الأساسية هي حرف واحد. false يحدد أن الوحدة الأساسية هي كلمة كاملة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setBackOleColor(int value) {#setBackOleColor-int-}
```
public void setBackOleColor(int value)
```


يضبط لون OLE للخلفية.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setBorderOleColor(int value) {#setBorderOleColor-int-}
```
public void setBorderOleColor(int value)
```


يضبط لون OLE للخلفية.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setBorderStyle(int value) {#setBorderStyle-int-}
```
public void setBorderStyle(int value)
```


يضبط نوع الحد المستخدم من قبل التحكم.

انظر [ControlBorderType](../../com.aspose.cells/controlbordertype).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setDragBehaviorEnabled(boolean value) {#setDragBehaviorEnabled-boolean-}
```
public void setDragBehaviorEnabled(boolean value)
```


يشير إلى ما إذا كان السحب والإفلات مفعلاً للتحكم.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setDropButtonStyle(int value) {#setDropButtonStyle-int-}
```
public void setDropButtonStyle(int value)
```


يحدد الرمز المعروض على زر القائمة المنسدلة

انظر [DropButtonStyle](../../com.aspose.cells/dropbuttonstyle).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setEditable(boolean value) {#setEditable-boolean-}
```
public void setEditable(boolean value)
```


يشير إلى ما إذا كان المستخدم يمكنه الكتابة في التحكم.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setEnabled(boolean value) {#setEnabled-boolean-}
```
public void setEnabled(boolean value)
```


يشير إلى ما إذا كان التحكم يمكنه استلام التركيز والاستجابة للأحداث التي يولدها المستخدم.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setEnterFieldBehavior(boolean value) {#setEnterFieldBehavior-boolean-}
```
public void setEnterFieldBehavior(boolean value)
```


يحدد سلوك التحديد عند دخول التحكم. True يحدد أن التحديد يبقى دون تغيير منذ آخر مرة كان فيها التحكم نشطًا. False يحدد أنه سيتم تحديد كل النص داخل التحكم عند دخول التحكم.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setEnterKeyBehavior(boolean value) {#setEnterKeyBehavior-boolean-}
```
public void setEnterKeyBehavior(boolean value)
```


يحدد سلوك مفتاح ENTER. true يعني أن الضغط على ENTER سيخلق سطرًا جديدًا. false يعني أن الضغط على ENTER سينقل التركيز إلى الكائن التالي في ترتيب التبويب.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setForeOleColor(int value) {#setForeOleColor-int-}
```
public void setForeOleColor(int value)
```


يضبط لون OLE للمقدمة.

**Remarks**

لا ينطبق على التحكم بالصورة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setHeight(double value) {#setHeight-double-}
```
public void setHeight(double value)
```


يضبط ارتفاع التحكم بوحدة النقاط.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | double |  |

### setHideSelection(boolean value) {#setHideSelection-boolean-}
```
public void setHideSelection(boolean value)
```


يشير إلى ما إذا كان النص المحدد في التحكم يظهر مميزًا عندما لا يكون للتحكم تركيز.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setIMEMode(int value) {#setIMEMode-int-}
```
public void setIMEMode(int value)
```


يضبط وضع التشغيل الافتراضي لمحرر طريقة الإدخال للتحكم عند استلامه للتركيز.

انظر [InputMethodEditorMode](../../com.aspose.cells/inputmethodeditormode).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setIntegralHeight(boolean value) {#setIntegralHeight-boolean-}
```
public void setIntegralHeight(boolean value)
```


يشير إلى ما إذا كان التحكم سيظهر فقط أسطر النص الكاملة دون إظهار أي أسطر جزئية.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setLinkedCell(String value) {#setLinkedCell-java.lang.String-}
```
public void setLinkedCell(String value)
```


يضبط الخلية المرتبطة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

### setListFillRange(String value) {#setListFillRange-java.lang.String-}
```
public void setListFillRange(String value)
```


يضبط نطاق تعبئة القائمة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

### setLocked(boolean value) {#setLocked-boolean-}
```
public void setLocked(boolean value)
```


يشير إلى ما إذا كانت البيانات في التحكم مقفلة للتحرير.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setMaxLength(int value) {#setMaxLength-int-}
```
public void setMaxLength(int value)
```


يضبط الحد الأقصى لعدد الأحرف

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setMouseIcon(byte[] value) {#setMouseIcon-byte---}
```
public void setMouseIcon(byte[] value)
```


يضبط أيقونة مخصصة لتظهر كمؤشر الفأرة للتحكم.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | byte[] |  |

### setMousePointer(int value) {#setMousePointer-int-}
```
public void setMousePointer(int value)
```


يضبط نوع الأيقونة المعروضة كمؤشر الفأرة للتحكم.

انظر [ControlMousePointerType](../../com.aspose.cells/controlmousepointertype).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setMultiLine(boolean value) {#setMultiLine-boolean-}
```
public void setMultiLine(boolean value)
```


يشير إلى ما إذا كان التحكم يمكنه عرض أكثر من سطر نص واحد.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setPasswordChar(char value) {#setPasswordChar-char-}
```
public void setPasswordChar(char value)
```


يضبط حرفًا يُعرض بدلاً من الأحرف التي تم إدخالها.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | char |  |

### setScrollBars(int value) {#setScrollBars-int-}
```
public void setScrollBars(int value)
```


يشير إلى ما إذا كان التحكم يحتوي على أشرطة تمرير عمودية، أشرطة تمرير أفقية، كلاهما، أو لا شيء.

انظر [ControlScrollBarType](../../com.aspose.cells/controlscrollbartype).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setShadow(boolean value) {#setShadow-boolean-}
```
public void setShadow(boolean value)
```


يشير إلى ما إذا كان يجب إظهار الظل.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setShowDropButtonTypeWhen(int value) {#setShowDropButtonTypeWhen-int-}
```
public void setShowDropButtonTypeWhen(int value)
```


يحدد الرمز المعروض على زر القائمة المنسدلة

انظر [ShowDropButtonType](../../com.aspose.cells/showdropbuttontype).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setSpecialEffect(int value) {#setSpecialEffect-int-}
```
public void setSpecialEffect(int value)
```


يضبط التأثير الخاص للتحكم.

انظر [ControlSpecialEffectType](../../com.aspose.cells/controlspecialeffecttype).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setTabKeyBehavior(boolean value) {#setTabKeyBehavior-boolean-}
```
public void setTabKeyBehavior(boolean value)
```


يشير إلى ما إذا كانت مسافات التبويب مسموحة في نص التحكم.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setText(String value) {#setText-java.lang.String-}
```
public void setText(String value)
```


يضبط نص التحكم.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

### setTextAlign(int value) {#setTextAlign-int-}
```
public void setTextAlign(int value)
```


يمثل طريقة محاذاة النص المستخدم في التحكم.

انظر [TextAlignmentType](../../com.aspose.cells/textalignmenttype).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setTransparent(boolean value) {#setTransparent-boolean-}
```
public void setTransparent(boolean value)
```


يشير إلى ما إذا كان التحكم شفافًا.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setVisible(boolean value) {#setVisible-boolean-}
```
public void setVisible(boolean value)
```


يشير إلى ما إذا كان هذا التحكم مرئيًا.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setWidth(double value) {#setWidth-double-}
```
public void setWidth(double value)
```


يضبط عرض التحكم بوحدة النقاط.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | double |  |

### setWordWrapped(boolean value) {#setWordWrapped-boolean-}
```
public void setWordWrapped(boolean value)
```


يشير إلى ما إذا كانت محتويات العنصر تُلتف تلقائيًا في نهاية السطر.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

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

