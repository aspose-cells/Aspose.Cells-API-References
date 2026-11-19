---
title: "شريط تمرير"
second_title: "Aspose.Cells for Java API Reference"
description: "يمثل كائن شريط تمرير."
type: docs
url: /ar/java/com.aspose.cells/scrollbar/
---

**Inheritance:**
java.lang.Object، [com.aspose.cells.Shape](../../com.aspose.cells/shape)
```
public class ScrollBar extends Shape
```

يمثل كائن شريط تمرير.

**Remarks**

يجب أن تكون قيمة التمرير بين 0 و 30000.
## الطرق

| طريقة | الوصف |
| --- | --- |
| [addHyperlink(String address)](#addHyperlink-java.lang.String-) | يضيف ارتباطًا تشعبيًا إلى الشكل. |
| [alignTopRightCorner(int topRow, int rightColumn)](#alignTopRightCorner-int-int-) | ينقل الصورة إلى الزاوية العليا اليمنى. |
| [calculateTextSize()](#calculateTextSize--) | إعادة حساب منطقة النص |
| [characters(int startIndex, int length)](#characters-int-int-) | يرجع كائن Characters يمثل نطاقًا من الأحرف داخل النص. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [fitToTextSize()](#fitToTextSize--) | إعادة حساب منطقة نصية مناسبة لعرض كل محتوى النص. |
| [formatCharacters(int startIndex, int length, Font font, StyleFlag flag)](#formatCharacters-int-int-com.aspose.cells.Font-com.aspose.cells.StyleFlag-) | يقوم بتنسيق بعض الأحرف باستخدام إعداد الخط. |
| [getActiveXControl()](#getActiveXControl--) | يحصل على عنصر التحكم ActiveX. |
| [getActualBox()](#getActualBox--) | احصل على الموضع والحجم الفعليين للشكل (بعد تطبيق الدوران أو الانعكاس، إلخ). |
| [getActualLowerRightRow()](#getActualLowerRightRow--) | احصل على الصف السفلي الفعلي. |
| [getAlternativeText()](#getAlternativeText--) | يرجع أو يضبط النص الوصفي (البديل) لكائن الـ [Shape](../../com.aspose.cells/shape). |
| [getAnchorType()](#getAnchorType--) | يحصل على نوع العنصر النائب لمرساة الشكل. |
| [getAutoShapeType()](#getAutoShapeType--) | يحصل على نوع الشكل التلقائي. |
| [getBottom()](#getBottom--) | يمثل عرض الإزاحة العمودية للشكل من صف زاوية أسفله السفلية، بوحدة البكسل. |
| [getCharacters()](#getCharacters--) | يرجع جميع كائنات Characters التي تمثل نطاقًا من الأحرف داخل النص. |
| [getClass()](#getClass--) |  |
| [getConnectionPoints()](#getConnectionPoints--) | احصل على نقاط الاتصال |
| [getControlData()](#getControlData--) | يحصل على بيانات التحكم. |
| [getCreateId()](#getCreateId--) | يحصل على معرف الإنشاء لهذا الشكل. |
| [getCurrentValue()](#getCurrentValue--) | يحصل على القيمة الحالية. |
| [getFill()](#getFill--) | يرجع كائن [getFillFormat()](../../com.aspose.cells/shape\#getFillFormat--) الذي يحتوي على خصائص تنسيق التعبئة للشكل المحدد. |
| [getFillFormat()](#getFillFormat--) | يرجع كائن MsoFillFormat الذي يحتوي على خصائص تنسيق التعبئة للشكل المحدد. |
| [getFont()](#getFont--) | يمثل خط الشكل. |
| [getFormatPicture()](#getFormatPicture--) | يحصل على خيارات تنسيق الصورة. |
| [getGeometry()](#getGeometry--) | يحصل على الهندسة |
| [getGlow()](#getGlow--) | يمثل كائن [GlowEffect](../../com.aspose.cells/gloweffect) الذي يحدد تأثير التوهج لعنصر المخطط أو الشكل. |
| [getGroup()](#getGroup--) | يحصل على الشكل الجماعي الذي يحتوي على هذا الشكل. |
| [getHeight()](#getHeight--) | يمثل ارتفاع الشكل، بوحدة البكسل. |
| [getHeightCM()](#getHeightCM--) | يمثل ارتفاع الشكل، بوحدة السنتيمتر. |
| [getHeightInShape()](#getHeightInShape--) | يمثل الإزاحة العمودية للشكل من الحد العلوي للشكل الأب، بوحدة 1/4000 من ارتفاع الشكل الأب. |
| [getHeightInch()](#getHeightInch--) | يمثل ارتفاع الشكل، بوحدة البوصة. |
| [getHeightPt()](#getHeightPt--) | يمثل ارتفاع الشكل، بوحدة النقاط. |
| [getHeightScale()](#getHeightScale--) | يحصل على مقياس الارتفاع، بوحدة النسبة المئوية من ارتفاع الصورة الأصلي. |
| [getHtmlText()](#getHtmlText--) | يحصل على سلسلة HTML التي تحتوي على البيانات وبعض التنسيقات في هذا مربع النص. |
| [getHyperlink()](#getHyperlink--) | يحصل على الارتباط التشعبي للشكل. |
| [getId()](#getId--) | يحصل على معرف هذا الشكل. |
| [getIncrementalChange()](#getIncrementalChange--) | يحصل على مقدار الزيادة التي يتم تطبيقها على شريط التمرير أو المؤشر عند تمرير سطر واحد. |
| [getInputRange()](#getInputRange--) | يحصل على نطاق ورقة العمل المستخدم لملء صندوق القائمة المحدد. |
| [getInputRange(boolean isR1C1, boolean isLocal)](#getInputRange-boolean-boolean-) | يحصل على النطاق المستخدم لملء التحكم. |
| [getLeft()](#getLeft--) | يمثل الإزاحة الأفقية للشكل من عموده الأيسر، بوحدة البكسل. |
| [getLeftCM()](#getLeftCM--) | يمثل الإزاحة الأفقية للشكل من عموده الأيسر، بوحدة السنتيمتر. |
| [getLeftInShape()](#getLeftInShape--) | يمثل الإزاحة الأفقية للشكل من الحد الأيسر للشكل الأب، بوحدة 1/4000 من عرض الشكل الأب. |
| [getLeftInch()](#getLeftInch--) | يمثل الإزاحة الأفقية للشكل من عموده الأيسر، بوحدة البوصة. |
| [getLeftToCorner()](#getLeftToCorner--) | يحصل على الإزاحة الأفقية للشكل من الحد الأيسر لورقة العمل. |
| [getLine()](#getLine--) | يحصل على نمط الخط |
| [getLineFormat()](#getLineFormat--) | يرجع كائن MsoLineFormat يحتوي على خصائص تنسيق الخط للشكل المحدد. |
| [getLinkedCell()](#getLinkedCell--) | يحصل على نطاق ورقة العمل المرتبط بقيمة التحكم. |
| [getLinkedCell(boolean isR1C1, boolean isLocal)](#getLinkedCell-boolean-boolean-) | يحصل على النطاق المرتبط بقيمة التحكم. |
| [getLockedProperty(int type)](#getLockedProperty-int-) | يحصل على قيمة الخاصية المقفلة. |
| [getLowerDeltaX()](#getLowerDeltaX--) | يحصل على الإزاحة الأفقية للشكل من عمود زاويةه السفلية اليمنى. |
| [getLowerDeltaY()](#getLowerDeltaY--) | يحصل على الإزاحة العمودية للشكل من صف زاويةه السفلية اليمنى. |
| [getLowerRightColumn()](#getLowerRightColumn--) | يمثل فهرس عمود الزاوية السفلية اليمنى. |
| [getLowerRightRow()](#getLowerRightRow--) | يمثل فهرس صف الزاوية السفلية اليمنى. |
| [getMacroName()](#getMacroName--) | يحصل على اسم الماكرو. |
| [getMax()](#getMax--) | يحصل على القيمة القصوى لنطاق شريط التمرير أو المؤشر. |
| [getMin()](#getMin--) | يحصل على القيمة الدنيا لنطاق شريط التمرير أو المؤشر. |
| [getMsoDrawingType()](#getMsoDrawingType--) | يحصل على نوع الرسم. |
| [getName()](#getName--) | يحصل على اسم الشكل. |
| [getPageChange()](#getPageChange--) | يحصل على تغيير الصفحة. |
| [getPaths()](#getPaths--) | يحصل على مسارات الشكل الهندسي المخصص. |
| [getPlacement()](#getPlacement--) | يمثل الطريقة التي يتم بها إرفاق كائن الرسم بالخلايا تحته. |
| [getReflection()](#getReflection--) | يمثل كائن [ReflectionEffect](../../com.aspose.cells/reflectioneffect) الذي يحدد تأثير الانعكاس لعنصر المخطط أو الشكل. |
| [getRelativeToOriginalPictureSize()](#getRelativeToOriginalPictureSize--) | يشير إلى ما إذا كان الشكل نسبيًا لحجم الصورة الأصلي. |
| [getResultOfSmartArt()](#getResultOfSmartArt--) | تحويل Smart Art إلى أشكال مجمعة. |
| [getRichFormattings()](#getRichFormattings--) | يرجع جميع كائنات Characters التي تمثل نطاقًا من الأحرف داخل النص. |
| [getRight()](#getRight--) | يمثل عرض الإزاحة الأفقية للشكل من عمود زاويةه السفلية اليمنى، بوحدة البكسل. |
| [getRotationAngle()](#getRotationAngle--) | يحصل على دوران الشكل. |
| [getShadow()](#getShadow--) | يشير إلى ما إذا كان الشكل يحتوي على تظليل ثلاثي الأبعاد. |
| [getShadowEffect()](#getShadowEffect--) | يمثل كائن [ShadowEffect](../../com.aspose.cells/shadoweffect) الذي يحدد تأثير الظل لعنصر المخطط أو الشكل. |
| [getSoftEdges()](#getSoftEdges--) | يحصل على نصف قطر الضبابية لتطبيقه على الحواف، بوحدة النقاط. |
| [getSpid()](#getSpid--) | يحدد معرف سلسلة اختياري يمكن للتطبيق استخدامه لتحديد الشكل المحدد. |
| [getSpt()](#getSpt--) | يحدد رقمًا اختياريًا يمكن للتطبيق استخدامه لربط الشكل المحدد بنوع شكل معرف. |
| [getText()](#getText--) | يحصل على نص هذا الشكل. |
| [getTextBody()](#getTextBody--) | يحصل على إعداد نص الشكل. |
| [getTextBoxOptions()](#getTextBoxOptions--) | يحصل على معلومات النص في الشكل |
| [getTextDirection()](#getTextDirection--) | يحصل على اتجاه تدفق النص لهذا الكائن. |
| [getTextEffect()](#getTextEffect--) | يرجع كائن TextEffectFormat يحتوي على خصائص تنسيق تأثير النص للشكل المحدد. |
| [getTextHorizontalAlignment()](#getTextHorizontalAlignment--) | يحصل على نوع محاذاة النص الأفقية للشكل. |
| [getTextHorizontalOverflow()](#getTextHorizontalOverflow--) | يحصل على نوع تجاوز النص الأفقي للشكل الذي يحتوي على النص. |
| [getTextOptions()](#getTextOptions--) | يمثل خيارات النص للشكل. |
| [getTextOrientationType()](#getTextOrientationType--) | يحصل على نوع توجيه النص للشكل. |
| [getTextShapeType()](#getTextShapeType--) | يحصل على نوع شكل النص المسبق. |
| [getTextVerticalAlignment()](#getTextVerticalAlignment--) | يحصل على نوع محاذاة النص العمودية للشكل. |
| [getTextVerticalOverflow()](#getTextVerticalOverflow--) | يحصل على نوع تجاوز النص العمودي للشكل الذي يحتوي على النص. |
| [getThreeDFormat()](#getThreeDFormat--) | يحصل على تنسيق ثلاثي الأبعاد للشكل. |
| [getTitle()](#getTitle--) | يحدد العنوان (التسمية) لكائن الشكل الحالي. |
| [getTop()](#getTop--) | يمثل الإزاحة العمودية للشكل من صفه العلوي، بوحدة البكسل. |
| [getTopCM()](#getTopCM--) | يمثل الإزاحة العمودية للشكل من صفه العلوي، بوحدة السنتيمتر. |
| [getTopInShape()](#getTopInShape--) | يمثل الإزاحة العمودية للشكل من الحد العلوي للشكل الأب، بوحدة 1/4000 من ارتفاع الشكل الأب. |
| [getTopInch()](#getTopInch--) | يمثل الإزاحة العمودية للشكل من صفه العلوي، بوحدة البوصة. |
| [getTopToCorner()](#getTopToCorner--) | يحصل على الإزاحة العمودية للشكل من الحد العلوي لورقة العمل، بوحدة البكسل. |
| [getType()](#getType--) | يحصل على نوع الشكل التلقائي. |
| [getUpperDeltaX()](#getUpperDeltaX--) | يحصل على الإزاحة الأفقية للشكل من عمود الزاوية العلوية اليسرى. |
| [getUpperDeltaY()](#getUpperDeltaY--) | يحصل على الإزاحة العمودية للشكل من صف الزاوية العلوية اليسرى. |
| [getUpperLeftColumn()](#getUpperLeftColumn--) | يمثل فهرس عمود الزاوية العلوية اليسرى. |
| [getUpperLeftRow()](#getUpperLeftRow--) | يمثل فهرس الصف العلوي. |
| [getWidth()](#getWidth--) | يمثل عرض الشكل، بوحدة البكسل. |
| [getWidthCM()](#getWidthCM--) | يمثل عرض الشكل، بوحدة السنتيمتر. |
| [getWidthInShape()](#getWidthInShape--) | يمثل عرض الشكل، بوحدة 1/4000 من الشكل الأصل. |
| [getWidthInch()](#getWidthInch--) | يمثل عرض الشكل، بوحدة البوصة. |
| [getWidthPt()](#getWidthPt--) | يمثل عرض الشكل، بوحدة النقطة. |
| [getWidthScale()](#getWidthScale--) | يحصل على مقياس العرض، بوحدة النسبة المئوية من عرض الصورة الأصلي. |
| [getWorksheet()](#getWorksheet--) | يحصل على كائن [Worksheet](../../com.aspose.cells/worksheet) الذي يحتوي على هذا الشكل. |
| [getX()](#getX--) | يحصل على الإزاحة الأفقية للشكل من الحد الأيسر للورقة، بوحدة البكسل. |
| [getY()](#getY--) | يحصل على الإزاحة العمودية للشكل من الحد العلوي للورقة، بوحدة البكسل. |
| [getZOrderPosition()](#getZOrderPosition--) | يعيد موضع الشكل في ترتيب z. |
| [hasLine()](#hasLine--) | يحصل على ما إذا كان حد الخط للشكل مرئيًا. |
| [hashCode()](#hashCode--) |  |
| [isAspectRatioLocked()](#isAspectRatioLocked--) | صحيح يعني أن نسبة أبعاد الشكل مقفلة. |
| [isDecorative()](#isDecorative--) | يشير إلى ما إذا كان الكائن زخرفيًا. |
| [isEquation()](#isEquation--) | يشير إلى ما إذا كان الشكل يحتوي فقط على معادلة. |
| [isFilled()](#isFilled--) | يشير إلى ما إذا كان تنسيق التعبئة مرئيًا. |
| [isFlippedHorizontally()](#isFlippedHorizontally--) | يحصل على ما إذا كان الشكل مقلوبًا أفقيًا. |
| [isFlippedVertically()](#isFlippedVertically--) | يحصل على ما إذا كان الشكل مقلوبًا عموديًا. |
| [isGroup()](#isGroup--) | يشير إلى ما إذا كان هذا الشكل شكل مجموعة. |
| [isHidden()](#isHidden--) | يشير إلى ما إذا كان الكائن مرئيًا. |
| [isHorizontal()](#isHorizontal--) | يشير إلى ما إذا كان هذا شريط تمرير أفقي. |
| [isInGroup()](#isInGroup--) | يشير إلى ما إذا كان الشكل مجموعة. |
| [isLockAspectRatio()](#isLockAspectRatio--) | صحيح يعني أن نسبة أبعاد الشكل مقفلة. |
| [isLocked()](#isLocked--) | صحيح يعني أن الكائن لا يمكن تعديله عندما تكون الورقة محمية. |
| [isPrintable()](#isPrintable--) | يشير إلى ما إذا كان الكائن قابلًا للطباعة. |
| [isRichText()](#isRichText--) | ما إذا كان النص نصًا غنيًا أم لا. |
| [isSameSetting(Object obj)](#isSameSetting-java.lang.Object-) | يعيد ما إذا كان الشكل متماثلًا. |
| [isSmartArt()](#isSmartArt--) | يشير إلى ما إذا كان الشكل فنًا ذكيًا. |
| [isTextWrapped()](#isTextWrapped--) | يحصل على نوع التفاف النص للشكل الذي يحتوي على نص. |
| [isWordArt()](#isWordArt--) | يشير إلى ما إذا كان هذا الشكل فن كلمة. |
| [moveToRange(int topRow, int leftColumn, int bottomRow, int rightColumn)](#moveToRange-int-int-int-int-) | ينقل الشكل إلى نطاق محدد. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [removeActiveXControl()](#removeActiveXControl--) | إزالة عنصر التحكم ActiveX. |
| [removeHyperlink()](#removeHyperlink--) | يزيل الارتباط التشعبي للشكل. |
| [setAlternativeText(String value)](#setAlternativeText-java.lang.String-) | يرجع أو يضبط النص الوصفي (البديل) لكائن الـ [Shape](../../com.aspose.cells/shape). |
| [setAnchorType(int value)](#setAnchorType-int-) | يضبط نوع العنصر النائب لمرساة الشكل. |
| [setAspectRatioLocked(boolean value)](#setAspectRatioLocked-boolean-) | صحيح يعني أن نسبة أبعاد الشكل مقفلة. |
| [setAutoShapeType(int value)](#setAutoShapeType-int-) | يضبط نوع الشكل التلقائي. |
| [setBottom(int value)](#setBottom-int-) | يمثل عرض الإزاحة العمودية للشكل من صف زاوية أسفله السفلية، بوحدة البكسل. |
| [setCreateId(UUID value)](#setCreateId-java.util.UUID-) | يضبط معرف الإنشاء لهذا الشكل. |
| [setCurrentValue(int value)](#setCurrentValue-int-) | يضبط القيمة الحالية. |
| [setDecorative(boolean value)](#setDecorative-boolean-) | يشير إلى ما إذا كان الكائن زخرفيًا. |
| [setFilled(boolean value)](#setFilled-boolean-) | يشير إلى ما إذا كان تنسيق التعبئة مرئيًا. |
| [setFlippedHorizontally(boolean value)](#setFlippedHorizontally-boolean-) | يضبط ما إذا كان الشكل مقلوبًا أفقيًا. |
| [setFlippedVertically(boolean value)](#setFlippedVertically-boolean-) | يضبط ما إذا كان الشكل مقلوبًا عموديًا. |
| [setFont(Font value)](#setFont-com.aspose.cells.Font-) | يمثل خط الشكل. |
| [setHasLine(boolean value)](#setHasLine-boolean-) | يضبط ظهور حد الخط للشكل. |
| [setHeight(int value)](#setHeight-int-) | يمثل ارتفاع الشكل، بوحدة البكسل. |
| [setHeightCM(double value)](#setHeightCM-double-) | يمثل ارتفاع الشكل، بوحدة السنتيمتر. |
| [setHeightInShape(int value)](#setHeightInShape-int-) | يمثل الإزاحة العمودية للشكل من الحد العلوي للشكل الأب، بوحدة 1/4000 من ارتفاع الشكل الأب. |
| [setHeightInch(double value)](#setHeightInch-double-) | يمثل ارتفاع الشكل، بوحدة البوصة. |
| [setHeightPt(double value)](#setHeightPt-double-) | يمثل ارتفاع الشكل، بوحدة النقاط. |
| [setHeightScale(int value)](#setHeightScale-int-) | يضبط مقياس الارتفاع، بوحدة النسبة المئوية لارتفاع الصورة الأصلية. |
| [setHidden(boolean value)](#setHidden-boolean-) | يشير إلى ما إذا كان الكائن مرئيًا. |
| [setHorizontal(boolean value)](#setHorizontal-boolean-) | يشير إلى ما إذا كان هذا شريط تمرير أفقي. |
| [setHtmlText(String value)](#setHtmlText-java.lang.String-) | يضبط سلسلة HTML التي تحتوي على البيانات وبعض التنسيقات في مربع النص هذا. |
| [setIncrementalChange(int value)](#setIncrementalChange-int-) | يضبط مقدار الزيادة التي يتم تطبيقها على شريط التمرير أو المؤشر عند تمرير سطر واحد. |
| [setInputRange(String value)](#setInputRange-java.lang.String-) | يضبط نطاق ورقة العمل المستخدم لملء مربع الاختيار المحدد. |
| [setInputRange(String formula, boolean isR1C1, boolean isLocal)](#setInputRange-java.lang.String-boolean-boolean-) | يضبط النطاق المستخدم لملء عنصر التحكم. |
| [setLeft(int value)](#setLeft-int-) | يمثل الإزاحة الأفقية للشكل من عموده الأيسر، بوحدة البكسل. |
| [setLeftCM(double value)](#setLeftCM-double-) | يمثل الإزاحة الأفقية للشكل من عموده الأيسر، بوحدة السنتيمتر. |
| [setLeftInShape(int value)](#setLeftInShape-int-) | يمثل الإزاحة الأفقية للشكل من الحد الأيسر للشكل الأب، بوحدة 1/4000 من عرض الشكل الأب. |
| [setLeftInch(double value)](#setLeftInch-double-) | يمثل الإزاحة الأفقية للشكل من عموده الأيسر، بوحدة البوصة. |
| [setLeftToCorner(int value)](#setLeftToCorner-int-) | يضبط الإزاحة الأفقية للشكل من الحد الأيسر لورقة العمل. |
| [setLinkedCell(String value)](#setLinkedCell-java.lang.String-) | يضبط نطاق ورقة العمل المرتبط بقيمة عنصر التحكم. |
| [setLinkedCell(String formula, boolean isR1C1, boolean isLocal)](#setLinkedCell-java.lang.String-boolean-boolean-) | يضبط النطاق المرتبط بقيمة عنصر التحكم. |
| [setLockAspectRatio(boolean value)](#setLockAspectRatio-boolean-) | صحيح يعني أن نسبة أبعاد الشكل مقفلة. |
| [setLocked(boolean value)](#setLocked-boolean-) | صحيح يعني أن الكائن لا يمكن تعديله عندما تكون الورقة محمية. |
| [setLockedProperty(int type, boolean value)](#setLockedProperty-int-boolean-) | ضبط الخاصية المقفلة. |
| [setLowerDeltaX(int value)](#setLowerDeltaX-int-) | يضبط الإزاحة الأفقية للشكل من عمود زاويته السفلية اليمنى. |
| [setLowerDeltaY(int value)](#setLowerDeltaY-int-) | يضبط الإزاحة العمودية للشكل من صف زاويته السفلية اليمنى. |
| [setLowerRightColumn(int value)](#setLowerRightColumn-int-) | يمثل فهرس عمود الزاوية السفلية اليمنى. |
| [setLowerRightRow(int value)](#setLowerRightRow-int-) | يمثل فهرس صف الزاوية السفلية اليمنى. |
| [setMacroName(String value)](#setMacroName-java.lang.String-) | يضبط اسم الماكرو. |
| [setMax(int value)](#setMax-int-) | يضبط القيمة القصوى لنطاق شريط التمرير أو المؤشر. |
| [setMin(int value)](#setMin-int-) | يضبط القيمة الدنيا لنطاق شريط التمرير أو المؤشر. |
| [setName(String value)](#setName-java.lang.String-) | يضبط اسم الشكل. |
| [setPageChange(int value)](#setPageChange-int-) | يضبط تغيير الصفحة. |
| [setPlacement(int value)](#setPlacement-int-) | يمثل الطريقة التي يتم بها إرفاق كائن الرسم بالخلايا تحته. |
| [setPrintable(boolean value)](#setPrintable-boolean-) | يشير إلى ما إذا كان الكائن قابلًا للطباعة. |
| [setRelativeToOriginalPictureSize(boolean value)](#setRelativeToOriginalPictureSize-boolean-) | يشير إلى ما إذا كان الشكل نسبيًا لحجم الصورة الأصلي. |
| [setRight(int value)](#setRight-int-) | يمثل عرض الإزاحة الأفقية للشكل من عمود زاويةه السفلية اليمنى، بوحدة البكسل. |
| [setRotationAngle(double value)](#setRotationAngle-double-) | يضبط دوران الشكل. |
| [setShadow(boolean value)](#setShadow-boolean-) | يشير إلى ما إذا كان الشكل يحتوي على تظليل ثلاثي الأبعاد. |
| [setSoftEdges(double value)](#setSoftEdges-double-) | يضبط نصف قطر الضبابية لتطبيقه على الحواف، بوحدة النقاط. |
| [setText(String value)](#setText-java.lang.String-) | يضبط نص هذا الشكل. |
| [setTextDirection(int value)](#setTextDirection-int-) | يضبط اتجاه تدفق النص لهذا الكائن. |
| [setTextHorizontalAlignment(int value)](#setTextHorizontalAlignment-int-) | يضبط نوع محاذاة النص الأفقية للشكل. |
| [setTextHorizontalOverflow(int value)](#setTextHorizontalOverflow-int-) | يضبط نوع تجاوز النص الأفقي للشكل الذي يحتوي على نص. |
| [setTextOptions(TextOptions value)](#setTextOptions-com.aspose.cells.TextOptions-) | يمثل خيارات النص للشكل. |
| [setTextOrientationType(int value)](#setTextOrientationType-int-) | يضبط نوع توجيه النص للشكل. |
| [setTextShapeType(int value)](#setTextShapeType-int-) | يضبط نوع شكل النص المسبق. |
| [setTextVerticalAlignment(int value)](#setTextVerticalAlignment-int-) | يضبط نوع محاذاة النص العمودية للشكل. |
| [setTextVerticalOverflow(int value)](#setTextVerticalOverflow-int-) | يضبط نوع تجاوز النص العمودي للشكل الذي يحتوي على نص. |
| [setTextWrapped(boolean value)](#setTextWrapped-boolean-) | يضبط نوع التفاف النص للشكل الذي يحتوي على نص. |
| [setTitle(String value)](#setTitle-java.lang.String-) | يحدد العنوان (التسمية) لكائن الشكل الحالي. |
| [setTop(int value)](#setTop-int-) | يمثل الإزاحة العمودية للشكل من صفه العلوي، بوحدة البكسل. |
| [setTopCM(double value)](#setTopCM-double-) | يمثل الإزاحة العمودية للشكل من صفه العلوي، بوحدة السنتيمتر. |
| [setTopInShape(int value)](#setTopInShape-int-) | يمثل الإزاحة العمودية للشكل من الحد العلوي للشكل الأب، بوحدة 1/4000 من ارتفاع الشكل الأب. |
| [setTopInch(double value)](#setTopInch-double-) | يمثل الإزاحة العمودية للشكل من صفه العلوي، بوحدة البوصة. |
| [setTopToCorner(int value)](#setTopToCorner-int-) | يضبط الإزاحة العمودية للشكل من الحد العلوي لورقة العمل، بوحدة البكسل. |
| [setUpperDeltaX(int value)](#setUpperDeltaX-int-) | يضبط الإزاحة الأفقية للشكل من عمود زاويته العلوية اليسرى. |
| [setUpperDeltaY(int value)](#setUpperDeltaY-int-) | يضبط الإزاحة العمودية للشكل من صف زاويته العلوية اليسرى. |
| [setUpperLeftColumn(int value)](#setUpperLeftColumn-int-) | يمثل فهرس عمود الزاوية العلوية اليسرى. |
| [setUpperLeftRow(int value)](#setUpperLeftRow-int-) | يمثل فهرس الصف العلوي. |
| [setWidth(int value)](#setWidth-int-) | يمثل عرض الشكل، بوحدة البكسل. |
| [setWidthCM(double value)](#setWidthCM-double-) | يمثل عرض الشكل، بوحدة السنتيمتر. |
| [setWidthInShape(int value)](#setWidthInShape-int-) | يمثل عرض الشكل، بوحدة 1/4000 من الشكل الأصل. |
| [setWidthInch(double value)](#setWidthInch-double-) | يمثل عرض الشكل، بوحدة البوصة. |
| [setWidthPt(double value)](#setWidthPt-double-) | يمثل عرض الشكل، بوحدة النقطة. |
| [setWidthScale(int value)](#setWidthScale-int-) | يضبط مقياس العرض، بوحدة النسبة المئوية لعرض الصورة الأصلي. |
| [setX(int value)](#setX-int-) | يضبط الإزاحة الأفقية للشكل من الحد الأيسر لورقة العمل، بوحدة البكسل. |
| [setY(int value)](#setY-int-) | يضبط الإزاحة العمودية للشكل من الحد العلوي لورقة العمل، بوحدة البكسل. |
| [setZOrderPosition(int value)](#setZOrderPosition-int-) | يعيد موضع الشكل في ترتيب z. |
| [toFrontOrBack(int orders)](#toFrontOrBack-int-) | ينقل الشكل إلى المقدمة أو يرسله إلى الخلف. |
| [toImage(OutputStream stream, ImageFormat imageFormat)](#toImage-java.io.OutputStream-com.aspose.cells.ImageFormat-) | ينشئ صورة الشكل ويحفظها إلى تدفق بالصيغة المحددة. |
| [toImage(OutputStream stream, ImageOrPrintOptions options)](#toImage-java.io.OutputStream-com.aspose.cells.ImageOrPrintOptions-) | يحفظ الشكل إلى تدفق. |
| [toImage(String imageFile, ImageOrPrintOptions options)](#toImage-java.lang.String-com.aspose.cells.ImageOrPrintOptions-) | يحفظ الشكل إلى ملف. |
| [toString()](#toString--) |  |
| [updateSelectedValue()](#updateSelectedValue--) | تحديث القيمة المحددة بقيمة الخلية المرتبطة. |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### addHyperlink(String address) {#addHyperlink-java.lang.String-}
```
public Hyperlink addHyperlink(String address)
```


يضيف ارتباطًا تشعبيًا إلى الشكل.

**Example**

```
         Hyperlink hyperlink = shape.addHyperlink("https://www.aspose.com/");
```

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| العنوان | java.lang.String | عنوان الارتباط التشعبي. |

**Returns:**
[Hyperlink](../../com.aspose.cells/hyperlink) - Returns the new hyperlink object.
### alignTopRightCorner(int topRow, int rightColumn) {#alignTopRightCorner-int-int-}
```
public void alignTopRightCorner(int topRow, int rightColumn)
```


ينقل الصورة إلى الزاوية العليا اليمنى.

**Example**

```
         shape.alignTopRightCorner(2, 5);
```

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| topRow | int | فهرس الصف. |
| rightColumn | int | فهرس العمود. |

### calculateTextSize() {#calculateTextSize--}
```
public int[] calculateTextSize()
```


إعادة حساب منطقة النص

**Example**

```
         //The size of the text area is:w=size[0],h=size[1]
         int[] size = shape.calculateTextSize();
```

**Returns:**
int[] - حجم النص في مصفوفة (العرض والارتفاع).
### characters(int startIndex, int length) {#characters-int-int-}
```
public FontSetting characters(int startIndex, int length)
```


يرجع كائن Characters يمثل نطاقًا من الأحرف داخل النص.

**Remarks**

هذه الطريقة تعمل فقط على الشكل الذي يحتوي على عنوان.

**Example**

```
         FontSetting fontSetting = shape.characters(0, 4);
```

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| startIndex | int | فهرس بداية الحرف. |
| length | int | عدد الأحرف. |

**Returns:**
[FontSetting](../../com.aspose.cells/fontsetting) - Characters object.
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
### fitToTextSize() {#fitToTextSize--}
```
public void fitToTextSize()
```


إعادة حساب منطقة نصية مناسبة لعرض كل محتوى النص.

**Example**

```
         if (shape.getName().startsWith("Your traget"))
         {
             shape.fitToTextSize();
         }
```

### formatCharacters(int startIndex, int length, Font font, StyleFlag flag) {#formatCharacters-int-int-com.aspose.cells.Font-com.aspose.cells.StyleFlag-}
```
public void formatCharacters(int startIndex, int length, Font font, StyleFlag flag)
```


يقوم بتنسيق بعض الأحرف باستخدام إعداد الخط.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| startIndex | int | فهرس البداية. |
| length | int | الطول. |
| font | [Font](../../com.aspose.cells/font) | إعداد الخط. |
| flag | [StyleFlag](../../com.aspose.cells/styleflag) | علامة إعداد الخط. |

### getActiveXControl() {#getActiveXControl--}
```
public ActiveXControl getActiveXControl()
```


يحصل على عنصر التحكم ActiveX.

**Example**

```
         if(shape.getActiveXControl() != null)
         {
             CheckBoxActiveXControl checkBox1 = (CheckBoxActiveXControl)shape.getActiveXControl();
             //The font name of CheckBox
             String fontName = checkBox1.getFont().getName();
         }
```

**Returns:**
[ActiveXControl](../../com.aspose.cells/activexcontrol)
### getActualBox() {#getActualBox--}
```
public float[] getActualBox()
```


احصل على الموضع والحجم الفعليين للشكل (بعد تطبيق الدوران أو الانعكاس، إلخ).

**Remarks**

ملاحظة: الواجهة ليست وظيفية بالكامل، خاصةً أن معلومات الموقع غير صحيحة. يُنصح بعدم استخدام هذه الواجهة حتى يكتمل الوظيفة.

**Example**

```
         float[] box = shape.getActualBox();
         System.out.println("x = " + box[0]);
         System.out.println("y = " + box[1]);
         System.out.println("w = " + box[2]);
         System.out.println("h = " + box[3]);
```

**Returns:**
float[] - يُعيد الموضع والحجم بالترتيب x, y, w, h
### getActualLowerRightRow() {#getActualLowerRightRow--}
```
public int getActualLowerRightRow()
```


احصل على الصف السفلي الفعلي.

**Example**

```
         int rRow = shape.getActualLowerRightRow();
```

**Returns:**
int
### getAlternativeText() {#getAlternativeText--}
```
public String getAlternativeText()
```


يرجع أو يضبط النص الوصفي (البديل) لكائن الـ [Shape](../../com.aspose.cells/shape).

**Example**

```
         shape.setAlternativeText("a rectangle");
```

**Returns:**
java.lang.String
### getAnchorType() {#getAnchorType--}
```
public int getAnchorType()
```


يحصل على نوع العنصر النائب لمرساة الشكل.

انظر [ShapeAnchorType](../../com.aspose.cells/shapeanchortype).

**Example**

```
         if (shape.getAnchorType() == ShapeAnchorType.ONE_CELL_ANCHOR)
             shape.setAnchorType(ShapeAnchorType.TWO_CELL_ANCHOR);
```

**Returns:**
int
### getAutoShapeType() {#getAutoShapeType--}
```
public int getAutoShapeType()
```


يحصل على نوع الشكل التلقائي.

انظر [AutoShapeType](../../com.aspose.cells/autoshapetype).

**Example**

```
         if (shape.getAutoShapeType() == com.aspose.cells.AutoShapeType.UNKNOWN)
             shape.setAutoShapeType(com.aspose.cells.AutoShapeType.RECTANGLE);
```

**Returns:**
int
### getBottom() {#getBottom--}
```
public int getBottom()
```


يمثل عرض الإزاحة العمودية للشكل من صف زاوية أسفله السفلية، بوحدة البكسل.

**Example**

```
         if (shape.getBottom() == 3)
             shape.setBottom(1);
```

**Returns:**
int
### getCharacters() {#getCharacters--}
```
public ArrayList getCharacters()
```


يرجع جميع كائنات Characters التي تمثل نطاقًا من الأحرف داخل النص.

**Remarks**

ملاحظة: هذه الطريقة أصبحت مهجورة الآن. بدلاً من ذلك، يرجى استخدام طريقة Shape.GetRichFormattings(). سيتم إزالة هذه الطريقة بعد 12 شهرًا منذ نوفمبر 2023. تعتذر Aspose عن أي إزعاج قد تكون قد تعرضت له.

**Example**

```
         FontSetting fontSetting = shape.characters(0, 4);
```

**Returns:**
java.util.ArrayList - جميع كائنات Characters
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getConnectionPoints() {#getConnectionPoints--}
```
public float[][] getConnectionPoints()
```


احصل على نقاط الاتصال

**Example**

```
         float[][] points = shape.getConnectionPoints();
```

**Returns:**
float[][] - أزواج [X,Y] لنقطة الاتصال. كل عنصر هو مصفوفة float[2]، حيث يمثل [0] x و[1] y.
### getControlData() {#getControlData--}
```
public byte[] getControlData()
```


يحصل على بيانات التحكم.

**Example**

```
         if(shape.getControlData() == null)
             System.out.println("No data.");
```

**Returns:**
byte[]
### getCreateId() {#getCreateId--}
```
public UUID getCreateId()
```


يحصل على معرف الإنشاء لهذا الشكل.

**Example**

```
         System.out.println(shape.getCreateId());
         java.util.UUID g = java.util.UUID.randomUUID();
         shape.setCreateId(g);
         System.out.println(shape.getCreateId());
```

**Returns:**
java.util.UUID
### getCurrentValue() {#getCurrentValue--}
```
public int getCurrentValue()
```


يحصل على القيمة الحالية.

**Returns:**
int
### getFill() {#getFill--}
```
public FillFormat getFill()
```


يرجع كائن [getFillFormat()](../../com.aspose.cells/shape\#getFillFormat--) الذي يحتوي على خصائص تنسيق التعبئة للشكل المحدد.

**Example**

```
         FillFormat fillFmt = shape.getFill();
```

**Returns:**
[FillFormat](../../com.aspose.cells/fillformat)
### getFillFormat() {#getFillFormat--}
```
public MsoFillFormat getFillFormat()
```


يرجع كائن MsoFillFormat الذي يحتوي على خصائص تنسيق التعبئة للشكل المحدد.

**Remarks**

ملاحظة: هذا العضو أصبح مهجورًا الآن. بدلاً من ذلك، يرجى استخدام خاصية Shape.Fill. سيتم إزالة هذه الخاصية بعد 12 شهرًا منذ يوليو 2016. تعتذر Aspose عن أي إزعاج قد تكون قد تعرضت له.

**Returns:**
[MsoFillFormat](../../com.aspose.cells/msofillformat)
### getFont() {#getFont--}
```
public Font getFont()
```


يمثل خط الشكل.

**Example**

```
         Font font = shape.getFont();
         font.setName("Arial");
         font.setSize(12);
         font.setColor(Color.getRed());
```

**Returns:**
[Font](../../com.aspose.cells/font)
### getFormatPicture() {#getFormatPicture--}
```
public MsoFormatPicture getFormatPicture()
```


يحصل على خيارات تنسيق الصورة.

**Example**

```
         MsoFormatPicture msoFormatPicture = shape.getFormatPicture();
```

**Returns:**
[MsoFormatPicture](../../com.aspose.cells/msoformatpicture)
### getGeometry() {#getGeometry--}
```
public Geometry getGeometry()
```


يحصل على الهندسة

**Example**

```
         if (shape.getGeometry() != null &&shape.getGeometry().getShapeAdjustValues().getCount() == 0)
             System.out.println("No geometry path.");
```

**Returns:**
[Geometry](../../com.aspose.cells/geometry)
### getGlow() {#getGlow--}
```
public GlowEffect getGlow()
```


يمثل كائن [GlowEffect](../../com.aspose.cells/gloweffect) الذي يحدد تأثير التوهج لعنصر المخطط أو الشكل.

**Example**

```
         GlowEffect glowEffect = shape.getGlow();
```

**Returns:**
[GlowEffect](../../com.aspose.cells/gloweffect)
### getGroup() {#getGroup--}
```
public GroupShape getGroup()
```


يحصل على الشكل الجماعي الذي يحتوي على هذا الشكل.

**Example**

```
         GroupShape groupShape = shape.getGroup();
```

**Returns:**
[GroupShape](../../com.aspose.cells/groupshape)
### getHeight() {#getHeight--}
```
public int getHeight()
```


يمثل ارتفاع الشكل، بوحدة البكسل.

**Example**

```
         if (shape.getHeight() == 3)
             shape.setHeight(1);
```

**Returns:**
int
### getHeightCM() {#getHeightCM--}
```
public double getHeightCM()
```


يمثل ارتفاع الشكل، بوحدة السنتيمتر.

**Example**

```
         if (shape.getHeightCM() == 3)
             shape.setHeightCM(1);
```

**Returns:**
double
### getHeightInShape() {#getHeightInShape--}
```
public int getHeightInShape()
```


يمثل الإزاحة العمودية للشكل من الحد العلوي للشكل الأب، بوحدة 1/4000 من ارتفاع الشكل الأب.

**Remarks**

يطبق فقط عندما يكون هذا الشكل ضمن مجموعة أو مخطط.

**Example**

```
         if (shape.isInGroup() &&shape.getHeightInShape() == 4000)
             shape.setHeightInShape(2000);
```

**Returns:**
int
### getHeightInch() {#getHeightInch--}
```
public double getHeightInch()
```


يمثل ارتفاع الشكل، بوحدة البوصة.

**Example**

```
         if (shape.getHeightInch() == 3)
             shape.setHeightInch(1);
```

**Returns:**
double
### getHeightPt() {#getHeightPt--}
```
public double getHeightPt()
```


يمثل ارتفاع الشكل، بوحدة النقاط.

**Example**

```
         if (shape.getHeightPt() == 3)
             shape.setHeightPt(1);
```

**Returns:**
double
### getHeightScale() {#getHeightScale--}
```
public int getHeightScale()
```


يحصل على مقياس الارتفاع، بوحدة النسبة المئوية لارتفاع الصورة الأصلي. إذا لم يكن الشكل صورة، فإن خاصية HeightScale تُعيد فقط 100؛

**Example**

```
         if (shape.getHeightScale() == 3)
             shape.setHeightScale(1);
```

**Returns:**
int
### getHtmlText() {#getHtmlText--}
```
public String getHtmlText()
```


يحصل على سلسلة HTML التي تحتوي على البيانات وبعض التنسيقات في هذا مربع النص.

**Example**

```
         String html = shape.getHtmlText();
         if(html == null || "".equals(html))
         {
             shape.setHtmlText("<Font Style='FONT-FAMILY: Calibri;FONT-SIZE: 11pt;COLOR: #0000ff;TEXT-ALIGN: left;'>This is a <b>test</b>.</Font>");
         }
```

**Returns:**
java.lang.String
### getHyperlink() {#getHyperlink--}
```
public Hyperlink getHyperlink()
```


يحصل على الارتباط التشعبي للشكل.

**Example**

```
         Hyperlink hyperlink = shape.getHyperlink();
```

**Returns:**
[Hyperlink](../../com.aspose.cells/hyperlink)
### getId() {#getId--}
```
public int getId()
```


يحصل على معرف هذا الشكل.

**Example**

```
         int id = shape.getId();
```

**Returns:**
int
### getIncrementalChange() {#getIncrementalChange--}
```
public int getIncrementalChange()
```


يحصل على مقدار الزيادة التي يتم تطبيقها على شريط التمرير أو المؤشر عند تمرير سطر واحد.

**Returns:**
int
### getInputRange() {#getInputRange--}
```
public String getInputRange()
```


يحصل على نطاق ورقة العمل المستخدم لملء صندوق القائمة المحدد.

**Example**

```
         if (shape.getInputRange().equals("$B$6:$B10"))
             shape.setInputRange("$A$1:$A$5");
```

**Returns:**
java.lang.String
### getInputRange(boolean isR1C1, boolean isLocal) {#getInputRange-boolean-boolean-}
```
public String getInputRange(boolean isR1C1, boolean isLocal)
```


يحصل على النطاق المستخدم لملء التحكم.

**Example**

```
         String range = shape.getInputRange(false, true);
         //If successful, a value like "$A$1:$A$3" will be returned
```

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| isR1C1 | boolean | ما إذا كانت الصيغة تحتاج إلى تنسيق كـ R1C1. |
| isLocal | boolean | ما إذا كانت الصيغة تحتاج إلى تنسيق حسب الإعدادات الإقليمية. |

**Returns:**
java.lang.String - النطاق المستخدم لملء التحكم.
### getLeft() {#getLeft--}
```
public int getLeft()
```


يمثل الإزاحة الأفقية للشكل من عموده الأيسر، بوحدة البكسل.

**Example**

```
         if (shape.getLeft() == 3)
             shape.setLeft(1);
```

**Returns:**
int
### getLeftCM() {#getLeftCM--}
```
public double getLeftCM()
```


يمثل الإزاحة الأفقية للشكل من عموده الأيسر، بوحدة السنتيمتر.

**Example**

```
         if (shape.getLeftCM() == 3)
             shape.setLeftCM(1);
```

**Returns:**
double
### getLeftInShape() {#getLeftInShape--}
```
public int getLeftInShape()
```


يمثل الإزاحة الأفقية للشكل من الحد الأيسر للشكل الأب، بوحدة 1/4000 من عرض الشكل الأب.

**Remarks**

يطبق فقط عندما يكون هذا الشكل ضمن مجموعة أو مخطط.

**Example**

```
         if (shape.isInGroup() &&shape.getLeftInShape() == 2000)
             shape.setLeftInShape(4000);
```

**Returns:**
int
### getLeftInch() {#getLeftInch--}
```
public double getLeftInch()
```


يمثل الإزاحة الأفقية للشكل من عموده الأيسر، بوحدة البوصة.

**Example**

```
         if (shape.getLeftInch() == 3)
             shape.setLeftInch(1);
```

**Returns:**
double
### getLeftToCorner() {#getLeftToCorner--}
```
public int getLeftToCorner()
```


يحصل على الإزاحة الأفقية للشكل من الحد الأيسر لورقة العمل.

**Example**

```
         if (shape.getLeftToCorner() == 3)
             shape.setLeftToCorner(1);
```

**Returns:**
int
### getLine() {#getLine--}
```
public LineFormat getLine()
```


يحصل على نمط الخط

**Example**

```
         LineFormat lineFmt = shape.getLine();
```

**Returns:**
[LineFormat](../../com.aspose.cells/lineformat)
### getLineFormat() {#getLineFormat--}
```
public MsoLineFormat getLineFormat()
```


يرجع كائن MsoLineFormat يحتوي على خصائص تنسيق الخط للشكل المحدد.

**Remarks**

ملاحظة: هذا العضو أصبح الآن مهملًا. بدلاً من ذلك، يرجى استخدام خاصية Shape.Line. سيتم إزالة هذه الخاصية بعد 12 شهرًا منذ يوليو 2016. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

**Returns:**
[MsoLineFormat](../../com.aspose.cells/msolineformat)
### getLinkedCell() {#getLinkedCell--}
```
public String getLinkedCell()
```


يحصل على نطاق ورقة العمل المرتبط بقيمة التحكم.

**Example**

```
         if (shape.getLinkedCell().equals("$B$6"))
         {
             shape.setLinkedCell("A1");
         }
         shape.updateSelectedValue();
```

**Returns:**
java.lang.String
### getLinkedCell(boolean isR1C1, boolean isLocal) {#getLinkedCell-boolean-boolean-}
```
public String getLinkedCell(boolean isR1C1, boolean isLocal)
```


يحصل على النطاق المرتبط بقيمة التحكم.

**Example**

```
         //You may get results like '$A$1'
         String link = shape.getLinkedCell(false, false);
```

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| isR1C1 | boolean | ما إذا كانت الصيغة تحتاج إلى تنسيق كـ R1C1. |
| isLocal | boolean | ما إذا كانت الصيغة تحتاج إلى تنسيق حسب الإعدادات الإقليمية. |

**Returns:**
java.lang.String - النطاق المرتبط بقيمة التحكم.
### getLockedProperty(int type) {#getLockedProperty-int-}
```
public boolean getLockedProperty(int type)
```


يحصل على قيمة الخاصية المقفلة.

**Example**

```
         int noAdjustHandles = 0;
         if (shape.getLockedProperty(ShapeLockType.ADJUST_HANDLES))
             noAdjustHandles = 1;
```

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| type | int | [ShapeLockType](../../com.aspose.cells/shapelocktype). نوع الخاصية المقفلة للشكل. |

**Returns:**
boolean - يُعيد قيمة الخاصية المقفلة.
### getLowerDeltaX() {#getLowerDeltaX--}
```
public int getLowerDeltaX()
```


يحصل على الإزاحة الأفقية للشكل من عمود زاويةه السفلية اليمنى.

**Remarks**

نطاق القيمة هو من 0 إلى 1024.

**Example**

```
         if (shape.getLowerDeltaX() == 3)
             shape.setLowerDeltaX(1);
```

**Returns:**
int
### getLowerDeltaY() {#getLowerDeltaY--}
```
public int getLowerDeltaY()
```


يحصل على الإزاحة العمودية للشكل من صف زاويةه السفلية اليمنى.

**Remarks**

نطاق القيمة هو من 0 إلى 256.

**Example**

```
         if (shape.getLowerDeltaY() == 3)
             shape.setLowerDeltaY(1);
```

**Returns:**
int
### getLowerRightColumn() {#getLowerRightColumn--}
```
public int getLowerRightColumn()
```


يمثل فهرس عمود الزاوية السفلية اليمنى.

**Example**

```
         if (shape.getLowerRightColumn() == 3)
             shape.setLowerRightColumn(1);
```

**Returns:**
int
### getLowerRightRow() {#getLowerRightRow--}
```
public int getLowerRightRow()
```


يمثل فهرس صف الزاوية السفلية اليمنى.

**Example**

```
         if (shape.getLowerRightRow() == 3)
             shape.setLowerRightRow(1);
```

**Returns:**
int
### getMacroName() {#getMacroName--}
```
public String getMacroName()
```


يحصل على اسم الماكرو.

**Example**

```
         //Sets the name of macro.
         shape.setMacroName("DoWork()");
```

**Returns:**
java.lang.String
### getMax() {#getMax--}
```
public int getMax()
```


يحصل على القيمة القصوى لنطاق شريط التمرير أو المؤشر.

**Returns:**
int
### getMin() {#getMin--}
```
public int getMin()
```


يحصل على القيمة الدنيا لنطاق شريط التمرير أو المؤشر.

**Returns:**
int
### getMsoDrawingType() {#getMsoDrawingType--}
```
public int getMsoDrawingType()
```


يحصل على نوع الرسم.

انظر [MsoDrawingType](../../com.aspose.cells/msodrawingtype).

**Example**

```
         /*Aspose.Cells.Drawing.MsoDrawingType*/int msoDrawingType = shape.getMsoDrawingType();
```

**Returns:**
int
### getName() {#getName--}
```
public String getName()
```


يحصل على اسم الشكل.

**Example**

```
         shape.setName("shape1");
```

**Returns:**
java.lang.String
### getPageChange() {#getPageChange--}
```
public int getPageChange()
```


يحصل على تغيير الصفحة.

**Returns:**
int
### getPaths() {#getPaths--}
```
public ShapePathCollection getPaths()
```


يحصل على مسارات الشكل الهندسي المخصص.

**Example**

```
         //Returns non-null if there is a path to the custom geometry
         if(shape.getPaths() == null)
             System.out.println("No custom geometry path.");
```

**Returns:**
[ShapePathCollection](../../com.aspose.cells/shapepathcollection)
### getPlacement() {#getPlacement--}
```
public int getPlacement()
```


يمثل الطريقة التي يتم بها إرفاق كائن الرسم بالخلايا تحته. تتحكم الخاصية في وضع الكائن على ورقة العمل.

انظر [PlacementType](../../com.aspose.cells/placementtype).

**Example**

```
         if (shape.getPlacement() == PlacementType.MOVE)
             shape.setPlacement(PlacementType.MOVE_AND_SIZE);
```

**Returns:**
int
### getReflection() {#getReflection--}
```
public ReflectionEffect getReflection()
```


يمثل كائن [ReflectionEffect](../../com.aspose.cells/reflectioneffect) الذي يحدد تأثير الانعكاس لعنصر المخطط أو الشكل.

**Example**

```
         ReflectionEffect reflectionEffect = shape.getReflection();
```

**Returns:**
[ReflectionEffect](../../com.aspose.cells/reflectioneffect)
### getRelativeToOriginalPictureSize() {#getRelativeToOriginalPictureSize--}
```
public boolean getRelativeToOriginalPictureSize()
```


يشير إلى ما إذا كان الشكل نسبيًا لحجم الصورة الأصلي.

**Example**

```
         if(shape.getRelativeToOriginalPictureSize())
             shape.setRelativeToOriginalPictureSize(false);
```

**Returns:**
boolean
### getResultOfSmartArt() {#getResultOfSmartArt--}
```
public GroupShape getResultOfSmartArt()
```


تحويل Smart Art إلى أشكال مجمعة.

**Example**

```
         if(shape.isSmartArt())
         {
             GroupShape groupShape = shape.getResultOfSmartArt();
         }
```

**Returns:**
[GroupShape](../../com.aspose.cells/groupshape)
### getRichFormattings() {#getRichFormattings--}
```
public FontSetting[] getRichFormattings()
```


يرجع جميع كائنات Characters التي تمثل نطاقًا من الأحرف داخل النص.

**Example**

```
         FontSetting[] list = shape.getRichFormattings();
```

**Returns:**
com.aspose.cells.FontSetting[] - جميع كائنات الأحرف
### getRight() {#getRight--}
```
public int getRight()
```


يمثل عرض الإزاحة الأفقية للشكل من عمود زاويةه السفلية اليمنى، بوحدة البكسل.

**Example**

```
         if (shape.getRight() == 3)
             shape.setRight(1);
```

**Returns:**
int
### getRotationAngle() {#getRotationAngle--}
```
public double getRotationAngle()
```


يحصل على دوران الشكل.

**Example**

```
         //Gets rotation angle of the shape.
         double angle = shape.getRotationAngle() ;
 
         //Gets rotation angle of the shape.
          shape.setRotationAngle(60);
```

**Returns:**
double
### getShadow() {#getShadow--}
```
public boolean getShadow()
```


يشير إلى ما إذا كان الشكل يحتوي على تظليل ثلاثي الأبعاد.

**Returns:**
boolean
### getShadowEffect() {#getShadowEffect--}
```
public ShadowEffect getShadowEffect()
```


يمثل كائن [ShadowEffect](../../com.aspose.cells/shadoweffect) الذي يحدد تأثير الظل لعنصر المخطط أو الشكل.

**Example**

```
         ShadowEffect shadowEffect = shape.getShadowEffect();
```

**Returns:**
[ShadowEffect](../../com.aspose.cells/shadoweffect)
### getSoftEdges() {#getSoftEdges--}
```
public double getSoftEdges()
```


يحصل على نصف قطر الضبابية لتطبيقه على الحواف، بوحدة النقاط.

**Example**

```
         shape.setSoftEdges(0.5d);
```

**Returns:**
double
### getSpid() {#getSpid--}
```
public String getSpid()
```


يحدد معرف سلسلة اختياري يمكن للتطبيق استخدامه لتحديد الشكل المحدد.

**Example**

```
         String spid = shape.getSpid();
```

**Returns:**
java.lang.String
### getSpt() {#getSpt--}
```
public int getSpt()
```


يحدد رقمًا اختياريًا يمكن للتطبيق استخدامه لربط الشكل المحدد بنوع شكل معرف.

**Example**

```
         int spt = shape.getSpt();
```

**Returns:**
int
### getText() {#getText--}
```
public String getText()
```


يحصل على نص هذا الشكل.

**Example**

```
         if(shape.getText() == null)
             shape.setText("This is a test.");
```

**Returns:**
java.lang.String
### getTextBody() {#getTextBody--}
```
public FontSettingCollection getTextBody()
```


يحصل على إعداد نص الشكل.

**Example**

```
         FontSettingCollection fontSettingCollection = shape.getTextBody();
         fontSettingCollection.setText("This is a test.");
```

**Returns:**
[FontSettingCollection](../../com.aspose.cells/fontsettingcollection)
### getTextBoxOptions() {#getTextBoxOptions--}
```
public TextBoxOptions getTextBoxOptions()
```


يحصل على معلومات النص في الشكل

**Example**

```
         TextBoxOptions textBoxOpt = shape.getTextBoxOptions();
         textBoxOpt.setShapeTextVerticalAlignment(ShapeTextVerticalAlignmentType.LEFT);
         textBoxOpt.setTopMarginPt(0.2d);
         textBoxOpt.setLeftMarginPt(0.2d);
         textBoxOpt.setRightMarginPt(0.2d);
         textBoxOpt.setBottomMarginPt(0.2d);
```

**Returns:**
[TextBoxOptions](../../com.aspose.cells/textboxoptions)
### getTextDirection() {#getTextDirection--}
```
public int getTextDirection()
```


يحصل على اتجاه تدفق النص لهذا الكائن.

انظر [TextDirectionType](../../com.aspose.cells/textdirectiontype).

**Example**

```
         if (shape.getTextDirection() == com.aspose.cells.TextDirectionType.CONTEXT)
             shape.setTextDirection(com.aspose.cells.TextDirectionType.LEFT_TO_RIGHT);
```

**Returns:**
int
### getTextEffect() {#getTextEffect--}
```
public TextEffectFormat getTextEffect()
```


يُعيد كائن TextEffectFormat الذي يحتوي على خصائص تنسيق تأثير النص للشكل المحدد. ينطبق على كائنات Shape التي تمثل WordArt.

**Example**

```
         if(shape.isWordArt())
         {
             TextEffectFormat textEffectFormat = shape.getTextEffect();
         }
```

**Returns:**
[TextEffectFormat](../../com.aspose.cells/texteffectformat)
### getTextHorizontalAlignment() {#getTextHorizontalAlignment--}
```
public int getTextHorizontalAlignment()
```


يحصل على نوع محاذاة النص الأفقية للشكل.

انظر [TextAlignmentType](../../com.aspose.cells/textalignmenttype).

**Example**

```
         if (shape.getTextHorizontalAlignment() == com.aspose.cells.TextAlignmentType.BOTTOM)
             shape.setTextHorizontalAlignment(com.aspose.cells.TextAlignmentType.CENTER);
```

**Returns:**
int
### getTextHorizontalOverflow() {#getTextHorizontalOverflow--}
```
public int getTextHorizontalOverflow()
```


يحصل على نوع تجاوز النص الأفقي للشكل الذي يحتوي على النص.

انظر [TextOverflowType](../../com.aspose.cells/textoverflowtype).

**Example**

```
         if (shape.getTextHorizontalOverflow() == com.aspose.cells.TextOverflowType.CLIP)
             shape.setTextHorizontalOverflow(com.aspose.cells.TextOverflowType.OVERFLOW);
```

**Returns:**
int
### getTextOptions() {#getTextOptions--}
```
public TextOptions getTextOptions()
```


يمثل خيارات النص للشكل.

**Example**

```
         TextOptions opt = shape.getTextOptions();
         opt.setColor(Color.getBlue());
         opt.setSize(8);
```

**Returns:**
[TextOptions](../../com.aspose.cells/textoptions)
### getTextOrientationType() {#getTextOrientationType--}
```
public int getTextOrientationType()
```


يحصل على نوع توجيه النص للشكل.

انظر [TextOrientationType](../../com.aspose.cells/textorientationtype).

**Example**

```
         if (shape.getTextOrientationType() == com.aspose.cells.TextOrientationType.NO_ROTATION)
             shape.setTextOrientationType(com.aspose.cells.TextOrientationType.TOP_TO_BOTTOM);
```

**Returns:**
int
### getTextShapeType() {#getTextShapeType--}
```
public int getTextShapeType()
```


يحصل على نوع شكل النص المسبق.

انظر [AutoShapeType](../../com.aspose.cells/autoshapetype).

**Example**

```
         if (shape.getTextShapeType() == com.aspose.cells.AutoShapeType.UNKNOWN)
             shape.setTextShapeType(com.aspose.cells.AutoShapeType.RECTANGLE);
```

**Returns:**
int
### getTextVerticalAlignment() {#getTextVerticalAlignment--}
```
public int getTextVerticalAlignment()
```


يحصل على نوع محاذاة النص العمودية للشكل.

انظر [TextAlignmentType](../../com.aspose.cells/textalignmenttype).

**Example**

```
         if (shape.getTextVerticalAlignment() == com.aspose.cells.TextAlignmentType.BOTTOM)
             shape.setTextVerticalAlignment(com.aspose.cells.TextAlignmentType.CENTER);
```

**Returns:**
int
### getTextVerticalOverflow() {#getTextVerticalOverflow--}
```
public int getTextVerticalOverflow()
```


يحصل على نوع تجاوز النص العمودي للشكل الذي يحتوي على النص.

انظر [TextOverflowType](../../com.aspose.cells/textoverflowtype).

**Example**

```
         if (shape.getTextVerticalOverflow() == com.aspose.cells.TextOverflowType.CLIP)
             shape.setTextVerticalOverflow(com.aspose.cells.TextOverflowType.OVERFLOW);
```

**Returns:**
int
### getThreeDFormat() {#getThreeDFormat--}
```
public ThreeDFormat getThreeDFormat()
```


يحصل على تنسيق ثلاثي الأبعاد للشكل.

**Example**

```
         ThreeDFormat threeDFormat = shape.getThreeDFormat();
```

**Returns:**
[ThreeDFormat](../../com.aspose.cells/threedformat)
### getTitle() {#getTitle--}
```
public String getTitle()
```


يحدد العنوان (التسمية) لكائن الشكل الحالي.

**Example**

```
         shape.setTitle("title1");
```

**Returns:**
java.lang.String
### getTop() {#getTop--}
```
public int getTop()
```


يمثل الإزاحة العمودية للشكل من صفه العلوي، بوحدة البكسل.

**Remarks**

إذا كان الشكل داخل المخطط، يمثل الإزاحة العمودية للشكل من حدّه العلوي.

**Example**

```
         if (shape.getTop() == 3)
             shape.setTop(1);
```

**Returns:**
int
### getTopCM() {#getTopCM--}
```
public double getTopCM()
```


يمثل الإزاحة العمودية للشكل من صفه العلوي، بوحدة السنتيمتر.

**Example**

```
         if (shape.getTopCM() == 3)
             shape.setTopCM(1);
```

**Returns:**
double
### getTopInShape() {#getTopInShape--}
```
public int getTopInShape()
```


يمثل الإزاحة العمودية للشكل من الحد العلوي للشكل الأب، بوحدة 1/4000 من ارتفاع الشكل الأب.

**Remarks**

يطبق فقط عندما يكون هذا الشكل ضمن مجموعة أو مخطط.

**Example**

```
         if (shape.isInGroup() &&shape.getTopInShape() == 8000)
             shape.setTopInShape(4000);
```

**Returns:**
int
### getTopInch() {#getTopInch--}
```
public double getTopInch()
```


يمثل الإزاحة العمودية للشكل من صفه العلوي، بوحدة البوصة.

**Example**

```
         if (shape.getTopInch() == 3)
             shape.setTopInch(1);
```

**Returns:**
double
### getTopToCorner() {#getTopToCorner--}
```
public int getTopToCorner()
```


يحصل على الإزاحة العمودية للشكل من الحد العلوي لورقة العمل، بوحدة البكسل.

**Example**

```
         if (shape.getTopToCorner() == 3)
             shape.setTopToCorner(1);
```

**Returns:**
int
### getType() {#getType--}
```
public int getType()
```


يحصل على نوع الشكل التلقائي.

انظر [AutoShapeType](../../com.aspose.cells/autoshapetype).

**Example**

```
         /*Aspose.Cells.Drawing.AutoShapeType*/int autoShapeType = shape.getType();
```

**Returns:**
int
### getUpperDeltaX() {#getUpperDeltaX--}
```
public int getUpperDeltaX()
```


يحصل على الإزاحة الأفقية للشكل من عمود الزاوية العلوية اليسرى.

**Remarks**

نطاق القيمة هو من 0 إلى 1024.

**Example**

```
         if (shape.getUpperDeltaX() == 3)
             shape.setUpperDeltaX(1);
```

**Returns:**
int
### getUpperDeltaY() {#getUpperDeltaY--}
```
public int getUpperDeltaY()
```


يحصل على الإزاحة العمودية للشكل من صف الزاوية العلوية اليسرى.

**Remarks**

نطاق القيمة هو من 0 إلى 256.

**Example**

```
         if (shape.getUpperDeltaY() == 3)
             shape.setUpperDeltaY(1);
```

**Returns:**
int
### getUpperLeftColumn() {#getUpperLeftColumn--}
```
public int getUpperLeftColumn()
```


يمثل فهرس عمود الزاوية العلوية اليسرى.

**Example**

```
         if (shape.getUpperLeftColumn() == 3)
             shape.setUpperLeftColumn(1);
```

**Returns:**
int
### getUpperLeftRow() {#getUpperLeftRow--}
```
public int getUpperLeftRow()
```


يمثل فهرس الصف العلوي.

**Remarks**

إذا كان الشكل داخل شكل آخر أو داخل مجموعة، سيتم تجاهل UpperLeftRow.

**Example**

```
         if (shape.getUpperLeftRow() == 3)
             shape.setUpperLeftRow(1);
```

**Returns:**
int
### getWidth() {#getWidth--}
```
public int getWidth()
```


يمثل عرض الشكل، بوحدة البكسل.

**Example**

```
         if (shape.getWidth() == 3)
             shape.setWidth(1);
```

**Returns:**
int
### getWidthCM() {#getWidthCM--}
```
public double getWidthCM()
```


يمثل عرض الشكل، بوحدة السنتيمتر.

**Example**

```
         if (shape.getWidthCM() == 3)
             shape.setWidthCM(1);
```

**Returns:**
double
### getWidthInShape() {#getWidthInShape--}
```
public int getWidthInShape()
```


يمثل عرض الشكل، بوحدة 1/4000 من الشكل الأصل.

**Remarks**

يطبق فقط عندما يكون هذا الشكل ضمن مجموعة أو مخطط.

**Example**

```
         if (shape.isInGroup() &&shape.getWidthInShape() == 2000)
             shape.setWidthInShape(4000);
```

**Returns:**
int
### getWidthInch() {#getWidthInch--}
```
public double getWidthInch()
```


يمثل عرض الشكل، بوحدة البوصة.

**Example**

```
         if (shape.getWidthInch() == 3)
             shape.setWidthInch(1);
```

**Returns:**
double
### getWidthPt() {#getWidthPt--}
```
public double getWidthPt()
```


يمثل عرض الشكل، بوحدة النقطة.

**Example**

```
         if (shape.getWidthPt() == 3)
             shape.setWidthPt(1);
```

**Returns:**
double
### getWidthScale() {#getWidthScale--}
```
public int getWidthScale()
```


يحصل على مقياس العرض، بوحدة النسبة المئوية لعرض الصورة الأصلي. إذا لم يكن الشكل صورة، فإن خاصية WidthScale تُعيد فقط 100؛

**Example**

```
         if (shape.getWidthScale() == 3)
             shape.setWidthScale(1);
```

**Returns:**
int
### getWorksheet() {#getWorksheet--}
```
public Worksheet getWorksheet()
```


يحصل على كائن [Worksheet](../../com.aspose.cells/worksheet) الذي يحتوي على هذا الشكل.

**Example**

```
         Worksheet worksheet = shape.getWorksheet();
```

**Returns:**
[Worksheet](../../com.aspose.cells/worksheet)
### getX() {#getX--}
```
public int getX()
```


يحصل على الإزاحة الأفقية للشكل من الحد الأيسر للورقة، بوحدة البكسل.

**Example**

```
         if (shape.getX() == 3)
             shape.setX(1);
```

**Returns:**
int
### getY() {#getY--}
```
public int getY()
```


يحصل على الإزاحة العمودية للشكل من الحد العلوي للورقة، بوحدة البكسل.

**Example**

```
         if (shape.getY() == 3)
             shape.setY(1);
```

**Returns:**
int
### getZOrderPosition() {#getZOrderPosition--}
```
public int getZOrderPosition()
```


يعيد موضع الشكل في ترتيب z.

**Example**

```
         shape.setZOrderPosition(3);
```

**Returns:**
int
### hasLine() {#hasLine--}
```
public boolean hasLine()
```


يحصل على ما إذا كان حد الخط للشكل مرئيًا.

**Example**

```
         if(shape.hasLine() == false)
             shape.setHasLine(true);
```

**Returns:**
boolean
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isAspectRatioLocked() {#isAspectRatioLocked--}
```
public boolean isAspectRatioLocked()
```


صحيح يعني أن نسبة أبعاد الشكل مقفلة.

**Remarks**

فقط للصور وكائنات Ole.

**Example**

```
         shape.setAspectRatioLocked(false);
```

**Returns:**
boolean
### isDecorative() {#isDecorative--}
```
public boolean isDecorative()
```


يشير إلى ما إذا كان الكائن زخرفيًا.

**Example**

```
         if (!shape.isDecorative())
             shape.setDecorative(true);
```

**Returns:**
boolean
### isEquation() {#isEquation--}
```
public boolean isEquation()
```


يشير إلى ما إذا كان الشكل يحتوي فقط على معادلة.

**Example**

```
         //If true,the shape only contains an equation.
         if(shape.isEquation())
         {
             //The shape contains only an equation
         }
```

**Returns:**
boolean
### isFilled() {#isFilled--}
```
public boolean isFilled()
```


يشير إلى ما إذا كان تنسيق التعبئة مرئيًا.

**Example**

```
         if(shape.isFilled() == false)
             shape.setFilled(true);
```

**Returns:**
boolean
### isFlippedHorizontally() {#isFlippedHorizontally--}
```
public boolean isFlippedHorizontally()
```


يحصل على ما إذا كان الشكل مقلوبًا أفقيًا.

**Example**

```
         if(shape.isFlippedHorizontally() == false)
             shape.setFlippedHorizontally(true);
```

**Returns:**
boolean
### isFlippedVertically() {#isFlippedVertically--}
```
public boolean isFlippedVertically()
```


يحصل على ما إذا كان الشكل مقلوبًا عموديًا.

**Example**

```
         if(shape.isFlippedVertically() == false)
             shape.setFlippedVertically(true);
```

**Returns:**
boolean
### isGroup() {#isGroup--}
```
public boolean isGroup()
```


يشير إلى ما إذا كان هذا الشكل شكل مجموعة.

**Example**

```
         if(shape.isGroup())
         {
             //This shape is a group.
         }
```

**Returns:**
boolean
### isHidden() {#isHidden--}
```
public boolean isHidden()
```


يشير إلى ما إذا كان الكائن مرئيًا.

**Example**

```
         shape.setHidden(false);
```

**Returns:**
boolean
### isHorizontal() {#isHorizontal--}
```
public boolean isHorizontal()
```


يشير إلى ما إذا كان هذا شريط تمرير أفقي.

**Returns:**
boolean
### isInGroup() {#isInGroup--}
```
public boolean isInGroup()
```


يشير إلى ما إذا كان الشكل مجموعة.

**Returns:**
boolean
### isLockAspectRatio() {#isLockAspectRatio--}
```
public boolean isLockAspectRatio()
```


صحيح يعني أن نسبة أبعاد الشكل مقفلة.

**Remarks**

فقط للصور وكائنات Ole. ملاحظة: هذه العضو الآن مهمل. بدلاً من ذلك، يرجى استخدام الخاصية Shape.IsAspectRatioLocked. سيتم إزالة هذه الخاصية بعد 12 شهرًا منذ يوليو 2024. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

**Example**

```
         shape.setHidden(false);
```

**Returns:**
boolean
### isLocked() {#isLocked--}
```
public boolean isLocked()
```


True يعني أن الكائن لا يمكن تعديله عندما تكون الورقة محمية. لاحظ أن هذه القيمة ذات معنى فقط إذا كانت ورقة العمل أو الكائنات في ورقة العمل محمية.

**Example**

```
         //Sets the specified shape to unlocked state
         if (shape.getWorksheet().isProtected() &&shape.isLocked())
         {
             shape.setLocked(false);
         }
 
         //Sets the specified shape to a locked state
         if (shape.getWorksheet().isProtected() &&!shape.isLocked())
         {
             shape.setLocked(true);
         }
```

**Returns:**
boolean
### isPrintable() {#isPrintable--}
```
public boolean isPrintable()
```


يشير إلى ما إذا كان الكائن قابلًا للطباعة. إذا كان False، فلن يتم طباعة هذا الشكل عند الطباعة.

**Example**

```
         if(shape.isPrintable())
             shape.setPrintable(false);
```

**Returns:**
boolean
### isRichText() {#isRichText--}
```
public boolean isRichText()
```


ما إذا كان النص نصًا غنيًا أم لا.

**Example**

```
         if(shape.isRichText())
             System.out.println("The text is rich text.");
```

**Returns:**
boolean
### isSameSetting(Object obj) {#isSameSetting-java.lang.Object-}
```
public boolean isSameSetting(Object obj)
```


يعيد ما إذا كان الشكل متماثلًا.

**Example**

```
         if (shape.isSameSetting(shape))
             System.out.println("Two objects the same.");
```

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| obj | java.lang.Object |  |

**Returns:**
boolean -
### isSmartArt() {#isSmartArt--}
```
public boolean isSmartArt()
```


يشير إلى ما إذا كان الشكل فنًا ذكيًا.

**Remarks**

فقط لملف ooxml.

**Example**

```
         //if true,the shape is a smart art.
         if(shape.isSmartArt())
         {
             //The shape is SmartArt object.
         }
```

**Returns:**
boolean
### isTextWrapped() {#isTextWrapped--}
```
public boolean isTextWrapped()
```


يحصل على نوع التفاف النص للشكل الذي يحتوي على نص.

**Example**

```
         if (shape.isTextWrapped())
             shape.setTextWrapped(!shape.isTextWrapped());
```

**Returns:**
boolean
### isWordArt() {#isWordArt--}
```
public boolean isWordArt()
```


يشير إلى ما إذا كان هذا الشكل فن كلمة.

**Remarks**

فقط للشكل Legacy لملف xls.

**Example**

```
         if(shape.isWordArt())
         {
             //This shape is a WordArt object.
         }
```

**Returns:**
boolean
### moveToRange(int topRow, int leftColumn, int bottomRow, int rightColumn) {#moveToRange-int-int-int-int-}
```
public void moveToRange(int topRow, int leftColumn, int bottomRow, int rightColumn)
```


ينقل الشكل إلى نطاق محدد.

**Example**

```
         shape.moveToRange(12, 3, 13, 5);
```

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| topRow | int | فهرس الصف العلوي الأيسر. |
| leftColumn | int | فهرس العمود العلوي الأيسر. |
| bottomRow | int | فهرس الصف السفلي الأيمن. |
| rightColumn | int | فهرس العمود السفلي الأيمن. |

### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### removeActiveXControl() {#removeActiveXControl--}
```
public void removeActiveXControl()
```


إزالة عنصر التحكم ActiveX.

**Example**

```
         if(shape.getActiveXControl() != null)
         {
             shape.removeActiveXControl();
         }
```

### removeHyperlink() {#removeHyperlink--}
```
public void removeHyperlink()
```


يزيل الارتباط التشعبي للشكل.

**Example**

```
         shape.removeHyperlink();
```

### setAlternativeText(String value) {#setAlternativeText-java.lang.String-}
```
public void setAlternativeText(String value)
```


يرجع أو يضبط النص الوصفي (البديل) لكائن الـ [Shape](../../com.aspose.cells/shape).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

### setAnchorType(int value) {#setAnchorType-int-}
```
public void setAnchorType(int value)
```


يضبط نوع العنصر النائب لمرساة الشكل.

انظر [ShapeAnchorType](../../com.aspose.cells/shapeanchortype).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setAspectRatioLocked(boolean value) {#setAspectRatioLocked-boolean-}
```
public void setAspectRatioLocked(boolean value)
```


صحيح يعني أن نسبة أبعاد الشكل مقفلة.

**Remarks**

فقط للصور وكائنات Ole.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setAutoShapeType(int value) {#setAutoShapeType-int-}
```
public void setAutoShapeType(int value)
```


يضبط نوع الشكل التلقائي.

انظر [AutoShapeType](../../com.aspose.cells/autoshapetype).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setBottom(int value) {#setBottom-int-}
```
public void setBottom(int value)
```


يمثل عرض الإزاحة العمودية للشكل من صف زاوية أسفله السفلية، بوحدة البكسل.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setCreateId(UUID value) {#setCreateId-java.util.UUID-}
```
public void setCreateId(UUID value)
```


يضبط معرف الإنشاء لهذا الشكل.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.util.UUID |  |

### setCurrentValue(int value) {#setCurrentValue-int-}
```
public void setCurrentValue(int value)
```


يضبط القيمة الحالية.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setDecorative(boolean value) {#setDecorative-boolean-}
```
public void setDecorative(boolean value)
```


يشير إلى ما إذا كان الكائن زخرفيًا.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setFilled(boolean value) {#setFilled-boolean-}
```
public void setFilled(boolean value)
```


يشير إلى ما إذا كان تنسيق التعبئة مرئيًا.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setFlippedHorizontally(boolean value) {#setFlippedHorizontally-boolean-}
```
public void setFlippedHorizontally(boolean value)
```


يضبط ما إذا كان الشكل مقلوبًا أفقيًا.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setFlippedVertically(boolean value) {#setFlippedVertically-boolean-}
```
public void setFlippedVertically(boolean value)
```


يضبط ما إذا كان الشكل مقلوبًا عموديًا.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setFont(Font value) {#setFont-com.aspose.cells.Font-}
```
public void setFont(Font value)
```


يمثل خط الشكل.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | [Font](../../com.aspose.cells/font) |  |

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


يمثل ارتفاع الشكل، بوحدة السنتيمتر.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | double |  |

### setHeightInShape(int value) {#setHeightInShape-int-}
```
public void setHeightInShape(int value)
```


يمثل الإزاحة العمودية للشكل من الحد العلوي للشكل الأب، بوحدة 1/4000 من ارتفاع الشكل الأب.

**Remarks**

يطبق فقط عندما يكون هذا الشكل ضمن مجموعة أو مخطط.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

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

### setHorizontal(boolean value) {#setHorizontal-boolean-}
```
public void setHorizontal(boolean value)
```


يشير إلى ما إذا كان هذا شريط تمرير أفقي.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setHtmlText(String value) {#setHtmlText-java.lang.String-}
```
public void setHtmlText(String value)
```


يضبط سلسلة HTML التي تحتوي على البيانات وبعض التنسيقات في مربع النص هذا.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

### setIncrementalChange(int value) {#setIncrementalChange-int-}
```
public void setIncrementalChange(int value)
```


يضبط مقدار الزيادة التي يتم تطبيقها على شريط التمرير أو المؤشر عند تمرير سطر واحد.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setInputRange(String value) {#setInputRange-java.lang.String-}
```
public void setInputRange(String value)
```


يضبط نطاق ورقة العمل المستخدم لملء مربع الاختيار المحدد.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

### setInputRange(String formula, boolean isR1C1, boolean isLocal) {#setInputRange-java.lang.String-boolean-boolean-}
```
public void setInputRange(String formula, boolean isR1C1, boolean isLocal)
```


يضبط النطاق المستخدم لملء عنصر التحكم.

**Example**

```
         //After executing the code below, a ListBox object is created in the generated file. When the selected option is clicked, the selected value is displayed in cell A12.
 
         for (int i = 0; i? ++i)
         {
             Cell cell = book.getWorksheets().get(0).getCells().get(i, 0);
             cell.setValue(i + 1);
         }
 
         //Create a ListBox object
 
         //ActiveX Controls
         //Aspose.Cells.Drawing.Shape listBox = book.Worksheets[0].Shapes.AddActiveXControl( Aspose.Cells.Drawing.ActiveXControls.ControlType.ListBox,2, 0, 2, 0, 130, 130);
 
         //Form Controls
         Shape listBox = book.getWorksheets().get(0).getShapes().addListBox(2, 0, 2, 0, 130, 130);
 
         //Sets the range used to fill the control.
         listBox.setInputRange("$A$1:$A$6", false, false);
 
         //Sets the range linked to the control's value.
         listBox.setLinkedCell("$A$12", false, true);
```

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| formula | java.lang.String | النطاق المستخدم لملء التحكم. |
| isR1C1 | boolean | ما إذا كانت الصيغة تحتاج إلى تنسيق كـ R1C1. |
| isLocal | boolean | ما إذا كانت الصيغة تحتاج إلى تنسيق حسب الإعدادات الإقليمية. |

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

### setLeftInShape(int value) {#setLeftInShape-int-}
```
public void setLeftInShape(int value)
```


يمثل الإزاحة الأفقية للشكل من الحد الأيسر للشكل الأب، بوحدة 1/4000 من عرض الشكل الأب.

**Remarks**

يطبق فقط عندما يكون هذا الشكل ضمن مجموعة أو مخطط.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

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


يضبط الإزاحة الأفقية للشكل من الحد الأيسر لورقة العمل.

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

### setLinkedCell(String formula, boolean isR1C1, boolean isLocal) {#setLinkedCell-java.lang.String-boolean-boolean-}
```
public void setLinkedCell(String formula, boolean isR1C1, boolean isLocal)
```


يضبط النطاق المرتبط بقيمة عنصر التحكم.

**Example**

```
         //After executing the code below, a ScrollBar object is created in the generated file. As you drag the slider, the value is displayed in cell A12.
 
         //ActiveX Controls
         //Aspose.Cells.Drawing.Shape scrollBar = book.Worksheets[0].Shapes.AddActiveXControl( Aspose.Cells.Drawing.ActiveXControls.ControlType.ScrollBar,2, 0, 2, 0, 30, 130);
 
         //Form Controls
         Shape scrollBar = book.getWorksheets().get(0).getShapes().addScrollBar(2, 0, 2, 0, 130, 30);
 
         //Sets the range linked to the control's value.
         scrollBar.setLinkedCell("$A$12", false, true);
```

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| formula | java.lang.String | النطاق المرتبط بقيمة التحكم. |
| isR1C1 | boolean | ما إذا كانت الصيغة تحتاج إلى تنسيق كـ R1C1. |
| isLocal | boolean | ما إذا كانت الصيغة تحتاج إلى تنسيق حسب الإعدادات الإقليمية. |

### setLockAspectRatio(boolean value) {#setLockAspectRatio-boolean-}
```
public void setLockAspectRatio(boolean value)
```


صحيح يعني أن نسبة أبعاد الشكل مقفلة.

**Remarks**

فقط للصور وكائنات Ole. ملاحظة: هذه العضو الآن مهمل. بدلاً من ذلك، يرجى استخدام الخاصية Shape.IsAspectRatioLocked. سيتم إزالة هذه الخاصية بعد 12 شهرًا منذ يوليو 2024. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setLocked(boolean value) {#setLocked-boolean-}
```
public void setLocked(boolean value)
```


True يعني أن الكائن لا يمكن تعديله عندما تكون الورقة محمية. لاحظ أن هذه القيمة ذات معنى فقط إذا كانت ورقة العمل أو الكائنات في ورقة العمل محمية.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setLockedProperty(int type, boolean value) {#setLockedProperty-int-boolean-}
```
public void setLockedProperty(int type, boolean value)
```


ضبط الخاصية المقفلة.

**Example**

```
         shape.setLockedProperty(ShapeLockType.ADJUST_HANDLES, true);
```

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| type | int | [ShapeLockType](../../com.aspose.cells/shapelocktype). النوع المقفل. |
| القيمة | boolean | قيمة الخاصية. |

### setLowerDeltaX(int value) {#setLowerDeltaX-int-}
```
public void setLowerDeltaX(int value)
```


يضبط الإزاحة الأفقية للشكل من عمود زاويته السفلية اليمنى.

**Remarks**

نطاق القيمة هو من 0 إلى 1024.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setLowerDeltaY(int value) {#setLowerDeltaY-int-}
```
public void setLowerDeltaY(int value)
```


يضبط الإزاحة العمودية للشكل من صف زاويته السفلية اليمنى.

**Remarks**

نطاق القيمة هو من 0 إلى 256.

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

### setMacroName(String value) {#setMacroName-java.lang.String-}
```
public void setMacroName(String value)
```


يضبط اسم الماكرو.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

### setMax(int value) {#setMax-int-}
```
public void setMax(int value)
```


يضبط القيمة القصوى لنطاق شريط التمرير أو المؤشر.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setMin(int value) {#setMin-int-}
```
public void setMin(int value)
```


يضبط القيمة الدنيا لنطاق شريط التمرير أو المؤشر.

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

### setPageChange(int value) {#setPageChange-int-}
```
public void setPageChange(int value)
```


يضبط تغيير الصفحة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setPlacement(int value) {#setPlacement-int-}
```
public void setPlacement(int value)
```


يمثل الطريقة التي يتم بها إرفاق كائن الرسم بالخلايا تحته. تتحكم الخاصية في وضع الكائن على ورقة العمل.

انظر [PlacementType](../../com.aspose.cells/placementtype).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setPrintable(boolean value) {#setPrintable-boolean-}
```
public void setPrintable(boolean value)
```


يشير إلى ما إذا كان الكائن قابلًا للطباعة. إذا كان False، فلن يتم طباعة هذا الشكل عند الطباعة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

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

### setShadow(boolean value) {#setShadow-boolean-}
```
public void setShadow(boolean value)
```


يشير إلى ما إذا كان الشكل يحتوي على تظليل ثلاثي الأبعاد.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setSoftEdges(double value) {#setSoftEdges-double-}
```
public void setSoftEdges(double value)
```


يضبط نصف قطر الضبابية لتطبيقه على الحواف، بوحدة النقاط.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | double |  |

### setText(String value) {#setText-java.lang.String-}
```
public void setText(String value)
```


يضبط نص هذا الشكل.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

### setTextDirection(int value) {#setTextDirection-int-}
```
public void setTextDirection(int value)
```


يضبط اتجاه تدفق النص لهذا الكائن.

انظر [TextDirectionType](../../com.aspose.cells/textdirectiontype).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setTextHorizontalAlignment(int value) {#setTextHorizontalAlignment-int-}
```
public void setTextHorizontalAlignment(int value)
```


يضبط نوع محاذاة النص الأفقية للشكل.

انظر [TextAlignmentType](../../com.aspose.cells/textalignmenttype).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setTextHorizontalOverflow(int value) {#setTextHorizontalOverflow-int-}
```
public void setTextHorizontalOverflow(int value)
```


يضبط نوع تجاوز النص الأفقي للشكل الذي يحتوي على نص.

انظر [TextOverflowType](../../com.aspose.cells/textoverflowtype).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setTextOptions(TextOptions value) {#setTextOptions-com.aspose.cells.TextOptions-}
```
public void setTextOptions(TextOptions value)
```


يمثل خيارات النص للشكل.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | [TextOptions](../../com.aspose.cells/textoptions) |  |

### setTextOrientationType(int value) {#setTextOrientationType-int-}
```
public void setTextOrientationType(int value)
```


يضبط نوع توجيه النص للشكل.

انظر [TextOrientationType](../../com.aspose.cells/textorientationtype).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setTextShapeType(int value) {#setTextShapeType-int-}
```
public void setTextShapeType(int value)
```


يضبط نوع شكل النص المسبق.

انظر [AutoShapeType](../../com.aspose.cells/autoshapetype).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setTextVerticalAlignment(int value) {#setTextVerticalAlignment-int-}
```
public void setTextVerticalAlignment(int value)
```


يضبط نوع محاذاة النص العمودية للشكل.

انظر [TextAlignmentType](../../com.aspose.cells/textalignmenttype).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setTextVerticalOverflow(int value) {#setTextVerticalOverflow-int-}
```
public void setTextVerticalOverflow(int value)
```


يضبط نوع تجاوز النص العمودي للشكل الذي يحتوي على نص.

انظر [TextOverflowType](../../com.aspose.cells/textoverflowtype).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

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

### setTopInShape(int value) {#setTopInShape-int-}
```
public void setTopInShape(int value)
```


يمثل الإزاحة العمودية للشكل من الحد العلوي للشكل الأب، بوحدة 1/4000 من ارتفاع الشكل الأب.

**Remarks**

يطبق فقط عندما يكون هذا الشكل ضمن مجموعة أو مخطط.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

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


يضبط الإزاحة العمودية للشكل من الحد العلوي لورقة العمل، بوحدة البكسل.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setUpperDeltaX(int value) {#setUpperDeltaX-int-}
```
public void setUpperDeltaX(int value)
```


يضبط الإزاحة الأفقية للشكل من عمود زاويته العلوية اليسرى.

**Remarks**

نطاق القيمة هو من 0 إلى 1024.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setUpperDeltaY(int value) {#setUpperDeltaY-int-}
```
public void setUpperDeltaY(int value)
```


يضبط الإزاحة العمودية للشكل من صف زاويته العلوية اليسرى.

**Remarks**

نطاق القيمة هو من 0 إلى 256.

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


يمثل فهرس الصف العلوي.

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

### setWidthInShape(int value) {#setWidthInShape-int-}
```
public void setWidthInShape(int value)
```


يمثل عرض الشكل، بوحدة 1/4000 من الشكل الأصل.

**Remarks**

يطبق فقط عندما يكون هذا الشكل ضمن مجموعة أو مخطط.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

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


يضبط الإزاحة الأفقية للشكل من الحد الأيسر لورقة العمل، بوحدة البكسل.

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

### toFrontOrBack(int orders) {#toFrontOrBack-int-}
```
public void toFrontOrBack(int orders)
```


ينقل الشكل إلى المقدمة أو يرسله إلى الخلف.

**Example**

```
         shape.toFrontOrBack(2);
         //or shape.ToFrontOrBack(-1);
```

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| orders | int | إذا كان أقل من الصفر، يضع الشكل في الخلف. إذا كان أكبر من الصفر، يجلب الشكل إلى الأمام. |

### toImage(OutputStream stream, ImageFormat imageFormat) {#toImage-java.io.OutputStream-com.aspose.cells.ImageFormat-}
```
public void toImage(OutputStream stream, ImageFormat imageFormat)
```


ينشئ صورة الشكل ويحفظها إلى تدفق بالصيغة المحددة.

**Remarks**

الصيغ التالية مدعومة: .bmp, .gif, .jpg, .jpeg, .tiff, .emf.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| stream | java.io.OutputStream | دفق الإخراج. |
| imageFormat | [ImageFormat](../../com.aspose.cells/imageformat) | الصيغة التي سيتم حفظ الصورة بها. |

### toImage(OutputStream stream, ImageOrPrintOptions options) {#toImage-java.io.OutputStream-com.aspose.cells.ImageOrPrintOptions-}
```
public void toImage(OutputStream stream, ImageOrPrintOptions options)
```


يحفظ الشكل إلى تدفق.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| stream | java.io.OutputStream |  |
| options | [ImageOrPrintOptions](../../com.aspose.cells/imageorprintoptions) |  |

### toImage(String imageFile, ImageOrPrintOptions options) {#toImage-java.lang.String-com.aspose.cells.ImageOrPrintOptions-}
```
public void toImage(String imageFile, ImageOrPrintOptions options)
```


يحفظ الشكل إلى ملف.

**Example**

```
         ImageOrPrintOptions op = new ImageOrPrintOptions();
         shape.toImage("exmaple.png", op);
```

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| imageFile | java.lang.String |  |
| options | [ImageOrPrintOptions](../../com.aspose.cells/imageorprintoptions) |  |

### toString() {#toString--}
```
public String toString()
```




**Returns:**
java.lang.String
### updateSelectedValue() {#updateSelectedValue--}
```
public void updateSelectedValue()
```


تحديث القيمة المحددة بقيمة الخلية المرتبطة.

**Example**

```
         Cell cell = null;
         for (int i = 0; i? ++i)
         {
             cell = book.getWorksheets().get(0).getCells().get(i, 0);
             cell.setValue(i + 1);
         }
 
         //Create a ListBox object
 
         //ActiveX Controls
         //Aspose.Cells.Drawing.Shape listBox = book.Worksheets[0].Shapes.AddActiveXControl( Aspose.Cells.Drawing.ActiveXControls.ControlType.ListBox,2, 0, 2, 0, 130, 130);
 
         //Form Controls
         Shape listBox = book.getWorksheets().get(0).getShapes().addListBox(2, 0, 2, 0, 130, 130);
 
         //Sets the range used to fill the control.
         listBox.setInputRange("$A$1:$A$6", false, false);
 
         //Sets the range linked to the control's value.
         listBox.setLinkedCell("$A$12", false, true);
 
         ListBox listbx = (ListBox)listBox;
 
         //Set the value of cell A12
         cell = book.getWorksheets().get(0).getCells().get(11, 0);
         cell.setValue(3);
 
         //Update the selected value by the value of the linked cell.
         listBox.updateSelectedValue();
 
         //-1 default, no option selected
         if(listbx.isSelected(2))
         {
             //Option 3 of the ListBox is selected
         }
 
         //Change the value of a linked cell
         cell.setValue(4);
 
         //Update the selected value by the value of the linked cell.
         listBox.updateSelectedValue();
         if(listbx.isSelected(3))
         {
             //Option 4 of the ListBox is selected
         }
```

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

