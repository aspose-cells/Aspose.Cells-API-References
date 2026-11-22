---
title: "فئة WebWorksheets"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "فئة Aspose.Cells.GridWeb.Data.WebWorksheets."
type: docs
url: /ar/net/aspose.cells.gridweb.data/webworksheets/
---
## WebWorksheets class

```csharp
[Obsolete("This class is obsolete; use  GridWorksheetCollection instead")]
public class WebWorksheets : ICollection, ISerializable
```

## المنشئات

| الاسم | الوصف |
| --- | --- |
| [WebWorksheets](webworksheets/)(MainWeb, GridWorksheetCollection) |  |

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [ActiveSheet](../../aspose.cells.gridweb.data/webworksheets/activesheet/) { get; } |  |
| [ActiveSheetIndex](../../aspose.cells.gridweb.data/webworksheets/activesheetindex/) { get; set; } |  |
| [Count](../../aspose.cells.gridweb.data/webworksheets/count/) { get; } |  |
| [DefaultFontName](../../aspose.cells.gridweb.data/webworksheets/defaultfontname/) { get; set; } |  |
| [DefaultFontSize](../../aspose.cells.gridweb.data/webworksheets/defaultfontsize/) { get; set; } |  |
| [IsFixedSize](../../aspose.cells.gridweb.data/webworksheets/isfixedsize/) { get; } | يحصل على قيمة تشير إلى ما إذا كانت المجموعة ذات حجم ثابت. |
| [IsReadOnly](../../aspose.cells.gridweb.data/webworksheets/isreadonly/) { get; } | يحصل على قيمة تشير إلى ما إذا كانت IList للقراءة فقط. |
| [IsSynchronized](../../aspose.cells.gridweb.data/webworksheets/issynchronized/) { get; } | يحصل على قيمة تشير إلى ما إذا كان الوصول إلى ICollection متزامنًا (آمن للخيوط). |
| [Item](../../aspose.cells.gridweb.data/webworksheets/item/) { get; } | يحصل على عنصر Worksheet في الفهرس المحدد. (2 مؤشرات) |
| [PivotCaches](../../aspose.cells.gridweb.data/webworksheets/pivotcaches/) { get; } | يحصل على كائن مجموعة PivotCache |
| [PivotTables](../../aspose.cells.gridweb.data/webworksheets/pivottables/) { get; } | يحصل على كائن مجموعة pivotTable. |
| [SyncRoot](../../aspose.cells.gridweb.data/webworksheets/syncroot/) { get; } | يحصل على كائن يمكن استخدامه لمزامنة الوصول إلى ICollection. |

## الطرق

| الاسم | الوصف |
| --- | --- |
| [Add](../../aspose.cells.gridweb.data/webworksheets/add/#add)() | يضيف ورقة عمل إلى المجموعة. |
| [Add](../../aspose.cells.gridweb.data/webworksheets/add/#add_1)(object) | يضيف كائن ورقة. |
| [Add](../../aspose.cells.gridweb.data/webworksheets/add/#add_2)(string) | يضيف ورقة عمل إلى المجموعة. |
| [AddCopy](../../aspose.cells.gridweb.data/webworksheets/addcopy/#addcopy_1)(int) | يضيف ورقة عمل إلى المجموعة وينسخ البيانات من ورقة عمل موجودة. |
| [AddCopy](../../aspose.cells.gridweb.data/webworksheets/addcopy/#addcopy_2)(string) | يضيف ورقة عمل إلى المجموعة وينسخ البيانات من ورقة عمل موجودة. |
| [AddCopy](../../aspose.cells.gridweb.data/webworksheets/addcopy/#addcopy)(WebWorksheet) | يضيف ورقة عمل إلى المجموعة وينسخ البيانات من ورقة عمل موجودة. |
| [Clear](../../aspose.cells.gridweb.data/webworksheets/clear/)() | مسح جميع أوراق العمل. |
| [Contains](../../aspose.cells.gridweb.data/webworksheets/contains/)(object) | يشير إلى ما إذا كانت المجموعة تحتوي على الورقة. |
| [CopyTo](../../aspose.cells.gridweb.data/webworksheets/copyto/)(Array, int) | ينسخ المحتويات إلى مصفوفة. |
| [GetEnumerator](../../aspose.cells.gridweb.data/webworksheets/getenumerator/)() |  |
| [ImportDataView](../../aspose.cells.gridweb.data/webworksheets/importdataview/#importdataview)(DataView, TableItemStyle, TableItemStyle) | يستورد من DataView. ينشئ ورقة باسم جدول DataView تلقائيًا. |
| [ImportDataView](../../aspose.cells.gridweb.data/webworksheets/importdataview/#importdataview_1)(DataView, TableItemStyle, TableItemStyle, string, int, int) | يستورد من DataView إلى الورقة والموقع المحددين. |
| [ImportExcelFile](../../aspose.cells.gridweb.data/webworksheets/importexcelfile/#importexcelfile)(Stream) | يستورد من تدفق ملف Excel، بما في ذلك تدفق ملف على القرص أو تدفق الذاكرة. |
| [ImportExcelFile](../../aspose.cells.gridweb.data/webworksheets/importexcelfile/#importexcelfile_1)(string) | يستورد من ملف Excel. |
| [IndexOf](../../aspose.cells.gridweb.data/webworksheets/indexof/)(object) | يحصل على فهرس الورقة. |
| [Insert](../../aspose.cells.gridweb.data/webworksheets/insert/)(int, string) | يدرج ورقة في الفهرس. |
| [LoadCSVFile](../../aspose.cells.gridweb.data/webworksheets/loadcsvfile/#loadcsvfile)(Stream) | يقوم بتحميل البيانات من تدفق ملف CSV. |
| [LoadCSVFile](../../aspose.cells.gridweb.data/webworksheets/loadcsvfile/#loadcsvfile_1)(string) | يقوم بتحميل البيانات من ملف CSV. |
| [LoadHTMLFile](../../aspose.cells.gridweb.data/webworksheets/loadhtmlfile/#loadhtmlfile)(Stream) | يقوم بتحميل البيانات من تدفق ملف HTML. |
| [LoadHTMLFile](../../aspose.cells.gridweb.data/webworksheets/loadhtmlfile/#loadhtmlfile_1)(string) | يقوم بتحميل البيانات من ملف HTML. |
| [LoadSpreadSheetMLFile](../../aspose.cells.gridweb.data/webworksheets/loadspreadsheetmlfile/#loadspreadsheetmlfile)(Stream) | يقوم بتحميل البيانات من تدفق ملف SpreadSheetML. |
| [LoadSpreadSheetMLFile](../../aspose.cells.gridweb.data/webworksheets/loadspreadsheetmlfile/#loadspreadsheetmlfile_1)(string) | يقوم بتحميل البيانات من ملف SpreadSheetML. |
| [Remove](../../aspose.cells.gridweb.data/webworksheets/remove/)(object) | يزيل ورقة. |
| [RemoveAt](../../aspose.cells.gridweb.data/webworksheets/removeat/#removeat)(int) | يزيل ورقة في الفهرس. |
| [RemoveAt](../../aspose.cells.gridweb.data/webworksheets/removeat/#removeat_1)(string) | يضبط الحجم المعروض عندما يُستخدم ملف دفتر العمل ككائن Ole. |
| [RunAllFormulas](../../aspose.cells.gridweb.data/webworksheets/runallformulas/)() | ينفّذ جميع صيغ الخلايا. |
| [SaveCSVFile](../../aspose.cells.gridweb.data/webworksheets/savecsvfile/#savecsvfile)(Stream) | يحفظ البيانات إلى تدفق ملف CSV. |
| [SaveCSVFile](../../aspose.cells.gridweb.data/webworksheets/savecsvfile/#savecsvfile_1)(string) | يحفظ البيانات إلى ملف CSV. |
| [SaveHTMLFile](../../aspose.cells.gridweb.data/webworksheets/savehtmlfile/#savehtmlfile)(Stream) | يحفظ البيانات إلى تدفق ملف HTML. |
| [SaveHTMLFile](../../aspose.cells.gridweb.data/webworksheets/savehtmlfile/#savehtmlfile_1)(string) | يحفظ البيانات إلى ملف HTML. |
| [SaveSpreadSheetMLFile](../../aspose.cells.gridweb.data/webworksheets/savespreadsheetmlfile/#savespreadsheetmlfile)(Stream) | يحفظ البيانات إلى تدفق ملف SpreadSheetML. |
| [SaveSpreadSheetMLFile](../../aspose.cells.gridweb.data/webworksheets/savespreadsheetmlfile/#savespreadsheetmlfile_1)(string) | يحفظ البيانات إلى ملف SpreadSheetML. |
| [SaveToExcelFile](../../aspose.cells.gridweb.data/webworksheets/savetoexcelfile/#savetoexcelfile)(Stream) | يحفظ أوراق العمل إلى تدفق ملف إكسل، بما في ذلك تدفق إدخال/إخراج القرص أو تدفق الذاكرة. |
| [SaveToExcelFile](../../aspose.cells.gridweb.data/webworksheets/savetoexcelfile/#savetoexcelfile_2)(string) | يحفظ أوراق العمل إلى ملف إكسل بصيغة Excel 2003. |
| [SaveToExcelFile](../../aspose.cells.gridweb.data/webworksheets/savetoexcelfile/#savetoexcelfile_1)(Stream, GridSaveFormat) | يحفظ أوراق العمل إلى ملف إكسل. |
| [SaveToExcelFile](../../aspose.cells.gridweb.data/webworksheets/savetoexcelfile/#savetoexcelfile_3)(string, GridSaveFormat) | يحفظ أوراق العمل إلى ملف إكسل. |

### ملاحظات

ملاحظة: هذه الفئة أصبحت الآن مهجورة. يرجى استخدام GridWorksheetCollection بدلاً منها. سيتم إزالة هذه الفئة بعد 6 أشهر من أغسطس 2014. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

### انظر أيضًا

* namespace [Aspose.Cells.GridWeb.Data](../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../)


