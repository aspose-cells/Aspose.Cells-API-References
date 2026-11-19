---
title: "خلية"
second_title: "Aspose.Cells for Java API Reference"
description: "يغلف الكائن الذي يمثل خلية واحدة في دفتر العمل."
type: docs
url: /ar/java/com.aspose.cells/cell/
---

**Inheritance:**
java.lang.Object
```
public class Cell
```

يغلف الكائن الذي يمثل خلية واحدة في دفتر العمل.

**Example**

```
         Workbook excel = new Workbook();
         Cells cells = excel.getWorksheets().get(0).getCells();
 
         //Put a string into a cell
         Cell cell = cells.get(0, 0);
         cell.putValue("Hello");
 
         String first = cell.getStringValue();
 
         //Put an integer into a cell
         cell = cells.get("B1");
         cell.putValue(12);
 
         int second = cell.getIntValue();
 
         //Put a double into a cell
         cell = cells.get(0, 2);
         cell.putValue(-1.234);
 
         double third = cell.getDoubleValue();
 
         //Put a formula into a cell
         cell = cells.get("D1");
         cell.setFormula("=B1 + C1");
 
         //Put a combined formula: "sum(average(b1,c1), b1)" to cell at b2
         cell = cells.get("b2");
         cell.setFormula("=sum(average(b1,c1), b1)");
 
         //Set style of a cell
         Style style = cell.getStyle();
         //Set background color
         style.setBackgroundColor(Color.getYellow());
         //Set format of a cell
         style.getFont().setName("Courier New");
         style.setVerticalAlignment(TextAlignmentType.TOP);
          cell.setStyle(style);
```
## الطرق

| طريقة | الوصف |
| --- | --- |
| [calculate(CalculationOptions options)](#calculate-com.aspose.cells.CalculationOptions-) | يحسب صيغة الخلية. |
| [characters(int startIndex, int length)](#characters-int-int-) | يعيد كائن Characters الذي يمثل نطاقًا من الأحرف داخل نص الخلية. |
| [containsExternalLink()](#containsExternalLink--) | يشير إلى ما إذا كانت هذه الخلية تحتوي على رابط خارجي. |
| [copy(Cell cell)](#copy-com.aspose.cells.Cell-) | ينسخ البيانات من خلية المصدر. |
| [equals(Cell cell)](#equals-com.aspose.cells.Cell-) | يتحقق مما إذا كان هذا الكائن يشير إلى نفس الخلية مع كائن خلية آخر. |
| [equals(Object obj)](#equals-java.lang.Object-) | يتحقق مما إذا كان هذا الكائن يشير إلى نفس الخلية مع آخر. |
| [getArrayRange()](#getArrayRange--) | يحصل على نطاق المصفوفة إذا كانت صيغة الخلية صيغة مصفوفة. |
| [getBoolValue()](#getBoolValue--) | يحصل على القيمة المنطقية الموجودة في الخلية. |
| [getCharacters()](#getCharacters--) | يعيد جميع كائنات Characters التي تمثل نطاقًا من الأحرف داخل نص الخلية. |
| [getCharacters(boolean flag)](#getCharacters-boolean-) | يعيد جميع كائنات Characters التي تمثل نطاقًا من الأحرف داخل نص الخلية. |
| [getClass()](#getClass--) |  |
| [getColumn()](#getColumn--) | يحصل على رقم العمود (بدءًا من الصفر) للخلية. |
| [getComment()](#getComment--) | يحصل على التعليق الخاص بهذه الخلية. |
| [getConditionalFormattingResult()](#getConditionalFormattingResult--) | احصل على نتيجة التنسيق الشرطي. |
| [getDateTimeValue()](#getDateTimeValue--) | يحصل على قيمة DateTime الموجودة في الخلية. |
| [getDependents(boolean isAll)](#getDependents-boolean-) | احصل على جميع الخلايا التي تشير صيغتها إلى هذه الخلية مباشرة. |
| [getDependentsInCalculation(boolean recursive)](#getDependentsInCalculation-boolean-) | يحصل على جميع الخلايا التي تعتمد نتيجتها المحسوبة على هذه الخلية. |
| [getDisplayStringValue()](#getDisplayStringValue--) | يحصل على قيمة السلسلة المنسقة لهذه الخلية وفقًا لنمط عرض الخلية. |
| [getDisplayStyle()](#getDisplayStyle--) | يحصل على نمط العرض لهذه الخلية. |
| [getDisplayStyle(boolean includeMergedBorders)](#getDisplayStyle-boolean-) | يحصل على نمط العرض لهذه الخلية. |
| [getDisplayStyle(int adjacentBorders)](#getDisplayStyle-int-) | يحصل على نمط العرض لهذه الخلية. |
| [getDoubleValue()](#getDoubleValue--) | يحصل على القيمة المزدوجة الموجودة في الخلية. |
| [getEmbeddedImage()](#getEmbeddedImage--) | يحصل على الصورة المضمنة في الخلية. |
| [getFloatValue()](#getFloatValue--) | يحصل على القيمة العائمة الموجودة في الخلية. |
| [getFormatConditions()](#getFormatConditions--) | يحصل على شروط التنسيق التي تُطبق على هذه الخلية. |
| [getFormula()](#getFormula--) | يحصل على صيغة من الـ [Cell](../../com.aspose.cells/cell). |
| [getFormula(boolean isR1C1, boolean isLocal)](#getFormula-boolean-boolean-) | احصل على صيغة هذه الخلية. |
| [getFormulaLocal()](#getFormulaLocal--) | احصل على الصيغة المنسقة حسب اللغة للخلية. |
| [getHeightOfValue()](#getHeightOfValue--) | يحصل على ارتفاع القيمة بوحدة البكسل. |
| [getHtmlString()](#getHtmlString--) | يحصل على سلسلة HTML التي تحتوي على البيانات وبعض الصيغ في هذه الخلية. |
| [getHtmlString(boolean html5)](#getHtmlString-boolean-) | يحصل على سلسلة HTML التي تحتوي على البيانات وبعض الصيغ في هذه الخلية. |
| [getIntValue()](#getIntValue--) | يحصل على القيمة الصحيحة الموجودة في الخلية. |
| [getLeafs()](#getLeafs--) | احصل على جميع الخلايا التي تشير إلى هذه الخلية مباشرة وتحتاج إلى تحديث عندما يتم تعديل هذه الخلية. |
| [getLeafs(boolean recursive)](#getLeafs-boolean-) | احصل على جميع الخلايا التي سيتم تحديثها عندما يتم تعديل هذه الخلية. |
| [getMergedRange()](#getMergedRange--) | يرجع كائن [Range](../../com.aspose.cells/range) الذي يمثل نطاقًا مدمجًا. |
| [getName()](#getName--) | يحصل على اسم الخلية. |
| [getNumberCategoryType()](#getNumberCategoryType--) | يمثل نوع الفئة لتنسيق أرقام هذه الخلية. |
| [getPicture()](#getPicture--) | يحصل على نسخة [Picture](../../com.aspose.cells/picture) لتمثيل الصورة المدمجة في هذه الخلية أو null إذا لم توجد صورة مدمجة لهذه الخلية. |
| [getPrecedents()](#getPrecedents--) | يحصل على جميع المراجع التي تظهر في صيغة هذه الخلية. |
| [getPrecedentsInCalculation()](#getPrecedentsInCalculation--) | يحصل على جميع السلف (إشارة إلى خلايا في المصنف الحالي) المستخدمة في صيغة هذه الخلية أثناء حسابها. |
| [getR1C1Formula()](#getR1C1Formula--) | يحصل على صيغة R1C1 للـ [Cell](../../com.aspose.cells/cell). |
| [getRichValue()](#getRichValue--) | يحصل على القيمة الغنية للخلية. |
| [getRow()](#getRow--) | يحصل على رقم الصف (مبني على الصفر) للخلية. |
| [getSharedStyleIndex()](#getSharedStyleIndex--) | يحصل على فهرس النمط المشترك للخلية في مجموعة الأنماط. |
| [getStringValue()](#getStringValue--) | يحصل على القيمة النصية الموجودة في الخلية. |
| [getStringValue(int formatStrategy)](#getStringValue-int-) | يحصل على القيمة النصية وفق استراتيجية تنسيق محددة. |
| [getStringValueWithoutFormat()](#getStringValueWithoutFormat--) | يحصل على قيمة الخلية كنص دون أي تنسيق. |
| [getStyle()](#getStyle--) | يحصل على نمط الخلية. |
| [getStyle(boolean checkBorders)](#getStyle-boolean-) | إذا كان checkBorders صحيحًا، تحقق مما إذا كانت حدود الخلايا الأخرى ستؤثر على نمط هذه الخلية. |
| [getTable()](#getTable--) | يحصل على الجدول الذي يحتوي على هذه الخلية. |
| [getType()](#getType--) | يمثل نوع قيمة الخلية. |
| [getValidation()](#getValidation--) | يحصل على التحقق المطبق على هذه الخلية. |
| [getValidationValue()](#getValidationValue--) | يحصل على قيمة التحقق المطبق على هذه الخلية. |
| [getValue()](#getValue--) | يحصل على القيمة الموجودة في هذه الخلية. |
| [getWidthOfValue()](#getWidthOfValue--) | يحصل على عرض القيمة بوحدة البكسل. |
| [getWorksheet()](#getWorksheet--) | يحصل على ورقة العمل الأصلية. |
| [hasCustomFunction()](#hasCustomFunction--) | يتحقق مما إذا كان هناك دالة مخصصة (دالة غير مدعومة) في صيغة هذه الخلية. |
| [hasCustomStyle()](#hasCustomStyle--) | يشير إلى ما إذا كانت هذه الخلية لديها إعدادات نمط مخصصة (مختلفة عن الإعداد الافتراضي الموروث من الصف أو العمود أو المصنف المقابل). |
| [hashCode()](#hashCode--) | يعمل كدالة تجزئة لنوع معين. |
| [insertText(int index, String text)](#insertText-int-java.lang.String-) | إدراج بعض الأحرف إلى الخلية. |
| [isArrayFormula()](#isArrayFormula--) | يشير إلى ما إذا كانت صيغة الخلية صيغة مصفوفة. |
| [isArrayHeader()](#isArrayHeader--) | يشير إلى أن صيغة الخلية هي صيغة مصفوفة وأنها الخلية الأولى في المصفوفة. |
| [isCheckBoxStyle()](#isCheckBoxStyle--) | يشير إلى ما إذا تم تعيين هذه الخلية كمربع اختيار. |
| [isDynamicArrayFormula()](#isDynamicArrayFormula--) | يشير إلى ما إذا كانت صيغة الخلية صيغة مصفوفة ديناميكية (true) أو صيغة مصفوفة قديمة (false). |
| [isErrorValue()](#isErrorValue--) | يتحقق مما إذا كانت قيمة هذه الخلية خطأ. |
| [isFormula()](#isFormula--) | يمثل ما إذا كانت الخلية المحددة تحتوي على صيغة. |
| [isInArray()](#isInArray--) | يشير إلى ما إذا كانت صيغة الخلية صيغة مصفوفة. |
| [isInTable()](#isInTable--) | يشير إلى ما إذا كانت هذه الخلية جزءًا من صيغة جدول. |
| [isMerged()](#isMerged--) | يتحقق مما إذا كانت الخلية جزءًا من نطاق مدمج أم لا. |
| [isNumericValue()](#isNumericValue--) | يشير إلى ما إذا كانت قيمة هذه الخلية رقمية (int، double و datetime). |
| [isRichText()](#isRichText--) | يشير إلى ما إذا كانت القيمة النصية لهذه الخلية نصًا منسقًا غنيًا. |
| [isSharedFormula()](#isSharedFormula--) | يشير إلى ما إذا كانت صيغة الخلية جزءًا من صيغة مشتركة. |
| [isStyleSet()](#isStyleSet--) | يشير إلى ما إذا تم تعيين نمط الخلية. |
| [isTableFormula()](#isTableFormula--) | يشير إلى ما إذا كانت هذه الخلية جزءًا من صيغة جدول. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [putValue(boolean boolValue)](#putValue-boolean-) | يضع قيمة منطقية في الخلية. |
| [putValue(DateTime dateTime)](#putValue-com.aspose.cells.DateTime-) | يضع قيمة تاريخ/وقت في الخلية. |
| [putValue(double doubleValue)](#putValue-double-) | يضع قيمة مزدوجة في الخلية. |
| [putValue(int intValue)](#putValue-int-) | يضع قيمة صحيحة في الخلية. |
| [putValue(Object objectValue)](#putValue-java.lang.Object-) | يضع قيمة كائن في الخلية. |
| [putValue(String stringValue)](#putValue-java.lang.String-) | يضع قيمة نصية في الخلية. |
| [putValue(String stringValue, boolean isConverted)](#putValue-java.lang.String-boolean-) | يضع قيمة نصية في الخلية ويحول القيمة إلى نوع بيانات آخر إذا كان ذلك مناسبًا. |
| [putValue(String stringValue, boolean isConverted, boolean setStyle)](#putValue-java.lang.String-boolean-boolean-) | يضع قيمة في الخلية، وإذا كان مناسبًا سيتم تحويل القيمة إلى نوع بيانات آخر وسيتم إعادة تعيين تنسيق الأرقام للخلية. |
| [removeArrayFormula(boolean leaveNormalFormula)](#removeArrayFormula-boolean-) | إزالة صيغة المصفوفة. |
| [replace(String placeHolder, String newValue, ReplaceOptions options)](#replace-java.lang.String-java.lang.String-com.aspose.cells.ReplaceOptions-) | استبدال نص الخلية بالخيارات. |
| [setArrayFormula(String arrayFormula, int rowNumber, int columnNumber)](#setArrayFormula-java.lang.String-int-int-) | يضبط صيغة مصفوفة (صيغة مصفوفة قديمة تُدخل عبر CTRL+SHIFT+ENTER في MS Excel) لنطاق من الخلايا. |
| [setArrayFormula(String arrayFormula, int rowNumber, int columnNumber, boolean isR1C1, boolean isLocal)](#setArrayFormula-java.lang.String-int-int-boolean-boolean-) | يضبط صيغة مصفوفة لنطاق من الخلايا. |
| [setArrayFormula(String arrayFormula, int rowNumber, int columnNumber, FormulaParseOptions options)](#setArrayFormula-java.lang.String-int-int-com.aspose.cells.FormulaParseOptions-) | يضبط صيغة مصفوفة لنطاق من الخلايا. |
| [setArrayFormula(String arrayFormula, int rowNumber, int columnNumber, FormulaParseOptions options, Object[][] values)](#setArrayFormula-java.lang.String-int-int-com.aspose.cells.FormulaParseOptions-java.lang.Object-----) | يضبط صيغة مصفوفة لنطاق من الخلايا. |
| [setCharacters(FontSetting[] characters)](#setCharacters-com.aspose.cells.FontSetting---) | يضبط تنسيق النص الغني للخلية. |
| [setCheckBoxStyle(boolean value)](#setCheckBoxStyle-boolean-) | يشير إلى ما إذا تم تعيين هذه الخلية كمربع اختيار. |
| [setDynamicArrayFormula(String arrayFormula, FormulaParseOptions options, boolean calculateValue)](#setDynamicArrayFormula-java.lang.String-com.aspose.cells.FormulaParseOptions-boolean-) | يضبط صيغة مصفوفة ديناميكية ويجعل الصيغة تمتد إلى الخلايا المجاورة إذا كان ذلك ممكنًا. |
| [setDynamicArrayFormula(String arrayFormula, FormulaParseOptions options, Object[][] values, boolean calculateRange, boolean calculateValue)](#setDynamicArrayFormula-java.lang.String-com.aspose.cells.FormulaParseOptions-java.lang.Object-----boolean-boolean-) | يضبط صيغة مصفوفة ديناميكية ويجعل الصيغة تمتد إلى الخلايا المجاورة إذا كان ذلك ممكنًا. |
| [setDynamicArrayFormula(String arrayFormula, FormulaParseOptions options, Object[][] values, boolean calculateRange, boolean calculateValue, CalculationOptions copts)](#setDynamicArrayFormula-java.lang.String-com.aspose.cells.FormulaParseOptions-java.lang.Object-----boolean-boolean-com.aspose.cells.CalculationOptions-) | يضبط صيغة مصفوفة ديناميكية ويجعل الصيغة تمتد إلى الخلايا المجاورة إذا كان ذلك ممكنًا. |
| [setEmbeddedImage(byte[] value)](#setEmbeddedImage-byte---) | يضبط الصورة المدمجة في الخلية. |
| [setFormula(String value)](#setFormula-java.lang.String-) | يضبط صيغة الـ[Cell](../../com.aspose.cells/cell). |
| [setFormula(String formula, boolean isR1C1, boolean isLocal, Object value)](#setFormula-java.lang.String-boolean-boolean-java.lang.Object-) | اضبط الصيغة وقيمة الصيغة. |
| [setFormula(String formula, FormulaParseOptions options)](#setFormula-java.lang.String-com.aspose.cells.FormulaParseOptions-) | اضبط الصيغة والقيمة (النتيجة المحسوبة) للصيغة. |
| [setFormula(String formula, FormulaParseOptions options, Object value)](#setFormula-java.lang.String-com.aspose.cells.FormulaParseOptions-java.lang.Object-) | اضبط الصيغة والقيمة (النتيجة المحسوبة) للصيغة. |
| [setFormula(String formula, Object value)](#setFormula-java.lang.String-java.lang.Object-) | اضبط الصيغة والقيمة (النتيجة المحسوبة) للصيغة. |
| [setFormulaLocal(String value)](#setFormulaLocal-java.lang.String-) | احصل على الصيغة المنسقة حسب اللغة للخلية. |
| [setHtmlString(String value)](#setHtmlString-java.lang.String-) | يضبط سلسلة HTML التي تحتوي على بيانات وبعض التنسيقات في هذه الخلية. |
| [setR1C1Formula(String value)](#setR1C1Formula-java.lang.String-) | يضبط صيغة R1C1 للـ[Cell](../../com.aspose.cells/cell). |
| [setSharedFormula(String sharedFormula, int rowNumber, int columnNumber)](#setSharedFormula-java.lang.String-int-int-) | يضبط صيغًا مشتركة لنطاق من الخلايا. |
| [setSharedFormula(String sharedFormula, int rowNumber, int columnNumber, boolean isR1C1, boolean isLocal)](#setSharedFormula-java.lang.String-int-int-boolean-boolean-) | يضبط صيغة لنطاق من الخلايا. |
| [setSharedFormula(String sharedFormula, int rowNumber, int columnNumber, FormulaParseOptions options)](#setSharedFormula-java.lang.String-int-int-com.aspose.cells.FormulaParseOptions-) | يضبط صيغًا مشتركة لنطاق من الخلايا. |
| [setSharedFormula(String sharedFormula, int rowNumber, int columnNumber, FormulaParseOptions options, Object[][] values)](#setSharedFormula-java.lang.String-int-int-com.aspose.cells.FormulaParseOptions-java.lang.Object-----) | يضبط صيغًا مشتركة لنطاق من الخلايا. |
| [setStyle(Style style)](#setStyle-com.aspose.cells.Style-) | يضبط نمط الخلية. |
| [setStyle(Style style, boolean explicitFlag)](#setStyle-com.aspose.cells.Style-boolean-) | تطبيق الخاصية المعدلة للنمط على الخلية. |
| [setStyle(Style style, StyleFlag flag)](#setStyle-com.aspose.cells.Style-com.aspose.cells.StyleFlag-) | تطبيق نمط الخلية بناءً على العلامات. |
| [setTableFormula(int rowNumber, int columnNumber, int rowIndexOfInputCell, int columnIndexOfInputCell, boolean isRowInput, Object[][] values)](#setTableFormula-int-int-int-int-boolean-java.lang.Object-----) | إنشاء جدول بيانات بمتغير واحد للنطاق المحدد بدءًا من هذه الخلية. |
| [setTableFormula(int rowNumber, int columnNumber, int rowIndexOfRowInputCell, int columnIndexOfRowInputCell, int rowIndexOfColumnInputCell, int columnIndexOfColumnInputCell, Object[][] values)](#setTableFormula-int-int-int-int-int-int-java.lang.Object-----) | إنشاء جدول بيانات بمتغيرين للنطاق المحدد بدءًا من هذه الخلية. |
| [setTableFormula(int rowNumber, int columnNumber, String inputCell, boolean isRowInput, Object[][] values)](#setTableFormula-int-int-java.lang.String-boolean-java.lang.Object-----) | إنشاء جدول بيانات بمتغير واحد للنطاق المحدد بدءًا من هذه الخلية. |
| [setTableFormula(int rowNumber, int columnNumber, String rowInputCell, String columnInputCell, Object[][] values)](#setTableFormula-int-int-java.lang.String-java.lang.String-java.lang.Object-----) | إنشاء جدول بيانات بمتغيرين للنطاق المحدد بدءًا من هذه الخلية. |
| [setValue(Object value)](#setValue-java.lang.Object-) | يضبط القيمة الموجودة في هذه الخلية. |
| [toJson()](#toJson--) | تحويل الـ[Cell](../../com.aspose.cells/cell) إلى بيانات هيكل JSON. |
| [toString()](#toString--) | يرجع سلسلة تمثل كائن Cell الحالي. |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### calculate(CalculationOptions options) {#calculate-com.aspose.cells.CalculationOptions-}
```
public void calculate(CalculationOptions options)
```


يحسب صيغة الخلية.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| options | [CalculationOptions](../../com.aspose.cells/calculationoptions) | خيارات الحساب |

### characters(int startIndex, int length) {#characters-int-int-}
```
public FontSetting characters(int startIndex, int length)
```


يعيد كائن Characters الذي يمثل نطاقًا من الأحرف داخل نص الخلية.

**Remarks**

هذه الطريقة تعمل فقط على الخلية التي تحتوي على قيمة نصية.

**Example**

```
         Workbook excel = new Workbook();
         	Cells cells = excel.getWorksheets().get(0).getCells();
         cells.get("A1").putValue("Helloworld");
         cells.get("A1").characters(5, 5).getFont().setBold(true);
         cells.get("A1").characters(5, 5).getFont().setColor(Color.getBlue());
```

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| startIndex | int | فهرس بداية الحرف. |
| length | int | عدد الأحرف. |

**Returns:**
[FontSetting](../../com.aspose.cells/fontsetting) - Characters object.
### containsExternalLink() {#containsExternalLink--}
```
public boolean containsExternalLink()
```


يشير إلى ما إذا كانت هذه الخلية تحتوي على رابط خارجي. ينطبق فقط عندما تكون الخلية خلية صيغة.

**Returns:**
boolean
### copy(Cell cell) {#copy-com.aspose.cells.Cell-}
```
public void copy(Cell cell)
```


ينسخ البيانات من خلية المصدر.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| cell | [Cell](../../com.aspose.cells/cell) | مصدر كائن [Cell](../../com.aspose.cells/cell). |

### equals(Cell cell) {#equals-com.aspose.cells.Cell-}
```
public boolean equals(Cell cell)
```


يتحقق مما إذا كان هذا الكائن يشير إلى نفس الخلية مع كائن خلية آخر.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| cell | [Cell](../../com.aspose.cells/cell) | كائن خلية آخر |

**Returns:**
منطقي - true إذا كان كائنان خلية يشيران إلى نفس الخلية.
### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```


يتحقق مما إذا كان هذا الكائن يشير إلى نفس الخلية مع آخر.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| obj | java.lang.Object | كائن آخر |

**Returns:**
منطقي - true إذا كان كائنان يشيران إلى نفس الخلية.
### getArrayRange() {#getArrayRange--}
```
public CellArea getArrayRange()
```


يحصل على نطاق المصفوفة إذا كانت صيغة الخلية صيغة مصفوفة.

**Remarks**

يطبق فقط عندما تكون صيغة الخلية صيغة مصفوفة

**Returns:**
[CellArea](../../com.aspose.cells/cellarea) - The array range.
### getBoolValue() {#getBoolValue--}
```
public boolean getBoolValue()
```


يحصل على القيمة المنطقية الموجودة في الخلية.

**Returns:**
boolean
### getCharacters() {#getCharacters--}
```
public FontSetting[] getCharacters()
```


يعيد جميع كائنات Characters التي تمثل نطاقًا من الأحرف داخل نص الخلية.

**Returns:**
com.aspose.cells.FontSetting[] - جميع كائنات الأحرف
### getCharacters(boolean flag) {#getCharacters-boolean-}
```
public FontSetting[] getCharacters(boolean flag)
```


يعيد جميع كائنات Characters التي تمثل نطاقًا من الأحرف داخل نص الخلية.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| علامة | boolean | يشير إلى ما إذا كان يتم تطبيق نمط الجدول على الخلية إذا كانت الخلية في الجدول. |

**Returns:**
com.aspose.cells.FontSetting[] - جميع كائنات الأحرف
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getColumn() {#getColumn--}
```
public int getColumn()
```


يحصل على رقم العمود (بدءًا من الصفر) للخلية.

**Returns:**
int
### getComment() {#getComment--}
```
public Comment getComment()
```


يحصل على التعليق الخاص بهذه الخلية.

**Remarks**

إذا لم يكن هناك تعليق يطبق على الخلية، يرجع null.

**Returns:**
[Comment](../../com.aspose.cells/comment)
### getConditionalFormattingResult() {#getConditionalFormattingResult--}
```
public ConditionalFormattingResult getConditionalFormattingResult()
```


احصل على نتيجة التنسيق الشرطي.

**Remarks**

يرجع null إذا لم يتم تطبيق تنسيق شرطي على هذه الخلية،

**Returns:**
[ConditionalFormattingResult](../../com.aspose.cells/conditionalformattingresult)
### getDateTimeValue() {#getDateTimeValue--}
```
public DateTime getDateTimeValue()
```


يحصل على قيمة DateTime الموجودة في الخلية.

**Returns:**
[DateTime](../../com.aspose.cells/datetime)
### getDependents(boolean isAll) {#getDependents-boolean-}
```
public Cell[] getDependents(boolean isAll)
```


احصل على جميع الخلايا التي تشير صيغتها إلى هذه الخلية مباشرة.

**Remarks**

 *  If one reference containing this cell appears in one cell's formula, that cell will be taken as the dependent of this cell, no matter the reference or this cell is used or not while calculating. For example, although cell A2 in formula "=IF(TRUE,A1,A2)" is not used while calculating, this formula is still be taken as A2's dependent.
 *  To get those formulas whose calculated results depend on this cell, please use .
 *  When tracing dependents for one cell, all formulas in the workbook or worksheet will be analized and checked. So it is a time consumed process. If user need to trace dependents for lots of cells, using this method will cause poor performance. For performance consideration, user should use  instead. Or, user may gather precedents map of all cells by  firstly, and then build the dependents map according to the precedents map.

**Example**

```
         Workbook workbook = new Workbook();
         Cells cells = workbook.getWorksheets().get(0).getCells();
         cells.get("A1").setFormula("=B1+SUM(B1:B10)+[Book1.xls]Sheet1!B2");
         cells.get("A2").setFormula("=IF(TRUE,B2,B1)");
         Cell[] dependents = cells.get("B1").getDependents(true);
         for (int i = 0; i <dependents.length; i++)
         {
              System.out.println(dependents[i].getName());
         }
```

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| isAll | boolean | يشير إلى ما إذا كان يتم فحص الصيغ في أوراق عمل أخرى |

**Returns:**
com.aspose.cells.Cell[]
### getDependentsInCalculation(boolean recursive) {#getDependentsInCalculation-boolean-}
```
public Iterator getDependentsInCalculation(boolean recursive)
```


يحصل على جميع الخلايا التي تعتمد نتيجتها المحسوبة على هذه الخلية.

**Remarks**

لاستخدام هذه الطريقة، يرجى التأكد من أن المصنف تم تعيينه بقيمة true للخاصية [FormulaSettings.getEnableCalculationChain()](../../com.aspose.cells/formulasettings\#getEnableCalculationChain--) وتم حسابه بالكامل باستخدام هذا الإعداد. إذا لم يكن هناك إشارة صيغية إلى هذه الخلية، سيتم إرجاع null.

**Example**

```
         Workbook workbook = new Workbook();
         Cells cells = workbook.getWorksheets().get(0).getCells();
         cells.get("A1").setFormula("=B1+SUM(B1:B10)+[Book1.xls]Sheet1!B2");
         cells.get("A2").setFormula("=IF(TRUE,B2,B1)");
         workbook.getSettings().getFormulaSettings().setEnableCalculationChain(true);
         workbook.calculateFormula();
         Iterator en = cells.get("B1").getDependentsInCalculation(false);
         System.out.println("B1's calculation dependents:");
         while(en.hasNext())
         {
             Cell c = (Cell)en.next();
             System.out.println(c.getName());
         }
         en = cells.get("B2").getDependentsInCalculation(false);
         System.out.println("B2's calculation dependents:");
         while(en.hasNext())
         {
             Cell c = (Cell)en.next();
             System.out.println(c.getName());
         }
```

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| recursive | boolean | ما إذا كان يرجع التبعيات التي لا تشير إلى هذه الخلية مباشرةً بل تشير إلى فروع أخرى لهذه الخلية |

**Returns:**
java.util.Iterator - مُعدد لتعداد جميع التبعيات (كائنات Cell)
### getDisplayStringValue() {#getDisplayStringValue--}
```
public String getDisplayStringValue()
```


يحصل على قيمة السلسلة المنسقة لهذه الخلية وفقًا لنمط عرض الخلية.

**Returns:**
java.lang.String
### getDisplayStyle() {#getDisplayStyle--}
```
public Style getDisplayStyle()
```


يحصل على نمط العرض لهذه الخلية.

**Remarks**

نفس الاستخدام مع [BorderType.SIDE\_BORDERS](../../com.aspose.cells/bordertype\#SIDE-BORDERS) للوظيفة [getDisplayStyle(int)](../../com.aspose.cells/cell\#getDisplayStyle-int-). أي أن هذه الطريقة ستتحقق وتضبط حدود الأعلى/الأسفل/اليسار/اليمين لهذه الخلية وفقًا للنمط ([getStyle()](../../com.aspose.cells/cell\#getStyle--)) للخلايا المجاورة لها، ولكن لا تتحقق من الخلايا المدمجة، ولا تتحقق من نمط العرض للخلايا المجاورة.

**Returns:**
[Style](../../com.aspose.cells/style) - display style of this cell
### getDisplayStyle(boolean includeMergedBorders) {#getDisplayStyle-boolean-}
```
public Style getDisplayStyle(boolean includeMergedBorders)
```


يحصل على نمط العرض لهذه الخلية.

**Remarks**

إذا كانت العلامة المحددة false، فإنها تكون مماثلة للوظيفة [getDisplayStyle()](../../com.aspose.cells/cell\#getDisplayStyle--). وإلا فإنها تكون مماثلة لاستخدام [BorderType.SIDE\_BORDERS](../../com.aspose.cells/bordertype\#SIDE-BORDERS)\|[BorderType.DYNAMIC\_STYLE\_BORDERS](../../com.aspose.cells/bordertype\#DYNAMIC-STYLE-BORDERS) للوظيفة [getDisplayStyle(int)](../../com.aspose.cells/cell\#getDisplayStyle-int-).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| includeMergedBorders | boolean | يشير إلى ما إذا كان يتم فحص حدود الخلايا المدمجة. |

**Returns:**
[Style](../../com.aspose.cells/style) - display style of this cell
### getDisplayStyle(int adjacentBorders) {#getDisplayStyle-int-}
```
public Style getDisplayStyle(int adjacentBorders)
```


يحصل على نمط العرض لهذه الخلية.

**Remarks**

إذا كانت هذه الخلية متأثرة أيضًا بإعدادات أخرى مثل التنسيق الشرطي، كائنات القوائم، إلخ، فقد يكون نمط العرض مختلفًا عن [getStyle()](../../com.aspose.cells/cell\#getStyle--).

بالنسبة للعلامات التي تضبط الحدود وفقًا للخلايا المجاورة، فإن [BorderType.TOP\_BORDER](../../com.aspose.cells/bordertype\#TOP-BORDER)/[BorderType.BOTTOM\_BORDER](../../com.aspose.cells/bordertype\#BOTTOM-BORDER)/[BorderType.LEFT\_BORDER](../../com.aspose.cells/bordertype\#LEFT-BORDER)/[BorderType.RIGHT\_BORDER](../../com.aspose.cells/bordertype\#RIGHT-BORDER) تشير إلى ما إذا كان يتم فحص ودمج حدود الأسفل/الأعلى/اليمين/اليسار للخلايا اليسرى/اليمنى/العليا/السفلى المجاورة لهذه الخلية.

لأسباب تتعلق بالأداء والتوافق، يتم استخدام بعض القيم التعداد (enums) للدلالة على بعض العمليات الخاصة:

[BorderType.HORIZONTAL](../../com.aspose.cells/bordertype\#HORIZONTAL)/[BorderType.VERTICAL](../../com.aspose.cells/bordertype\#VERTICAL) denote whether check and combine the bottom/right border of merged cells to this one.

[BorderType.DIAGONAL](../../com.aspose.cells/bordertype\#DIAGONAL)(that is, both [StyleModifyFlag.DIAGONAL\_UP\_BORDER](../../com.aspose.cells/stylemodifyflag\#DIAGONAL-UP-BORDER) and [StyleModifyFlag.DIAGONAL\_DOWN\_BORDER](../../com.aspose.cells/stylemodifyflag\#DIAGONAL-DOWN-BORDER) have been set) denotes check and combine borders from the display style of adjacent cells.

يرجى ملاحظة أن فحص حدود/أنماط الخلايا المجاورة، خاصة أنماط العرض، عملية تستغرق وقتًا. إذا لم تكن هناك حاجة للحصول على الحدود للنمط المرجع، فإن استخدام [BorderType.NONE](../../com.aspose.cells/bordertype\#NONE) لتعطيل عملية الخلايا المجاورة سيعطي أداءً أفضل. عند الحصول على حدود الخلايا المجاورة من الأنماط المعرفة على تلك الخلايا فقط (دون تعيين [BorderType.DIAGONAL](../../com.aspose.cells/bordertype\#DIAGONAL))، قد يكون الأداء أيضًا أفضل لأن فحص نمط العرض لخلية واحدة يستغرق وقتًا.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| adjacentBorders | int | [BorderType](../../com.aspose.cells/bordertype). يشير إلى الحدود التي تحتاج إلى فحصها وضبطها وفقًا لحدود الخلايا المجاورة. |

**Returns:**
[Style](../../com.aspose.cells/style) - display style of this cell
### getDoubleValue() {#getDoubleValue--}
```
public double getDoubleValue()
```


يحصل على القيمة المزدوجة الموجودة في الخلية.

**Returns:**
double
### getEmbeddedImage() {#getEmbeddedImage--}
```
public byte[] getEmbeddedImage()
```


يحصل على الصورة المضمنة في الخلية.

**Returns:**
byte[]
### getFloatValue() {#getFloatValue--}
```
public float getFloatValue()
```


يحصل على القيمة العائمة الموجودة في الخلية.

**Returns:**
float
### getFormatConditions() {#getFormatConditions--}
```
public FormatConditionCollection[] getFormatConditions()
```


يحصل على شروط التنسيق التي تُطبق على هذه الخلية.

**Returns:**
com.aspose.cells.FormatConditionCollection[] - يرجع كائن [FormatConditionCollection](../../com.aspose.cells/formatconditioncollection)
### getFormula() {#getFormula--}
```
public String getFormula()
```


يحصل على صيغة من الـ [Cell](../../com.aspose.cells/cell).

**Remarks**

دائمًا ما يبدأ نص الصيغة بعلامة مساواة (=). ويرجى دائمًا استخدام الفاصلة (,) كفاصل للمعاملات، مثل "=SUM(A1, E1, H2)".

**Example**

```
         Workbook excel = new Workbook();
         Cells cells = excel.getWorksheets().get(0).getCells();
         cells.get("B6").setFormula("=SUM(B2:B5, E1) + sheet1!A1");
```

**Returns:**
java.lang.String
### getFormula(boolean isR1C1, boolean isLocal) {#getFormula-boolean-boolean-}
```
public String getFormula(boolean isR1C1, boolean isLocal)
```


احصل على صيغة هذه الخلية.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| isR1C1 | boolean | ما إذا كانت الصيغة تحتاج إلى تنسيق كـ R1C1. |
| isLocal | boolean | ما إذا كانت الصيغة تحتاج إلى تنسيق حسب الإعدادات الإقليمية. |

**Returns:**
java.lang.String - صيغة هذه الخلية.
### getFormulaLocal() {#getFormulaLocal--}
```
public String getFormulaLocal()
```


احصل على الصيغة المنسقة حسب اللغة للخلية.

**Returns:**
java.lang.String
### getHeightOfValue() {#getHeightOfValue--}
```
public int getHeightOfValue()
```


يحصل على ارتفاع القيمة بوحدة البكسل.

**Returns:**
int -
### getHtmlString() {#getHtmlString--}
```
public String getHtmlString()
```


يحصل على سلسلة HTML التي تحتوي على البيانات وبعض الصيغ في هذه الخلية.

**Returns:**
java.lang.String
### getHtmlString(boolean html5) {#getHtmlString-boolean-}
```
public String getHtmlString(boolean html5)
```


يحصل على سلسلة HTML التي تحتوي على البيانات وبعض الصيغ في هذه الخلية.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| html5 | boolean | يشير إلى ما إذا كانت القيمة متوافقة مع html5 |

**Returns:**
java.lang.String -
### getIntValue() {#getIntValue--}
```
public int getIntValue()
```


يحصل على القيمة الصحيحة الموجودة في الخلية.

**Returns:**
int
### getLeafs() {#getLeafs--}
```
public Iterator getLeafs()
```


احصل على جميع الخلايا التي تشير إلى هذه الخلية مباشرة وتحتاج إلى تحديث عندما يتم تعديل هذه الخلية.

**Remarks**

ملاحظة: هذه الفئة الآن مهجورة. بدلاً من ذلك، يرجى استخدام Cell.GetDependentsInCalculation(bool) للحصول على جميع التبعيات في سلسلة الحساب. سيتم إزالة هذه الخاصية بعد 12 شهرًا منذ مايو 2022. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

**Returns:**
java.util.Iterator - مُعدد لتعداد جميع التبعيات (Cell)
### getLeafs(boolean recursive) {#getLeafs-boolean-}
```
public Iterator getLeafs(boolean recursive)
```


احصل على جميع الخلايا التي سيتم تحديثها عندما يتم تعديل هذه الخلية.

**Remarks**

ملاحظة: هذه الفئة الآن مهجورة. بدلاً من ذلك، يرجى استخدام Cell.GetDependentsInCalculation(bool) للحصول على جميع التبعيات في سلسلة الحساب. سيتم إزالة هذه الخاصية بعد 12 شهرًا منذ مايو 2022. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| recursive | boolean | ما إذا كان يُرجع تلك الأوراق التي لا تشير إلى هذه الخلية مباشرةً بل تشير إلى أوراق أخرى لهذه الخلية |

**Returns:**
java.util.Iterator - مُعدد لتعداد جميع التبعيات (Cell)
### getMergedRange() {#getMergedRange--}
```
public Range getMergedRange()
```


يرجع كائن [Range](../../com.aspose.cells/range) الذي يمثل نطاقًا مدمجًا.

**Returns:**
[Range](../../com.aspose.cells/range) - [Range](../../com.aspose.cells/range) object. Null if this cell is not merged.
### getName() {#getName--}
```
public String getName()
```


يحصل على اسم الخلية.

**Remarks**

يتضمن اسم الخلية حرف العمود ورقم الصف. على سبيل المثال، اسم خلية في الصف 0 والعمود 0 هو A1.

**Returns:**
java.lang.String
### getNumberCategoryType() {#getNumberCategoryType--}
```
public int getNumberCategoryType()
```


يمثل نوع الفئة لتنسيق أرقام هذه الخلية.

انظر [NumberCategoryType](../../com.aspose.cells/numbercategorytype).

**Remarks**

عندما يتم دمج نمط تنسيق الخلية مع أنماط التنسيق الشرطي، يكون النوع المرجع مطابقًا للجزء المستخدم للقيمة الحالية لهذه الخلية. على سبيل المثال، إذا كان نمط التنسيق لهذه الخلية هو "\#,\#\#0;(\#,\#\#0);"-";@"، فإن عندما تكون قيمة الخلية رقمية وغير صفرية، يكون النوع المرجع هو [NumberCategoryType.NUMBER](../../com.aspose.cells/numbercategorytype\#NUMBER)؛ وعندما تكون قيمة الخلية صفرًا أو غير رقمية، يكون النوع المرجع هو [NumberCategoryType.TEXT](../../com.aspose.cells/numbercategorytype\#TEXT).

**Returns:**
int
### getPicture() {#getPicture--}
```
public Picture getPicture()
```


يحصل على نسخة [Picture](../../com.aspose.cells/picture) لتمثيل الصورة المدمجة في هذه الخلية أو null إذا لم توجد صورة مدمجة لهذه الخلية.

**Returns:**
[Picture](../../com.aspose.cells/picture)
### getPrecedents() {#getPrecedents--}
```
public ReferredAreaCollection getPrecedents()
```


يحصل على جميع المراجع التي تظهر في صيغة هذه الخلية.

**Remarks**

 *  Returns null if this is not a formula cell.
 *  All references appearing in this cell's formula will be returned no matter they are referenced or not while calculating. For example, although cell A2 in formula "=IF(TRUE,A1,A2)" is not used while calculating, it is still taken as the formula's precedents.
 *  To get those references which influence the calculation only, please use .

**Example**

```
         Workbook workbook = new Workbook();
         Cells cells = workbook.getWorksheets().get(0).getCells();
         cells.get("A1").setFormula("=B1+SUM(B1:B10)+[Book1.xls]Sheet1!A1");
         ReferredAreaCollection areas = cells.get("A1").getPrecedents();
         for (int i = 0; i <areas.getCount(); i++)
         {
              ReferredArea area = areas.get(i);
              StringBuilder stringBuilder = new StringBuilder();
              if (area.isExternalLink())
              {
                  stringBuilder.append("[");
                  stringBuilder.append(area.getExternalFileName());
                  stringBuilder.append("]");
              }
              stringBuilder.append(area.getSheetName());
              stringBuilder.append("!");
              stringBuilder.append(CellsHelper.cellIndexToName(area.getStartRow(), area.getStartColumn()));
              if (area.isArea())
              {
                  stringBuilder.append(":");
                  stringBuilder.append(CellsHelper.cellIndexToName(area.getEndRow(), area.getEndColumn()));
              }
              System.out.println(stringBuilder.toString());
         }
```

**Returns:**
[ReferredAreaCollection](../../com.aspose.cells/referredareacollection) - Collection of all references appearing in this cell's formula.
### getPrecedentsInCalculation() {#getPrecedentsInCalculation--}
```
public Iterator getPrecedentsInCalculation()
```


يحصل على جميع السلف (إشارة إلى خلايا في المصنف الحالي) المستخدمة في صيغة هذه الخلية أثناء حسابها.

**Remarks**

يمكن لهذه الطريقة العمل فقط عندما تكون [FormulaSettings.getEnableCalculationChain()](../../com.aspose.cells/formulasettings\#getEnableCalculationChain--) صحيحة للمصنف وقد تم حساب المصنف بالكامل. إذا لم تكن هذه الخلية صيغة أو لم تُشير إلى أي خلايا أخرى، سيتم إرجاع null.

**Example**

```
         Workbook workbook = new Workbook();
         Cells cells = workbook.getWorksheets().get(0).getCells();
         cells.get("A2").setFormula("=IF(TRUE,B2,B1)");
         workbook.getSettings().getFormulaSettings().setEnableCalculationChain(true);
         workbook.calculateFormula();
         Iterator en = cells.get("A2").getPrecedentsInCalculation();
         System.out.println("A2's calculation precedents:");
         while(en.hasNext())
         {
             ReferredArea r = (ReferredArea)en.next();
             System.out.println(r);
         }
```

**Returns:**
java.util.Iterator - مُعدد لتعداد جميع المراجع (ReferredArea)
### getR1C1Formula() {#getR1C1Formula--}
```
public String getR1C1Formula()
```


يحصل على صيغة R1C1 للـ [Cell](../../com.aspose.cells/cell).

**Returns:**
java.lang.String
### getRichValue() {#getRichValue--}
```
public CellRichValue getRichValue()
```


يحصل على القيمة الغنية للخلية.

**Returns:**
[CellRichValue](../../com.aspose.cells/cellrichvalue)
### getRow() {#getRow--}
```
public int getRow()
```


يحصل على رقم الصف (مبني على الصفر) للخلية.

**Returns:**
int
### getSharedStyleIndex() {#getSharedStyleIndex--}
```
public int getSharedStyleIndex()
```


يحصل على فهرس النمط المشترك للخلية في مجموعة الأنماط.

**Returns:**
int
### getStringValue() {#getStringValue--}
```
public String getStringValue()
```


يحصل على القيمة النصية الموجودة في الخلية. إذا كان نوع هذه الخلية نصًا، فسيتم إرجاع القيمة النصية نفسها. بالنسبة لأنواع الخلايا الأخرى، سيتم إرجاع القيمة النصية المُنسقة (المُنسقة بالنمط المحدد لهذه الخلية). القيمة النصية المُنسقة للخلية هي نفسها ما يمكنك الحصول عليه من Excel عند نسخ خلية كنص (مثل نسخ الخلية إلى محرر نصوص أو تصدير إلى CSV).

**Returns:**
java.lang.String
### getStringValue(int formatStrategy) {#getStringValue-int-}
```
public String getStringValue(int formatStrategy)
```


يحصل على القيمة النصية وفق استراتيجية تنسيق محددة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| formatStrategy | int | [CellValueFormatStrategy](../../com.aspose.cells/cellvalueformatstrategy). الإستراتيجية المُنسقة. |

**Returns:**
java.lang.String -
### getStringValueWithoutFormat() {#getStringValueWithoutFormat--}
```
public String getStringValueWithoutFormat()
```


يحصل على قيمة الخلية كنص دون أي تنسيق.

**Remarks**

ملاحظة: هذه الطريقة الآن مهجورة. بدلاً من ذلك، يجب على المستخدم الحصول على كائن القيمة وتنسيقه وفقًا لنوع القيمة والمتطلبات المحددة. سيتم إزالة هذه الخاصية بعد 12 شهرًا منذ ديسمبر 2020. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

**Returns:**
java.lang.String
### getStyle() {#getStyle--}
```
public Style getStyle()
```


يحصل على نمط الخلية.

**Remarks**

لتغيير نمط الخلية، يرجى استدعاء طريقة Cell.SetStyle() بعد تعديل كائن النمط المرجع. هذه الطريقة هي نفسها مع [getStyle(boolean)](../../com.aspose.cells/cell\#getStyle-boolean-) مع قيمة true للمعامل.

**Returns:**
[Style](../../com.aspose.cells/style) - Style object.
### getStyle(boolean checkBorders) {#getStyle-boolean-}
```
public Style getStyle(boolean checkBorders)
```


إذا كان checkBorders صحيحًا، تحقق مما إذا كانت حدود الخلايا الأخرى ستؤثر على نمط هذه الخلية.

**Remarks**

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| checkBorders | boolean | تحقق من حدود الخلايا الأخرى |

**Returns:**
[Style](../../com.aspose.cells/style) - Style object.
### getTable() {#getTable--}
```
public ListObject getTable()
```


يحصل على الجدول الذي يحتوي على هذه الخلية.

**Returns:**
[ListObject](../../com.aspose.cells/listobject) - 
### getType() {#getType--}
```
public int getType()
```


يمثل نوع قيمة الخلية.

انظر [CellValueType](../../com.aspose.cells/cellvaluetype).

**Returns:**
int
### getValidation() {#getValidation--}
```
public Validation getValidation()
```


يحصل على التحقق المطبق على هذه الخلية.

**Returns:**
[Validation](../../com.aspose.cells/validation) - 
### getValidationValue() {#getValidationValue--}
```
public boolean getValidationValue()
```


يحصل على قيمة التحقق المطبق على هذه الخلية.

**Returns:**
boolean -
### getValue() {#getValue--}
```
public Object getValue()
```


يحصل على القيمة الموجودة في هذه الخلية.

**Remarks**

النوع المحتمل:

null,

Boolean,

DateTime,

Double,

Integer

String.

بالنسبة لقيمة int، قد يتم إرجاعها ككائن Integer أو ككائن Double. ولا توجد أي ضمانات بأن القيمة المرجعة ستظل من نفس نوع الكائن دائمًا.

**Returns:**
java.lang.Object
### getWidthOfValue() {#getWidthOfValue--}
```
public int getWidthOfValue()
```


يحصل على عرض القيمة بوحدة البكسل.

**Returns:**
int -
### getWorksheet() {#getWorksheet--}
```
public Worksheet getWorksheet()
```


يحصل على ورقة العمل الأصلية.

**Returns:**
[Worksheet](../../com.aspose.cells/worksheet)
### hasCustomFunction() {#hasCustomFunction--}
```
public boolean hasCustomFunction()
```


يتحقق مما إذا كان هناك دالة مخصصة (دالة غير مدعومة) في صيغة هذه الخلية.

**Returns:**
boolean
### hasCustomStyle() {#hasCustomStyle--}
```
public boolean hasCustomStyle()
```


يشير إلى ما إذا كانت هذه الخلية لديها إعدادات نمط مخصصة (مختلفة عن الإعداد الافتراضي الموروث من الصف أو العمود أو المصنف المقابل).

**Returns:**
boolean
### hashCode() {#hashCode--}
```
public int hashCode()
```


يعمل كدالة تجزئة لنوع معين.

**Returns:**
int - رمز تجزئة لكائن Cell الحالي.
### insertText(int index, String text) {#insertText-int-java.lang.String-}
```
public void insertText(int index, String text)
```


إدراج بعض الأحرف إلى الخلية. إذا كانت الخلية منسقة بشكل غني، يمكن لهذه الطريقة الحفاظ على التنسيق الأصلي.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| الفهرس | int | الفهرس. |
| نص | java.lang.String | النص المُدرج. |

### isArrayFormula() {#isArrayFormula--}
```
public boolean isArrayFormula()
```


يشير إلى ما إذا كانت صيغة الخلية صيغة مصفوفة.

**Returns:**
boolean
### isArrayHeader() {#isArrayHeader--}
```
public boolean isArrayHeader()
```


يشير إلى أن صيغة الخلية هي صيغة مصفوفة وأنها الخلية الأولى في المصفوفة.

**Returns:**
boolean
### isCheckBoxStyle() {#isCheckBoxStyle--}
```
public boolean isCheckBoxStyle()
```


يشير إلى ما إذا تم تعيين هذه الخلية كمربع اختيار.

**Returns:**
boolean
### isDynamicArrayFormula() {#isDynamicArrayFormula--}
```
public boolean isDynamicArrayFormula()
```


يشير إلى ما إذا كانت صيغة الخلية صيغة مصفوفة ديناميكية (true) أو صيغة مصفوفة قديمة (false).

**Returns:**
boolean
### isErrorValue() {#isErrorValue--}
```
public boolean isErrorValue()
```


يتحقق مما إذا كانت قيمة هذه الخلية خطأ.

**Remarks**

ينطبق أيضًا على خلية الصيغة للتحقق مما إذا كانت النتيجة المحسوبة خطأ.

**Returns:**
boolean
### isFormula() {#isFormula--}
```
public boolean isFormula()
```


يمثل ما إذا كانت الخلية المحددة تحتوي على صيغة.

**Returns:**
boolean
### isInArray() {#isInArray--}
```
public boolean isInArray()
```


يشير إلى ما إذا كانت صيغة الخلية صيغة مصفوفة.

**Remarks**

ملاحظة: هذه الفئة الآن مهجورة. بدلاً من ذلك، يرجى استخدام Cell.IsArrayFormula للتحقق مما إذا كانت صيغة الخلية هي صيغة مصفوفة. سيتم إزالة هذه الخاصية بعد 12 شهرًا منذ مايو 2018. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

**Returns:**
boolean
### isInTable() {#isInTable--}
```
public boolean isInTable()
```


يشير إلى ما إذا كانت هذه الخلية جزءًا من صيغة جدول.

**Remarks**

ملاحظة: هذه الفئة الآن مهجورة. بدلاً من ذلك، يرجى استخدام Cell.IsTableFormula للتحقق مما إذا كانت صيغة الخلية جزءًا من صيغة جدول. سيتم إزالة هذه الخاصية بعد 12 شهرًا منذ مايو 2018. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

**Returns:**
boolean
### isMerged() {#isMerged--}
```
public boolean isMerged()
```


يتحقق مما إذا كانت الخلية جزءًا من نطاق مدمج أم لا.

**Returns:**
boolean
### isNumericValue() {#isNumericValue--}
```
public boolean isNumericValue()
```


يشير إلى ما إذا كانت قيمة هذه الخلية رقمية (int، double و datetime).

**Remarks**

ينطبق أيضًا على خلية الصيغة للتحقق من النتيجة المحسوبة

**Returns:**
boolean
### isRichText() {#isRichText--}
```
public boolean isRichText()
```


يشير إلى ما إذا كانت القيمة النصية لهذه الخلية نصًا منسقًا غنيًا.

**Returns:**
boolean
### isSharedFormula() {#isSharedFormula--}
```
public boolean isSharedFormula()
```


يشير إلى ما إذا كانت صيغة الخلية جزءًا من صيغة مشتركة.

**Returns:**
boolean
### isStyleSet() {#isStyleSet--}
```
public boolean isStyleSet()
```


يشير إلى ما إذا كان نمط الخلية مضبوطًا. إذا تم إرجاع false، فهذا يعني أن هذه الخلية لها تنسيق خلية افتراضي.

**Returns:**
boolean
### isTableFormula() {#isTableFormula--}
```
public boolean isTableFormula()
```


يشير إلى ما إذا كانت هذه الخلية جزءًا من صيغة جدول.

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




### putValue(boolean boolValue) {#putValue-boolean-}
```
public void putValue(boolean boolValue)
```


يضع قيمة منطقية في الخلية.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| boolValue | boolean |  |

### putValue(DateTime dateTime) {#putValue-com.aspose.cells.DateTime-}
```
public void putValue(DateTime dateTime)
```


يضع قيمة تاريخ/وقت في الخلية.

**Remarks**

تعيين قيمة DateTime لخلية لا يعني أن الخلية سيتم تنسيقها كوقت وتاريخ تلقائيًا. تُحفظ قيمة DateTime كقيمة رقمية في نموذج البيانات لكل من MS Excel و Aspose.Cells. ما إذا كانت القيمة الرقمية ستُعامل كقيمة رقمية نفسها أو كوقت وتاريخ يعتمد على تنسيق الأرقام المطبق على هذه الخلية. إذا لم يتم تنسيق هذه الخلية كوقت وتاريخ، فستُعرض كقيمة رقمية حتى وإن كان الإدخال هو DateTime.

**Example**

يوضح هذا المثال كيفية تعيين قيمة DateTime لخلية وجعلها تُعرض كوقت وتاريخ.

```
         Workbook excel = new Workbook();
         Cells cells = excel.getWorksheets().get(0).getCells();
 
         //Put date time into a cell
         Cell cell = cells.get(0, 0);
         cell.putValue(new DateTime(2023, 5, 15));
         Style style = cell.getStyle(false);
         style.setNumber(14);
         cell.setStyle(style);
```

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| dateTime | [DateTime](../../com.aspose.cells/datetime) | قيمة الإدخال |

### putValue(double doubleValue) {#putValue-double-}
```
public void putValue(double doubleValue)
```


يضع قيمة مزدوجة في الخلية.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| doubleValue | double | قيمة الإدخال |

### putValue(int intValue) {#putValue-int-}
```
public void putValue(int intValue)
```


يضع قيمة صحيحة في الخلية.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| intValue | int | قيمة الإدخال |

### putValue(Object objectValue) {#putValue-java.lang.Object-}
```
public void putValue(Object objectValue)
```


يضع قيمة كائن في الخلية.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| objectValue | java.lang.Object | قيمة الإدخال |

### putValue(String stringValue) {#putValue-java.lang.String-}
```
public void putValue(String stringValue)
```


يضع قيمة نصية في الخلية.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| stringValue | java.lang.String | قيمة الإدخال |

### putValue(String stringValue, boolean isConverted) {#putValue-java.lang.String-boolean-}
```
public void putValue(String stringValue, boolean isConverted)
```


يضع قيمة نصية في الخلية ويحول القيمة إلى نوع بيانات آخر إذا كان ذلك مناسبًا.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| stringValue | java.lang.String | قيمة الإدخال |
| isConverted | boolean | True: تم التحويل إلى نوع بيانات آخر إذا كان مناسبًا. |

### putValue(String stringValue, boolean isConverted, boolean setStyle) {#putValue-java.lang.String-boolean-boolean-}
```
public void putValue(String stringValue, boolean isConverted, boolean setStyle)
```


يضع قيمة في الخلية، وإذا كان مناسبًا سيتم تحويل القيمة إلى نوع بيانات آخر وسيتم إعادة تعيين تنسيق الأرقام للخلية.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| stringValue | java.lang.String | قيمة الإدخال |
| isConverted | boolean | True: تم التحويل إلى نوع بيانات آخر إذا كان مناسبًا. |
| setStyle | boolean | True: ضبط تنسيق الرقم على نمط الخلية عند التحويل إلى نوع بيانات آخر |

### removeArrayFormula(boolean leaveNormalFormula) {#removeArrayFormula-boolean-}
```
public void removeArrayFormula(boolean leaveNormalFormula)
```


إزالة صيغة المصفوفة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| leaveNormalFormula | boolean | True تمثّل تحويل الصيغة المصفوفية إلى صيغة عادية. |

### replace(String placeHolder, String newValue, ReplaceOptions options) {#replace-java.lang.String-java.lang.String-com.aspose.cells.ReplaceOptions-}
```
public void replace(String placeHolder, String newValue, ReplaceOptions options)
```


استبدال نص الخلية بالخيارات.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| placeHolder | java.lang.String | عنصر نائب للخلية |
| newValue | java.lang.String | قيمة سلسلة للاستبدال |
| options | [ReplaceOptions](../../com.aspose.cells/replaceoptions) | خيارات الاستبدال |

### setArrayFormula(String arrayFormula, int rowNumber, int columnNumber) {#setArrayFormula-java.lang.String-int-int-}
```
public void setArrayFormula(String arrayFormula, int rowNumber, int columnNumber)
```


يضبط صيغة مصفوفة (صيغة مصفوفة قديمة تُدخل عبر CTRL+SHIFT+ENTER في MS Excel) لنطاق من الخلايا.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| arrayFormula | java.lang.String | صيغة مصفوفة. |
| rowNumber | int | عدد الصفوف لملء نتيجة الصيغة المصفوفية. |
| columnNumber | int | عدد الأعمدة لملء نتيجة صيغة المصفوفة. |

### setArrayFormula(String arrayFormula, int rowNumber, int columnNumber, boolean isR1C1, boolean isLocal) {#setArrayFormula-java.lang.String-int-int-boolean-boolean-}
```
public void setArrayFormula(String arrayFormula, int rowNumber, int columnNumber, boolean isR1C1, boolean isLocal)
```


يضبط صيغة مصفوفة لنطاق من الخلايا.

**Remarks**

ملاحظة: هذه الفئة أصبحت الآن مهجورة. بدلاً من ذلك، يرجى استخدام Cell.SetArrayFormula(string,int,int,FormulaParseOptions). سيتم إزالة هذه الخاصية بعد 12 شهرًا منذ ديسمبر 2019. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| arrayFormula | java.lang.String | صيغة مصفوفة. |
| rowNumber | int | عدد الصفوف لملء نتيجة الصيغة المصفوفية. |
| columnNumber | int | عدد الأعمدة لملء نتيجة صيغة المصفوفة. |
| isR1C1 | boolean | ما إذا كانت الصيغة بصيغة R1C1 |
| isLocal | boolean | ما إذا كانت الصيغة مهيأة وفقًا للمنطقة |

### setArrayFormula(String arrayFormula, int rowNumber, int columnNumber, FormulaParseOptions options) {#setArrayFormula-java.lang.String-int-int-com.aspose.cells.FormulaParseOptions-}
```
public void setArrayFormula(String arrayFormula, int rowNumber, int columnNumber, FormulaParseOptions options)
```


يضبط صيغة مصفوفة لنطاق من الخلايا.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| arrayFormula | java.lang.String | صيغة مصفوفة. |
| rowNumber | int | عدد الصفوف لملء نتيجة الصيغة المصفوفية. |
| columnNumber | int | عدد الأعمدة لملء نتيجة صيغة المصفوفة. |
| options | [FormulaParseOptions](../../com.aspose.cells/formulaparseoptions) | خيارات تحليل الصيغة. |

### setArrayFormula(String arrayFormula, int rowNumber, int columnNumber, FormulaParseOptions options, Object[][] values) {#setArrayFormula-java.lang.String-int-int-com.aspose.cells.FormulaParseOptions-java.lang.Object-----}
```
public void setArrayFormula(String arrayFormula, int rowNumber, int columnNumber, FormulaParseOptions options, Object[][] values)
```


يضبط صيغة مصفوفة لنطاق من الخلايا.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| arrayFormula | java.lang.String | صيغة مصفوفة. |
| rowNumber | int | عدد الصفوف لملء نتيجة الصيغة المصفوفية. |
| columnNumber | int | عدد الأعمدة لملء نتيجة صيغة المصفوفة. |
| options | [FormulaParseOptions](../../com.aspose.cells/formulaparseoptions) | خيارات تحليل الصيغة. |
| values | java.lang.Object[][] | القيم لتلك الخلايا التي لها صيغة مصفوفة معينة |

### setCharacters(FontSetting[] characters) {#setCharacters-com.aspose.cells.FontSetting---}
```
public void setCharacters(FontSetting[] characters)
```


يضبط تنسيق النص الغني للخلية.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| characters | [FontSetting\[\]](../../com.aspose.cells/fontsetting) | جميع كائنات Characters. |

### setCheckBoxStyle(boolean value) {#setCheckBoxStyle-boolean-}
```
public void setCheckBoxStyle(boolean value)
```


يشير إلى ما إذا تم تعيين هذه الخلية كمربع اختيار.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setDynamicArrayFormula(String arrayFormula, FormulaParseOptions options, boolean calculateValue) {#setDynamicArrayFormula-java.lang.String-com.aspose.cells.FormulaParseOptions-boolean-}
```
public CellArea setDynamicArrayFormula(String arrayFormula, FormulaParseOptions options, boolean calculateValue)
```


يضبط صيغة مصفوفة ديناميكية ويجعل الصيغة تمتد إلى الخلايا المجاورة إذا كان ذلك ممكنًا.

**Remarks**

قد لا يكون النطاق المعاد هو نفسه النطاق الفعلي الذي تتسرب إليه هذه الصيغة الديناميكية للمصفوفة. إذا كان هناك خلايا غير فارغة في النطاق، سيتم تعيين الصيغة للخلية الحالية فقط وتحديدها كـ \"\\#SPILL!\". ولكن في مثل هذه الحالة ما زلنا نعيد النطاق الكامل الذي يجب أن تتسرب إليه هذه الصيغة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| arrayFormula | java.lang.String | تعبير الصيغة |
| options | [FormulaParseOptions](../../com.aspose.cells/formulaparseoptions) | خيارات تحليل الصيغة. سيتم تجاهل خيار \"Parse\" وستتم دائمًا معالجة الصيغة على الفور |
| calculateValue | boolean | ما إذا كان سيتم حساب هذه الصيغة الديناميكية للمصفوفة لتلك الخلايا في النطاق المتسرب. |

**Returns:**
[CellArea](../../com.aspose.cells/cellarea) - the range that the formula should spill into.
### setDynamicArrayFormula(String arrayFormula, FormulaParseOptions options, Object[][] values, boolean calculateRange, boolean calculateValue) {#setDynamicArrayFormula-java.lang.String-com.aspose.cells.FormulaParseOptions-java.lang.Object-----boolean-boolean-}
```
public CellArea setDynamicArrayFormula(String arrayFormula, FormulaParseOptions options, Object[][] values, boolean calculateRange, boolean calculateValue)
```


يضبط صيغة مصفوفة ديناميكية ويجعل الصيغة تمتد إلى الخلايا المجاورة إذا كان ذلك ممكنًا.

**Remarks**

قد لا يكون النطاق المعاد هو نفسه النطاق الفعلي الذي تتسرب إليه هذه الصيغة الديناميكية للمصفوفة. إذا كان هناك خلايا غير فارغة في النطاق، سيتم تعيين الصيغة للخلية الحالية فقط وتحديدها كـ \"\\#SPILL!\". ولكن في مثل هذه الحالة ما زلنا نعيد النطاق الكامل الذي يجب أن تتسرب إليه هذه الصيغة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| arrayFormula | java.lang.String | تعبير الصيغة |
| options | [FormulaParseOptions](../../com.aspose.cells/formulaparseoptions) | خيارات تحليل الصيغة. سيتم تجاهل خيار \"Parse\" وستتم دائمًا معالجة الصيغة على الفور |
| values | java.lang.Object[][] | القيم (النتائج المحسوبة) لتلك الخلايا التي لها صيغة مصفوفة ديناميكية معينة |
| calculateRange | boolean | ما إذا كان سيتم حساب النطاق المتسرب لهذه الصيغة الديناميكية للمصفوفة. إذا لم يكن معامل \"values\" فارغًا وكان هذا العلم false، فسيكون ارتفاع النطاق المتسرب هو values.Length وعرضه هو values[0].Length. |
| calculateValue | boolean | ما إذا كان سيتم حساب هذه الصيغة الديناميكية للمصفوفة لتلك الخلايا في النطاق المتسرب عندما يكون \"values\" فارغًا أو يكون العنصر المقابل في \"values\" لخلية واحدة فارغًا. |

**Returns:**
[CellArea](../../com.aspose.cells/cellarea) - the range that the formula should spill into.
### setDynamicArrayFormula(String arrayFormula, FormulaParseOptions options, Object[][] values, boolean calculateRange, boolean calculateValue, CalculationOptions copts) {#setDynamicArrayFormula-java.lang.String-com.aspose.cells.FormulaParseOptions-java.lang.Object-----boolean-boolean-com.aspose.cells.CalculationOptions-}
```
public CellArea setDynamicArrayFormula(String arrayFormula, FormulaParseOptions options, Object[][] values, boolean calculateRange, boolean calculateValue, CalculationOptions copts)
```


يضبط صيغة مصفوفة ديناميكية ويجعل الصيغة تمتد إلى الخلايا المجاورة إذا كان ذلك ممكنًا.

**Remarks**

قد لا يكون النطاق المعاد هو نفسه النطاق الفعلي الذي تتسرب إليه هذه الصيغة الديناميكية للمصفوفة. إذا كان هناك خلايا غير فارغة في النطاق، سيتم تعيين الصيغة للخلية الحالية فقط وتحديدها كـ \"\\#SPILL!\". ولكن في مثل هذه الحالة ما زلنا نعيد النطاق الكامل الذي يجب أن تتسرب إليه هذه الصيغة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| arrayFormula | java.lang.String | تعبير الصيغة |
| options | [FormulaParseOptions](../../com.aspose.cells/formulaparseoptions) | خيارات تحليل الصيغة. سيتم تجاهل خيار \"Parse\" وستتم دائمًا معالجة الصيغة على الفور |
| values | java.lang.Object[][] | القيم (النتائج المحسوبة) لتلك الخلايا التي لها صيغة مصفوفة ديناميكية معينة |
| calculateRange | boolean | ما إذا كان سيتم حساب النطاق المتسرب لهذه الصيغة الديناميكية للمصفوفة. إذا لم يكن معامل \"values\" فارغًا وكان هذا العلم false، فسيكون ارتفاع النطاق المتسرب هو values.Length وعرضه هو values[0].Length. |
| calculateValue | boolean | ما إذا كان سيتم حساب هذه الصيغة الديناميكية للمصفوفة لتلك الخلايا في النطاق المتسرب عندما يكون \"values\" فارغًا أو يكون العنصر المقابل في \"values\" لخلية واحدة فارغًا. |
| copts | [CalculationOptions](../../com.aspose.cells/calculationoptions) | الخيارات لحساب الصيغة. عادةً، لأسباب تتعلق بالأداء، يجب أن تكون الخاصية [CalculationOptions.getRecursive()](../../com.aspose.cells/calculationoptions\\#getRecursive--) هي false. |

**Returns:**
[CellArea](../../com.aspose.cells/cellarea) - the range that the formula should spill into.
### setEmbeddedImage(byte[] value) {#setEmbeddedImage-byte---}
```
public void setEmbeddedImage(byte[] value)
```


يضبط الصورة المدمجة في الخلية.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | byte[] |  |

### setFormula(String value) {#setFormula-java.lang.String-}
```
public void setFormula(String value)
```


يضبط صيغة الـ[Cell](../../com.aspose.cells/cell).

**Remarks**

دائمًا ما يبدأ نص الصيغة بعلامة مساواة (=). ويرجى دائمًا استخدام الفاصلة (,) كفاصل للمعاملات، مثل "=SUM(A1, E1, H2)".

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

### setFormula(String formula, boolean isR1C1, boolean isLocal, Object value) {#setFormula-java.lang.String-boolean-boolean-java.lang.Object-}
```
public void setFormula(String formula, boolean isR1C1, boolean isLocal, Object value)
```


اضبط الصيغة وقيمة الصيغة.

**Remarks**

ملاحظة: هذه الفئة أصبحت الآن مهجورة. بدلاً من ذلك، يرجى استخدام Cell.SetFormula(string,FormulaParseOptions,object). سيتم إزالة هذه الخاصية بعد 12 شهرًا منذ ديسمبر 2019. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| formula | java.lang.String | الصيغة. |
| isR1C1 | boolean | ما إذا كانت الصيغة من نوع R1C1. |
| isLocal | boolean | ما إذا كانت الصيغة مهيأة وفقًا للمنطقة. |
| القيمة | java.lang.Object | قيمة الصيغة. |

### setFormula(String formula, FormulaParseOptions options) {#setFormula-java.lang.String-com.aspose.cells.FormulaParseOptions-}
```
public void setFormula(String formula, FormulaParseOptions options)
```


اضبط الصيغة والقيمة (النتيجة المحسوبة) للصيغة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| formula | java.lang.String | الصيغة. |
| options | [FormulaParseOptions](../../com.aspose.cells/formulaparseoptions) | خيارات تحليل الصيغة. |

### setFormula(String formula, FormulaParseOptions options, Object value) {#setFormula-java.lang.String-com.aspose.cells.FormulaParseOptions-java.lang.Object-}
```
public void setFormula(String formula, FormulaParseOptions options, Object value)
```


اضبط الصيغة والقيمة (النتيجة المحسوبة) للصيغة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| formula | java.lang.String | الصيغة. |
| options | [FormulaParseOptions](../../com.aspose.cells/formulaparseoptions) | خيارات تحليل الصيغة. |
| القيمة | java.lang.Object | قيمة الصيغة (النتيجة المحسوبة). |

### setFormula(String formula, Object value) {#setFormula-java.lang.String-java.lang.Object-}
```
public void setFormula(String formula, Object value)
```


اضبط الصيغة والقيمة (النتيجة المحسوبة) للصيغة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| formula | java.lang.String | الصيغة. |
| القيمة | java.lang.Object | قيمة الصيغة (النتيجة المحسوبة). |

### setFormulaLocal(String value) {#setFormulaLocal-java.lang.String-}
```
public void setFormulaLocal(String value)
```


احصل على الصيغة المنسقة حسب اللغة للخلية.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

### setHtmlString(String value) {#setHtmlString-java.lang.String-}
```
public void setHtmlString(String value)
```


يضبط سلسلة HTML التي تحتوي على بيانات وبعض التنسيقات في هذه الخلية.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

### setR1C1Formula(String value) {#setR1C1Formula-java.lang.String-}
```
public void setR1C1Formula(String value)
```


يضبط صيغة R1C1 للـ[Cell](../../com.aspose.cells/cell).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

### setSharedFormula(String sharedFormula, int rowNumber, int columnNumber) {#setSharedFormula-java.lang.String-int-int-}
```
public void setSharedFormula(String sharedFormula, int rowNumber, int columnNumber)
```


يضبط صيغًا مشتركة لنطاق من الخلايا.

**Remarks**

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| sharedFormula | java.lang.String | صيغة مشتركة. |
| rowNumber | int | عدد الصفوف لتعبئة الصيغة. |
| columnNumber | int | عدد الأعمدة لتعبئة الصيغة. |

### setSharedFormula(String sharedFormula, int rowNumber, int columnNumber, boolean isR1C1, boolean isLocal) {#setSharedFormula-java.lang.String-int-int-boolean-boolean-}
```
public void setSharedFormula(String sharedFormula, int rowNumber, int columnNumber, boolean isR1C1, boolean isLocal)
```


يضبط صيغة لنطاق من الخلايا.

**Remarks**

ملاحظة: هذه الفئة أصبحت الآن مهجورة. بدلاً من ذلك، يرجى استخدام Cell.SetSharedFormula(string,int,int,FormulaParseOptions). سيتم إزالة هذه الخاصية بعد 12 شهرًا منذ ديسمبر 2019. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| sharedFormula | java.lang.String | صيغة مشتركة. |
| rowNumber | int | عدد الصفوف لتعبئة الصيغة. |
| columnNumber | int | عدد الأعمدة لتعبئة الصيغة. |
| isR1C1 | boolean | ما إذا كانت الصيغة بصيغة R1C1 |
| isLocal | boolean | ما إذا كانت الصيغة مهيأة وفقًا للمنطقة |

### setSharedFormula(String sharedFormula, int rowNumber, int columnNumber, FormulaParseOptions options) {#setSharedFormula-java.lang.String-int-int-com.aspose.cells.FormulaParseOptions-}
```
public void setSharedFormula(String sharedFormula, int rowNumber, int columnNumber, FormulaParseOptions options)
```


يضبط صيغًا مشتركة لنطاق من الخلايا.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| sharedFormula | java.lang.String | صيغة مشتركة. |
| rowNumber | int | عدد الصفوف لتعبئة الصيغة. |
| columnNumber | int | عدد الأعمدة لتعبئة الصيغة. |
| options | [FormulaParseOptions](../../com.aspose.cells/formulaparseoptions) | خيارات تحليل الصيغة. |

### setSharedFormula(String sharedFormula, int rowNumber, int columnNumber, FormulaParseOptions options, Object[][] values) {#setSharedFormula-java.lang.String-int-int-com.aspose.cells.FormulaParseOptions-java.lang.Object-----}
```
public void setSharedFormula(String sharedFormula, int rowNumber, int columnNumber, FormulaParseOptions options, Object[][] values)
```


يضبط صيغًا مشتركة لنطاق من الخلايا.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| sharedFormula | java.lang.String | صيغة مشتركة. |
| rowNumber | int | عدد الصفوف لتعبئة الصيغة. |
| columnNumber | int | عدد الأعمدة لتعبئة الصيغة. |
| options | [FormulaParseOptions](../../com.aspose.cells/formulaparseoptions) | خيارات تحليل الصيغة. |
| values | java.lang.Object[][] | القيم لتلك الخلايا ذات الصيغة المشتركة المحددة |

### setStyle(Style style) {#setStyle-com.aspose.cells.Style-}
```
public void setStyle(Style style)
```


يضبط نمط الخلية.

**Remarks**

إذا تم تغيير إعدادات الحدود، سيتم تحديث حدود الخلايا المعدلة أيضًا.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| style | [Style](../../com.aspose.cells/style) | نمط الخلية. |

### setStyle(Style style, boolean explicitFlag) {#setStyle-com.aspose.cells.Style-boolean-}
```
public void setStyle(Style style, boolean explicitFlag)
```


تطبيق الخاصية المعدلة للنمط على الخلية.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| style | [Style](../../com.aspose.cells/style) | نمط الخلية. |
| explicitFlag | boolean | صحيح، يتم الكتابة فوق التنسيق فقط إذا تم تعيينه صراحةً. |

### setStyle(Style style, StyleFlag flag) {#setStyle-com.aspose.cells.Style-com.aspose.cells.StyleFlag-}
```
public void setStyle(Style style, StyleFlag flag)
```


تطبيق نمط الخلية بناءً على العلامات.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| style | [Style](../../com.aspose.cells/style) | نمط الخلية. |
| flag | [StyleFlag](../../com.aspose.cells/styleflag) | علامة النمط. |

### setTableFormula(int rowNumber, int columnNumber, int rowIndexOfInputCell, int columnIndexOfInputCell, boolean isRowInput, Object[][] values) {#setTableFormula-int-int-int-int-boolean-java.lang.Object-----}
```
public void setTableFormula(int rowNumber, int columnNumber, int rowIndexOfInputCell, int columnIndexOfInputCell, boolean isRowInput, Object[][] values)
```


إنشاء جدول بيانات بمتغير واحد للنطاق المحدد بدءًا من هذه الخلية.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| rowNumber | int | عدد الصفوف لتعبئة الصيغة. |
| columnNumber | int | عدد الأعمدة لتعبئة الصيغة. |
| rowIndexOfInputCell | int | فهرس الصف للخلية المدخلة |
| columnIndexOfInputCell | int | فهرس العمود للخلية المدخلة |
| isRowInput | boolean | يشير إلى ما إذا كانت الخلية المدخلة خلية صف (true) أو خلية عمود (false). |
| values | java.lang.Object[][] | القيم للخلايا في نطاق صيغة الجدول |

### setTableFormula(int rowNumber, int columnNumber, int rowIndexOfRowInputCell, int columnIndexOfRowInputCell, int rowIndexOfColumnInputCell, int columnIndexOfColumnInputCell, Object[][] values) {#setTableFormula-int-int-int-int-int-int-java.lang.Object-----}
```
public void setTableFormula(int rowNumber, int columnNumber, int rowIndexOfRowInputCell, int columnIndexOfRowInputCell, int rowIndexOfColumnInputCell, int columnIndexOfColumnInputCell, Object[][] values)
```


إنشاء جدول بيانات بمتغيرين للنطاق المحدد بدءًا من هذه الخلية.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| rowNumber | int | عدد الصفوف لتعبئة الصيغة. |
| columnNumber | int | عدد الأعمدة لتعبئة الصيغة. |
| rowIndexOfRowInputCell | int | فهرس الصف للخلية المدخلة للصف |
| columnIndexOfRowInputCell | int | فهرس العمود للخلية المدخلة للصف |
| rowIndexOfColumnInputCell | int | فهرس الصف للخلية المدخلة للعمود |
| columnIndexOfColumnInputCell | int | فهرس العمود للخلية المدخلة للعمود |
| values | java.lang.Object[][] | القيم للخلايا في نطاق صيغة الجدول |

### setTableFormula(int rowNumber, int columnNumber, String inputCell, boolean isRowInput, Object[][] values) {#setTableFormula-int-int-java.lang.String-boolean-java.lang.Object-----}
```
public void setTableFormula(int rowNumber, int columnNumber, String inputCell, boolean isRowInput, Object[][] values)
```


إنشاء جدول بيانات بمتغير واحد للنطاق المحدد بدءًا من هذه الخلية.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| rowNumber | int | عدد الصفوف لتعبئة الصيغة. |
| columnNumber | int | عدد الأعمدة لتعبئة الصيغة. |
| inputCell | java.lang.String | خلية الإدخال |
| isRowInput | boolean | يشير إلى ما إذا كانت الخلية المدخلة خلية صف (true) أو خلية عمود (false). |
| values | java.lang.Object[][] | القيم للخلايا في نطاق صيغة الجدول |

### setTableFormula(int rowNumber, int columnNumber, String rowInputCell, String columnInputCell, Object[][] values) {#setTableFormula-int-int-java.lang.String-java.lang.String-java.lang.Object-----}
```
public void setTableFormula(int rowNumber, int columnNumber, String rowInputCell, String columnInputCell, Object[][] values)
```


إنشاء جدول بيانات بمتغيرين للنطاق المحدد بدءًا من هذه الخلية.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| rowNumber | int | عدد الصفوف لتعبئة الصيغة. |
| columnNumber | int | عدد الأعمدة لتعبئة الصيغة. |
| rowInputCell | java.lang.String | خلية إدخال الصف |
| columnInputCell | java.lang.String | خلية إدخال العمود |
| values | java.lang.Object[][] | القيم للخلايا في نطاق صيغة الجدول |

### setValue(Object value) {#setValue-java.lang.Object-}
```
public void setValue(Object value)
```


يضبط القيمة الموجودة في هذه الخلية.

**Remarks**

النوع المحتمل:

null,

Boolean,

DateTime,

Double,

Integer

String.

بالنسبة لقيمة int، قد يتم إرجاعها ككائن Integer أو ككائن Double. ولا توجد أي ضمانات بأن القيمة المرجعة ستظل من نفس نوع الكائن دائمًا.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.Object |  |

### toJson() {#toJson--}
```
public String toJson()
```


تحويل الـ[Cell](../../com.aspose.cells/cell) إلى بيانات هيكل JSON.

**Returns:**
java.lang.String -
### toString() {#toString--}
```
public String toString()
```


يرجع سلسلة تمثل كائن Cell الحالي.

**Returns:**
java.lang.String -
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

