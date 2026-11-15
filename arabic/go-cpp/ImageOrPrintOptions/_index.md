---
title: "فئة ImageOrPrintOptions"
linktitle: "ImageOrPrintOptions"
second_title: "مرجع API لـ Aspose.Cells for Go عبر C++"
description: "فئة ImageOrPrintOptions. تغلف الكائن الذي يمثل imageorprintoptions في Go."
type: docs
weight: 200
url: /ar/go-cpp/imageorprintoptions/
---

## ImageOrPrintOptions class

يسمح بتحديد الخيارات عند تصيير ورقة العمل إلى صور، طباعة ورقة العمل أو تصيير المخطط إلى صورة.

```go

type ImageOrPrintOptions struct  {
	ptr unsafe.Pointer
}

```
## المُنشئات

| طريقة | الوصف |
| --- | --- |
| [NewImageOrPrintOptions](./newimageorprintoptions/) | منشئ. |

## طرق

| طريقة | الوصف |
| --- | --- |
| [IsNull](./isnull/) | يتحقق مما إذا كان كائن التنفيذ هو nullptr. |
| [SetPrintWithStatusDialog](./setprintwithstatusdialog/) | إذا كان PrintWithStatusDialog = true، سيظهر حوار يعرض حالة الطباعة الحالية. وإلا لن يظهر أي حوار من هذا النوع. |
| [GetPrintWithStatusDialog](./getprintwithstatusdialog/) | إذا كان PrintWithStatusDialog = true، سيظهر حوار يعرض حالة الطباعة الحالية. وإلا لن يظهر أي حوار من هذا النوع. |
| [GetHorizontalResolution](./gethorizontalresolution/) | يحصل أو يضبط الدقة الأفقية للصور المُولدة، بوحدة النقاط في البوصة. |
| [SetHorizontalResolution](./sethorizontalresolution/) | يحصل أو يضبط الدقة الأفقية للصور المُولدة، بوحدة النقاط في البوصة. |
| [GetVerticalResolution](./getverticalresolution/) | يحصل أو يضبط الدقة الرأسية للصور المُولدة، بوحدة النقاط في البوصة. |
| [SetVerticalResolution](./setverticalresolution/) | يحصل أو يضبط الدقة الرأسية للصور المُولدة، بوحدة النقاط في البوصة. |
| [GetTiffCompression](./gettiffcompression/) | يحصل أو يضبط نوع الضغط الذي يُطبق فقط عند حفظ الصفحات بتنسيق <c>Tiff</c>. |
| [SetTiffCompression](./settiffcompression/) | يحصل أو يضبط نوع الضغط الذي يُطبق فقط عند حفظ الصفحات بتنسيق <c>Tiff</c>. |
| [GetTiffColorDepth](./gettiffcolordepth/) | يحصل أو يضبط عمق البت الذي يُطبق فقط عند حفظ الصفحات بتنسيق <c>Tiff</c>. |
| [SetTiffColorDepth](./settiffcolordepth/) | يحصل أو يضبط عمق البت الذي يُطبق فقط عند حفظ الصفحات بتنسيق <c>Tiff</c>. |
| [GetTiffBinarizationMethod](./gettiffbinarizationmethod/) | يحصل أو يضبط الطريقة المستخدمة أثناء تحويل الصور إلى تنسيق 1 bpp عندما يكون ImageType هو Tiff ويكون TiffCompression مساويًا لـ Ccitt3 أو Ccitt4. |
| [SetTiffBinarizationMethod](./settiffbinarizationmethod/) | يحصل أو يضبط الطريقة المستخدمة أثناء تحويل الصور إلى تنسيق 1 bpp عندما يكون ImageType هو Tiff ويكون TiffCompression مساويًا لـ Ccitt3 أو Ccitt4. |
| [GetPrintingPage](./getprintingpage/) | يشير إلى الصفحات التي لن تُطبع. |
| [SetPrintingPage](./setprintingpage/) | يشير إلى الصفحات التي لن تُطبع. |
| [GetQuality](./getquality/) | يحصل أو يضبط قيمة تحدد جودة الصور المُولدة لتُطبق فقط عند حفظ الصفحات بتنسيق <c>Jpeg</c>. القيمة الافتراضية هي 100. |
| [SetQuality](./setquality/) | يحصل أو يضبط قيمة تحدد جودة الصور المُولدة لتُطبق فقط عند حفظ الصفحات بتنسيق <c>Jpeg</c>. القيمة الافتراضية هي 100. |
| [GetOnePagePerSheet](./getonepagepersheet/) | إذا كان OnePagePerSheet يساوي true، سيتم إخراج كل محتوى ورقة واحدة في صفحة واحدة فقط في النتيجة. سيكون حجم الورق في إعدادات الصفحة غير صالح، وستظل الإعدادات الأخرى لإعدادات الصفحة سارية. |
| [SetOnePagePerSheet](./setonepagepersheet/) | إذا كان OnePagePerSheet يساوي true، سيتم إخراج كل محتوى ورقة واحدة في صفحة واحدة فقط في النتيجة. سيكون حجم الورق في إعدادات الصفحة غير صالح، وستظل الإعدادات الأخرى لإعدادات الصفحة سارية. |
| [GetAllColumnsInOnePagePerSheet](./getallcolumnsinonepagepersheet/) | إذا كان AllColumnsInOnePagePerSheet = true، سيتم إخراج جميع محتويات الأعمدة لورقة واحدة في صفحة واحدة فقط في النتيجة. سيكون عرض حجم الورق في إعداد الصفحة غير صالح، وستظل الإعدادات الأخرى لإعداد الصفحة سارية. |
| [SetAllColumnsInOnePagePerSheet](./setallcolumnsinonepagepersheet/) | إذا كان AllColumnsInOnePagePerSheet = true، سيتم إخراج جميع محتويات الأعمدة لورقة واحدة في صفحة واحدة فقط في النتيجة. سيكون عرض حجم الورق في إعداد الصفحة غير صالح، وستظل الإعدادات الأخرى لإعداد الصفحة سارية. |
| [GetDrawObjectEventHandler](./getdrawobjecteventhandler/) | يطبق هذه الواجهة للحصول على DrawObject و Bound عند التصيير. |
| [SetDrawObjectEventHandler](./setdrawobjecteventhandler/) | يطبق هذه الواجهة للحصول على DrawObject و Bound عند التصيير. |
| [GetOnlyArea](./getonlyarea/) | إذا كانت هذه الخاصية صحيحة، سيتم إخراج منطقة واحدة، ولن يُطبق أي مقياس. |
| [SetOnlyArea](./setonlyarea/) | إذا كانت هذه الخاصية صحيحة، سيتم إخراج منطقة واحدة، ولن يُطبق أي مقياس. |
| [GetTransparent](./gettransparent/) | يحدد ما إذا كان خلفية الصورة المُولَّدة يجب أن تكون شفافة. |
| [SetTransparent](./settransparent/) | يحدد ما إذا كان خلفية الصورة المُولَّدة يجب أن تكون شفافة. |
| [SetIsFontSubstitutionCharGranularity](./setisfontsubstitutionchargranularity/) | يشير إلى ما إذا كان يجب استبدال خط الحرف فقط عندما يكون خط الخلية غير متوافق معه. |
| [IsFontSubstitutionCharGranularity](./isfontsubstitutionchargranularity/) | يشير إلى ما إذا كان يجب استبدال خط الحرف فقط عندما يكون خط الخلية غير متوافق معه. |
| [SetPageIndex](./setpageindex/) | يحصل أو يعيّن الفهرس القائم على الصفر للصفحة الأولى التي سيتم حفظها. |
| [GetPageIndex](./getpageindex/) | يحصل أو يعيّن الفهرس القائم على الصفر للصفحة الأولى التي سيتم حفظها. |
| [SetPageCount](./setpagecount/) | يحصل أو يعيّن عدد الصفحات التي سيتم حفظها. |
| [GetPageCount](./getpagecount/) | يحصل أو يعيّن عدد الصفحات التي سيتم حفظها. |
| [SetDesiredSize](./setdesiredsize/) | يضبط العرض والارتفاع المطلوبين للصورة. |
| [IsOptimized](./isoptimized/) | يحدد ما إذا كان يجب تحسين عناصر الإخراج. |
| [SetIsOptimized](./setisoptimized/) | يحدد ما إذا كان يجب تحسين عناصر الإخراج. |
| [GetDefaultFont](./getdefaultfont/) | عند تكون الأحرف في Excel يونيكود ولم يتم تعيين خط صحيح في نمط الخلية، قد تظهر ككتل في ملف pdf أو الصورة. اضبط DefaultFont مثل MingLiu أو MS Gothic لعرض هذه الأحرف. إذا لم يتم تعيين هذه الخاصية، سيستخدم Aspose.Cells الخط الافتراضي للنظام لعرض هذه الأحرف اليونيكود. |
| [SetDefaultFont](./setdefaultfont/) | عند تكون الأحرف في Excel يونيكود ولم يتم تعيين خط صحيح في نمط الخلية، قد تظهر ككتل في ملف pdf أو الصورة. اضبط DefaultFont مثل MingLiu أو MS Gothic لعرض هذه الأحرف. إذا لم يتم تعيين هذه الخاصية، سيستخدم Aspose.Cells الخط الافتراضي للنظام لعرض هذه الأحرف اليونيكود. |
| [GetCheckWorkbookDefaultFont](./getcheckworkbookdefaultfont/) | عند تكون الأحرف في Excel يونيكود ولم يتم تعيين خط صحيح في نمط الخلية، قد تظهر ككتل في ملف pdf أو الصورة. اضبط هذا إلى true لمحاولة استخدام الخط الافتراضي لدفتر العمل لعرض هذه الأحرف أولاً. |
| [SetCheckWorkbookDefaultFont](./setcheckworkbookdefaultfont/) | عند تكون الأحرف في Excel يونيكود ولم يتم تعيين خط صحيح في نمط الخلية، قد تظهر ككتل في ملف pdf أو الصورة. اضبط هذا إلى true لمحاولة استخدام الخط الافتراضي لدفتر العمل لعرض هذه الأحرف أولاً. |
| [GetOutputBlankPageWhenNothingToPrint](./getoutputblankpagewhennothingtoprint/) | يشير إلى ما إذا كان يجب إخراج صفحة فارغة عندما لا يوجد ما للطباعة. |
| [SetOutputBlankPageWhenNothingToPrint](./setoutputblankpagewhennothingtoprint/) | يشير إلى ما إذا كان يجب إخراج صفحة فارغة عندما لا يوجد ما للطباعة. |
| [GetGridlineType](./getgridlinetype/) | يحصل أو يعيّن نوع خطوط الشبكة. |
| [SetGridlineType](./setgridlinetype/) | يحصل أو يعيّن نوع خطوط الشبكة. |
| [GetGridlineColor](./getgridlinecolor/) | يحصل أو يضبط لون خطوط الشبكة. |
| [SetGridlineColor](./setgridlinecolor/) | يحصل أو يضبط لون خطوط الشبكة. |
| [GetTextCrossType](./gettextcrosstype/) | يحصل أو يعيّن نوع عرض النص عندما يكون عرض النص أكبر من عرض الخلية. |
| [SetTextCrossType](./settextcrosstype/) | يحصل أو يعيّن نوع عرض النص عندما يكون عرض النص أكبر من عرض الخلية. |
| [GetDefaultEditLanguage](./getdefaulteditlanguage/) | يحصل أو يعيّن لغة التحرير الافتراضية. |
| [SetDefaultEditLanguage](./setdefaulteditlanguage/) | يحصل أو يعيّن لغة التحرير الافتراضية. |
| [GetSheetSet](./getsheetset/) | يحصل أو يعيّن الأوراق التي سيتم تصييرها. الافتراضي هو جميع الأوراق المرئية في دفتر العمل: Aspose.Cells.Rendering.SheetSet.Visible. |
| [SetSheetSet](./setsheetset/) | يحصل أو يعيّن الأوراق التي سيتم تصييرها. الافتراضي هو جميع الأوراق المرئية في دفتر العمل: Aspose.Cells.Rendering.SheetSet.Visible. |
| [GetEmfRenderSetting](./getemfrendersetting/) | إعداد لتصوير ملفات Emf الميتا في ملف المصدر. |
| [SetEmfRenderSetting](./setemfrendersetting/) | إعداد لتصوير ملفات Emf الميتا في ملف المصدر. |
| [GetCustomRenderSettings](./getcustomrendersettings/) | يحصل أو يعيّن الإعدادات المخصصة أثناء التصيير. |
| [SetCustomRenderSettings](./setcustomrendersettings/) | يحصل أو يعيّن الإعدادات المخصصة أثناء التصيير. |
| [GetImageType](./getimagetype/) | يحصل أو يضبط تنسيق الصور المُولدة. القيمة الافتراضية: PNG. |
| [SetImageType](./setimagetype/) | يحصل أو يضبط تنسيق الصور المُولدة. القيمة الافتراضية: PNG. |
