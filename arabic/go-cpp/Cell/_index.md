---
title: "فئة Cell"
linktitle: "Cell"
second_title: "مرجع API لـ Aspose.Cells for Go عبر C++"
description: "فئة Cell. تغلف الكائن الذي يمثل cell في Go."
type: docs
weight: 200
url: /ar/go-cpp/cell/
---

## Cell class

يغلف الكائن الذي يمثل خلية واحدة في المصنف.

```go

type Cell struct  {
	ptr unsafe.Pointer
}

```
## المُنشئات

| طريقة | الوصف |
| --- | --- |

## طرق

| طريقة | الوصف |
| --- | --- |
| [IsNull](./isnull/) | يتحقق مما إذا كان كائن التنفيذ هو nullptr. |
| [Calculate](./calculate/) | يحسب صيغة الخلية. |
| [GetWorksheet](./getworksheet/) | يحصل على ورقة العمل الأصلية. |
| [PutValue_Bool](./putvalue_bool/) | يضع قيمة منطقية في الخلية. |
| [PutValue_Int](./putvalue_int/) | يضع قيمة عددية صحيحة في الخلية. |
| [PutValue_Double](./putvalue_double/) | يضع قيمة مزدوجة في الخلية. |
| [PutValue_String_Bool_Bool](./putvalue_string_bool_bool/) | يضع قيمة في الخلية، إذا كان مناسبًا سيتم تحويل القيمة إلى نوع بيانات آخر وسيتم إعادة تعيين تنسيق الأرقام للخلية. |
| [PutValue_String_Bool](./putvalue_string_bool/) | يضع قيمة نصية في الخلية ويحول القيمة إلى نوع بيانات آخر إذا كان مناسبًا. |
| [PutValue_String](./putvalue_string/) | يضع قيمة نصية في الخلية. |
| [PutValue_Date](./putvalue_date/) | يضع قيمة تاريخ ووقت في الخلية. |
| [PutValue_Object](./putvalue_object/) | يضع قيمة كائن في الخلية. |
| [GetRow](./getrow/) | يحصل على رقم الصف (مبني على الصفر) للخلية. |
| [GetColumn](./getcolumn/) | يحصل على رقم العمود (مبني على الصفر) للخلية. |
| [IsFormula](./isformula/) | يمثل ما إذا كانت الخلية المحددة تحتوي على صيغة. |
| [GetHasCustomFunction](./gethascustomfunction/) | يتحقق مما إذا كان هناك دالة مخصصة (دالة غير مدعومة) في صيغة هذه الخلية. |
| [GetType](./gettype/) | يمثل نوع قيمة الخلية. |
| [GetName](./getname/) | يحصل على اسم الخلية. |
| [IsErrorValue](./iserrorvalue/) | يتحقق مما إذا كانت قيمة هذه الخلية خطأ. |
| [IsNumericValue](./isnumericvalue/) | يشير إلى ما إذا كانت قيمة هذه الخلية رقمية (int، double و datetime). |
| [GetStringValue_CellValueFormatStrategy](./getstringvalue_cellvalueformatstrategy/) | يحصل على القيمة النصية وفق استراتيجية تنسيق محددة. |
| [GetStringValue](./getstringvalue/) | يحصل على القيمة النصية الموجودة في الخلية. إذا كان نوع هذه الخلية نصًا، فسيتم إرجاع القيمة النصية نفسها. بالنسبة لأنواع الخلايا الأخرى، سيتم إرجاع القيمة النصية المنسقة (منسقة باستخدام النمط المحدد لهذه الخلية). القيمة النصية المنسقة للخلية هي نفسها ما يمكنك الحصول عليه من Excel عند نسخ خلية كنص (مثل نسخ الخلية إلى محرر نصوص أو تصدير إلى CSV). |
| [GetNumberCategoryType](./getnumbercategorytype/) | يمثل نوع الفئة لتنسيق الأرقام في هذه الخلية. |
| [GetDisplayStringValue](./getdisplaystringvalue/) | يحصل على القيمة النصية المنسقة لهذه الخلية وفق نمط عرض الخلية. |
| [GetIntValue](./getintvalue/) | يحصل على القيمة الصحيحة الموجودة في الخلية. |
| [GetDoubleValue](./getdoublevalue/) | يحصل على القيمة المزدوجة الموجودة في الخلية. |
| [GetFloatValue](./getfloatvalue/) | يحصل على القيمة العائمة الموجودة في الخلية. |
| [GetDateTimeValue](./getdatetimevalue/) | يحصل على قيمة DateTime الموجودة في الخلية. |
| [GetBoolValue](./getboolvalue/) | يحصل على القيمة المنطقية الموجودة في الخلية. |
| [GetWidthOfValue](./getwidthofvalue/) | يحصل على عرض القيمة بوحدة البكسل. |
| [GetHeightOfValue](./getheightofvalue/) | يحصل على ارتفاع القيمة بوحدة البكسل. |
| [GetDisplayStyle](./getdisplaystyle/) | يحصل على نمط العرض لهذه الخلية. |
| [GetDisplayStyle_Bool](./getdisplaystyle_bool/) | يحصل على نمط العرض لهذه الخلية. |
| [GetDisplayStyle_BorderType](./getdisplaystyle_bordertype/) | يحصل على نمط العرض لهذه الخلية. |
| [GetFormatConditions](./getformatconditions/) | يحصل على شروط التنسيق التي تُطبق على هذه الخلية. |
| [GetStyle](./getstyle/) | يحصل على نمط الخلية. |
| [GetStyle_Bool](./getstyle_bool/) | إذا كان checkBorders صحيحًا، فتحقق مما إذا كانت حدود الخلايا الأخرى ستؤثر على نمط هذه الخلية. |
| [SetStyle_Style](./setstyle_style/) | يضبط نمط الخلية. |
| [SetStyle_Style_Bool](./setstyle_style_bool/) | تطبيق الخاصية المعدلة للنمط على الخلية. |
| [SetStyle_Style_StyleFlag](./setstyle_style_styleflag/) | تطبيق نمط الخلية بناءً على العلامات. |
| [GetHasCustomStyle](./gethascustomstyle/) | يشير إلى ما إذا كانت هذه الخلية تحتوي على إعدادات نمط مخصصة (مختلفة عن الإعداد الافتراضي الموروث من الصف أو العمود أو المصنف المقابل). |
| [GetSharedStyleIndex](./getsharedstyleindex/) | يحصل على فهرس النمط المشترك للخلية في مجموعة الأنماط. |
| [GetFormula](./getformula/) | يحصل أو يضبط صيغة الخلية. |
| [SetFormula_String](./setformula_string/) | يحصل أو يضبط صيغة الخلية. |
| [GetFormulaLocal](./getformulalocal/) | احصل على الصيغة المهيأة وفقًا للمنطقة للخلية. |
| [SetFormulaLocal](./setformulalocal/) | احصل على الصيغة المهيأة وفقًا للمنطقة للخلية. |
| [GetR1C1Formula](./getr1c1formula/) | يحصل أو يضبط صيغة R1C1 للخلية. |
| [SetR1C1Formula](./setr1c1formula/) | يحصل أو يضبط صيغة R1C1 للخلية. |
| [SetFormula_String_Object](./setformula_string_object/) | اضبط الصيغة والقيمة (النتيجة المحسوبة) للصيغة. |
| [SetFormula_String_FormulaParseOptions](./setformula_string_formulaparseoptions/) | اضبط الصيغة والقيمة (النتيجة المحسوبة) للصيغة. |
| [GetFormula_Bool_Bool](./getformula_bool_bool/) | احصل على صيغة هذه الخلية. |
| [SetFormula_String_FormulaParseOptions_Object](./setformula_string_formulaparseoptions_object/) | اضبط الصيغة والقيمة (النتيجة المحسوبة) للصيغة. |
| [SetArrayFormula_String_Int_Int](./setarrayformula_string_int_int/) | يضبط صيغة مصفوفة (صيغة مصفوفة قديمة تُدخل عبر CTRL+SHIFT+ENTER في MS Excel) لنطاق من الخلايا. |
| [SetArrayFormula_String_Int_Int_FormulaParseOptions](./setarrayformula_string_int_int_formulaparseoptions/) | يضبط صيغة مصفوفة لنطاق من الخلايا. |
| [SetArrayFormula_String_Int_Int_FormulaParseOptions_Object2Array](./setarrayformula_string_int_int_formulaparseoptions_object2array/) | يضبط صيغة مصفوفة لنطاق من الخلايا. |
| [SetSharedFormula_String_Int_Int](./setsharedformula_string_int_int/) | يضبط صيغًا مشتركة لنطاق من الخلايا. |
| [SetSharedFormula_String_Int_Int_FormulaParseOptions](./setsharedformula_string_int_int_formulaparseoptions/) | يضبط صيغًا مشتركة لنطاق من الخلايا. |
| [SetSharedFormula_String_Int_Int_FormulaParseOptions_Object2Array](./setsharedformula_string_int_int_formulaparseoptions_object2array/) | يضبط صيغًا مشتركة لنطاق من الخلايا. |
| [GetContainsExternalLink](./getcontainsexternallink/) | يشير إلى ما إذا كانت هذه الخلية تحتوي على رابط خارجي. ينطبق فقط عندما تكون الخلية خلية صيغة. |
| [GetPrecedents](./getprecedents/) | يحصل على جميع المراجع التي تظهر في صيغة هذه الخلية. |
| [GetDependents](./getdependents/) | احصل على جميع الخلايا التي تشير صيغتها إلى هذه الخلية مباشرة. |
| [GetPrecedentsInCalculation](./getprecedentsincalculation/) | يحصل على جميع السلف (الإشارة إلى خلايا في المصنف الحالي) المستخدمة بواسطة صيغة هذه الخلية أثناء حسابها. |
| [GetDependentsInCalculation](./getdependentsincalculation/) | يحصل على جميع الخلايا التي تعتمد نتيجتها المحسوبة على هذه الخلية. |
| [IsArrayHeader](./isarrayheader/) | يشير إلى أن صيغة الخلية هي صيغة مصفوفة وأنها الخلية الأولى في المصفوفة. |
| [IsDynamicArrayFormula](./isdynamicarrayformula/) | يشير إلى ما إذا كانت صيغة الخلية هي صيغة مصفوفة ديناميكية (true) أو صيغة مصفوفة قديمة (false). |
| [GetArrayRange](./getarrayrange/) | يحصل على نطاق المصفوفة إذا كانت صيغة الخلية هي صيغة مصفوفة. |
| [IsArrayFormula](./isarrayformula/) | يشير إلى ما إذا كانت صيغة الخلية هي صيغة مصفوفة. |
| [IsSharedFormula](./issharedformula/) | يشير إلى ما إذا كانت صيغة الخلية جزءًا من صيغة مشتركة. |
| [IsTableFormula](./istableformula/) | يشير إلى ما إذا كانت هذه الخلية جزءًا من صيغة جدول. |
| [SetDynamicArrayFormula_String_FormulaParseOptions_Bool](./setdynamicarrayformula_string_formulaparseoptions_bool/) | يضبط صيغة مصفوفة ديناميكية ويجعل الصيغة تمتد إلى الخلايا المجاورة إذا كان ذلك ممكنًا. |
| [SetDynamicArrayFormula_String_FormulaParseOptions_Object2Array_Bool_Bool](./setdynamicarrayformula_string_formulaparseoptions_object2array_bool_bool/) | يضبط صيغة مصفوفة ديناميكية ويجعل الصيغة تمتد إلى الخلايا المجاورة إذا كان ذلك ممكنًا. |
| [SetDynamicArrayFormula_String_FormulaParseOptions_Object2Array_Bool_Bool_CalculationOptions](./setdynamicarrayformula_string_formulaparseoptions_object2array_bool_bool_calculationoptions/) | يضبط صيغة مصفوفة ديناميكية ويجعل الصيغة تمتد إلى الخلايا المجاورة إذا كان ذلك ممكنًا. |
| [SetTableFormula_Int_Int_String_String_Object2Array](./settableformula_int_int_string_string_object2array/) | أنشئ جدول بيانات بمتغيرين للنطاق المحدد بدءًا من هذه الخلية. |
| [SetTableFormula_Int_Int_String_Bool_Object2Array](./settableformula_int_int_string_bool_object2array/) | أنشئ جدول بيانات بمتغير واحد للنطاق المحدد بدءًا من هذه الخلية. |
| [SetTableFormula_Int_Int_Int_Int_Int_Int_Object2Array](./settableformula_int_int_int_int_int_int_object2array/) | أنشئ جدول بيانات بمتغيرين للنطاق المحدد بدءًا من هذه الخلية. |
| [SetTableFormula_Int_Int_Int_Int_Bool_Object2Array](./settableformula_int_int_int_int_bool_object2array/) | أنشئ جدول بيانات بمتغير واحد للنطاق المحدد بدءًا من هذه الخلية. |
| [RemoveArrayFormula](./removearrayformula/) | إزالة صيغة المصفوفة. |
| [Copy](./copy/) | ينسخ البيانات من خلية المصدر. |
| [GetValue](./getvalue/) | يحصل/يضبط القيمة الموجودة في هذه الخلية. |
| [SetValue](./setvalue/) | يحصل/يضبط القيمة الموجودة في هذه الخلية. |
| [IsStyleSet](./isstyleset/) | يشير إلى ما إذا كان نمط الخلية مضبوطًا. إذا أعاد false، فهذا يعني أن هذه الخلية لها تنسيق خلية افتراضي. |
| [Characters](./characters/) | يرجع كائن Characters الذي يمثل نطاقًا من الأحرف داخل نص الخلية. |
| [Replace](./replace/) | استبدل نص الخلية باستخدام الخيارات. |
| [InsertText](./inserttext/) | أدخل بعض الأحرف إلى الخلية. إذا كانت الخلية منسقة بنص غني، يمكن لهذه الطريقة الحفاظ على التنسيق الأصلي. |
| [IsRichText](./isrichtext/) | يشير إلى ما إذا كانت القيمة النصية لهذه الخلية نصًا منسقًا بنص غني. |
| [GetCharacters](./getcharacters/) | يرجع جميع كائنات Characters التي تمثل نطاقًا من الأحرف داخل نص الخلية. |
| [GetCharacters_Bool](./getcharacters_bool/) | يرجع جميع كائنات Characters التي تمثل نطاقًا من الأحرف داخل نص الخلية. |
| [SetCharacters](./setcharacters/) | يضبط تنسيق النص الغني للخلية. |
| [IsMerged](./ismerged/) | يتحقق مما إذا كانت الخلية جزءًا من نطاق مدمج أم لا. |
| [GetMergedRange](./getmergedrange/) | يرجع كائن Range الذي يمثل نطاقًا مدمجًا. |
| [GetComment](./getcomment/) | يحصل على تعليق هذه الخلية. |
| [GetHtmlString](./gethtmlstring/) | يحصل ويضبط سلسلة HTML التي تحتوي على البيانات وبعض التنسيقات في هذه الخلية. |
| [SetHtmlString](./sethtmlstring/) | يحصل ويضبط سلسلة HTML التي تحتوي على البيانات وبعض التنسيقات في هذه الخلية. |
| [GetHtmlString_Bool](./gethtmlstring_bool/) | يحصل على سلسلة HTML التي تحتوي على البيانات وبعض التنسيقات في هذه الخلية. |
| [ToString](./tostring/) | يرجع سلسلة تمثل كائن الخلية الحالي. |
| [ToJson](./tojson/) | حوّل الخلية إلى بيانات بنية JSON. |
| [Equals_Object](./equals_object/) | يتحقق مما إذا كان هذا الكائن يشير إلى نفس الخلية مع آخر. |
| [GetHashCode](./gethashcode/) | يعمل كدالة تجزئة لنوع معين. |
| [Equals_Cell](./equals_cell/) | يتحقق مما إذا كان هذا الكائن يشير إلى نفس الخلية مع كائن خلية آخر. |
| [GetConditionalFormattingResult](./getconditionalformattingresult/) | احصل على نتيجة التنسيق الشرطي. |
| [GetValidation](./getvalidation/) | يحصل على التحقق المطبق على هذه الخلية. |
| [GetValidationValue](./getvalidationvalue/) | يحصل على قيمة التحقق التي تم تطبيقها على هذه الخلية. |
| [GetTable](./gettable/) | يحصل على الجدول الذي يحتوي على هذه الخلية. |
| [IsCheckBoxStyle](./ischeckboxstyle/) | يشير إلى ما إذا كان يتم تعيين هذه الخلية كمربع اختيار. |
| [SetIsCheckBoxStyle](./setischeckboxstyle/) | يشير إلى ما إذا كان يتم تعيين هذه الخلية كمربع اختيار. |
| [GetRichValue](./getrichvalue/) | يحصل على القيمة الغنية للخلية. |
| [GetEmbeddedImage](./getembeddedimage/) | يحصل ويضبط الصورة المدمجة في الخلية. |
| [SetEmbeddedImage](./setembeddedimage/) | يحصل ويضبط الصورة المدمجة في الخلية. |
| [GetPicture](./getpicture/) | يحصل على كائن Aspose.Cells.Drawing.Picture لتمثيل الصورة المضمنة في هذه الخلية أو يُعيد null إذا لم توجد صورة مضمَّنة لهذه الخلية. |
|[Dispose](./dispose/) |  | 
