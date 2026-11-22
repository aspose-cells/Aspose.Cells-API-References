---
title: "الفئة GridDesktop"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "فئة Aspose.Cells.GridDesktop.GridDesktop. فئة Aspose GridDesktop تمثل كائنًا أساسيًا لإنشاء عنصر تحكم GridDesktop. لاستخدام هذا العنصر، اسحبّه ببساطة من صندوق الأدوات إلى نموذج أو عنصر تحكم."
type: docs
url: /ar/net/aspose.cells.griddesktop/griddesktop/
---
## GridDesktop class

فئة Aspose GridDesktop تمثل كائنًا جذريًا لإنشاء عنصر تحكم GridDesktop. لاستخدام هذا العنصر، اسحبّه ببساطة من صندوق الأدوات إلى نموذج أو عنصر تحكم مستخدم.

```csharp
public class GridDesktop : UserControl
```

## المنشئات

| الاسم | الوصف |
| --- | --- |
| [GridDesktop](griddesktop/)() | فئة Aspose GridDesktop |

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [ActiveSheetIndex](../../aspose.cells.griddesktop/griddesktop/activesheetindex/) { get; set; } | يحصل أو يعيّن فهرس الورقة المحددة. |
| [ActiveSheetNameFont](../../aspose.cells.griddesktop/griddesktop/activesheetnamefont/) { get; set; } | يحصل أو يعيّن الخط المعروض للورقة النشطة في شريط الورقة. |
| [AlwasysRecalculateAllFormulas](../../aspose.cells.griddesktop/griddesktop/alwasysrecalculateallformulas/) { get; set; } | يحصل أو يعيّن قيمة تشير إلى ما إذا كنا بحاجة إلى تشغيل جميع الصيغ، كما أنه عند تشغيل جميع الصيغ، عند تحديث قيمة خلية واحدة، تؤثر على أخرى، وتؤثر الأخرى على أخرى، وهكذا، مما يجعل جميع الخلايا تحتاج إلى إعادة حساب، تمامًا مثل تأثير الفراشة، يتطلب ذلك الكثير من عمليات المكدس، مما يؤدي إلى أداء منخفض جدًا، كما في CELLSNET-41921، تحتوي هذه المشكلة على الملف الذي يمكنه إظهار هذا السيناريو؛ من الأفضل تشغيل جميع الصيغ فقط، حيث قد يكون هناك بعض التحسينات عند تشغيل جميع الصيغ. |
| [BorderStyle](../../aspose.cells.griddesktop/griddesktop/borderstyle/) { get; set; } | يشير إلى نمط الحدود للعنصر. |
| [ColumnHeaderVisible](../../aspose.cells.griddesktop/griddesktop/columnheadervisible/) { get; set; } | يحصل أو يعيّن قيمة تشير إلى ما إذا كان عنوان العمود مرئيًا. |
| [CommentDisplayingFont](../../aspose.cells.griddesktop/griddesktop/commentdisplayingfont/) { get; set; } | يحصل أو يعيّن الخط الافتراضي لعرض نص التعليق. |
| [ContextMenuManager](../../aspose.cells.griddesktop/griddesktop/contextmenumanager/) { get; } | يحصل على مثيل ContextMenuManager. |
| [DefaultCellFont](../../aspose.cells.griddesktop/griddesktop/defaultcellfont/) { get; set; } | يحصل أو يعيّن الخط الافتراضي للخلية |
| [DefaultCellFontColor](../../aspose.cells.griddesktop/griddesktop/defaultcellfontcolor/) { get; set; } | يحصل أو يعيّن لون الخط الافتراضي للخلية. |
| [EnableClipboardCopyPaste](../../aspose.cells.griddesktop/griddesktop/enableclipboardcopypaste/) { get; set; } | يشير إلى ما إذا كان النسخ/اللصق يعتمد على الحافظة، بحيث يمكن النسخ/اللصق مع MS-EXCEL. ينسخ/يلصق فقط قيمة الخلية، ولا ينسخ أي إعداد آخر للخلية مثل التنسيق، نمط الحدود، وما إلى ذلك. القيمة الافتراضية هي false. |
| [EnableCopyWithExtension](../../aspose.cells.griddesktop/griddesktop/enablecopywithextension/) { get; set; } | يحصل أو يعيّن قيمة تشير إلى ما إذا كانت عملية النسخ ستمدد عدد الصفوف أو الأعمدة. |
| [EnableCopyWithLockedOption](../../aspose.cells.griddesktop/griddesktop/enablecopywithlockedoption/) { get; set; } | يحصل أو يعيّن قيمة تشير إلى ما إذا كانت عملية النسخ ستنسخ قيمة خاصية CellLocked في النمط للخلية. |
| [EnableUndo](../../aspose.cells.griddesktop/griddesktop/enableundo/) { get; set; } | يحصل أو يضبط قيمة تشير إلى ما إذا كانت وظيفة التراجع مفعلة. القيمة الافتراضية هي false. |
| [GridMemorySetting](../../aspose.cells.griddesktop/griddesktop/gridmemorysetting/) { get; set; } | يحصل أو يعيّن خيار الذاكرة، القيمة الافتراضية هي GridMemorySetting.Normal |
| [IsHorizontalScrollBarVisible](../../aspose.cells.griddesktop/griddesktop/ishorizontalscrollbarvisible/) { get; set; } | يضبط حالة الظهور لشريط التمرير الأفقي. |
| [IsVerticalScrollBarVisible](../../aspose.cells.griddesktop/griddesktop/isverticalscrollbarvisible/) { get; set; } | يضبط حالة الظهور لشريط التمرير العمودي. |
| [Names](../../aspose.cells.griddesktop/griddesktop/names/) { get; } | يحصل على مجموعة جميع كائنات Name في جدول البيانات. |
| [PageRows](../../aspose.cells.griddesktop/griddesktop/pagerows/) { get; set; } | يضبط أو يحصل على حجم الصف للـ Pagination. الحد الأقصى لـ PageRows المدعوم هو 100000، والحد الأقصى لعدد الصفحات المدعوم هو 5000. |
| [PasteType](../../aspose.cells.griddesktop/griddesktop/pastetype/) { get; set; } | يشير إلى نوع اللصق عند تنفيذ عملية اللصق، يتوفر فقط عندما تكون EnableClipboardCopyPaste غير مفعلة. القيمة الافتراضية هي GridPasteType.Default؛ |
| [R1C1](../../aspose.cells.griddesktop/griddesktop/r1c1/) { get; set; } | يحصل أو يعيّن قيمة تشير إلى ما إذا كان التحكم يستخدم نمط الإشارة R1C1. |
| [RecalculateFormulas](../../aspose.cells.griddesktop/griddesktop/recalculateformulas/) { get; set; } | يحصل أو يعيّن قيمة تشير إلى ما إذا كان يجب إعادة حساب صيغ جميع الخلايا عندما يتغير قيمة خلية. القيمة الافتراضية هي true. |
| [RowHeaderVisible](../../aspose.cells.griddesktop/griddesktop/rowheadervisible/) { get; set; } | يحصل أو يعيّن قيمة تشير إلى ما إذا كان رأس الصف مرئيًا. |
| [SheetNameFont](../../aspose.cells.griddesktop/griddesktop/sheetnamefont/) { get; set; } | يحصل أو يعيّن الخط الافتراضي المعروض لشريط الورقة. |
| [SheetsBarVisible](../../aspose.cells.griddesktop/griddesktop/sheetsbarvisible/) { get; set; } | يحصل أو يعيّن قيمة تشير إلى ما إذا كان شريط الورقة مرئيًا. |
| [SheetTabWidth](../../aspose.cells.griddesktop/griddesktop/sheettabwidth/) { get; set; } | يضبط/يحصل على عرض علامة تبويب الورقة. |
| [ShowContextMenu](../../aspose.cells.griddesktop/griddesktop/showcontextmenu/) { get; set; } | يحصل أو يعيّن قيمة تشير إلى ما إذا كان التحكم يمكنه إظهار قائمة السياق. |
| [ShowFormulaWarning](../../aspose.cells.griddesktop/griddesktop/showformulawarning/) { get; set; } | يضبط/يحصل على ما إذا كان يجب إظهار رسالة الخطأ أو التحذير عند ضبط قيمة صيغة الخلية، القيمة الافتراضية هي true. |
| [ShowNumberStoredAsTextSymbol](../../aspose.cells.griddesktop/griddesktop/shownumberstoredastextsymbol/) { get; set; } | يضبط/يحصل على ما إذا كان يُظهر رمز المثلث للخلية التي تحتوي على سلسلة رقمية ولكن مخزنة كتنسيق نص. |
| [ShowStatus](../../aspose.cells.griddesktop/griddesktop/showstatus/) { get; set; } | يحصل أو يعيّن قيمة تشير إلى ما إذا كان يجب إظهار حالة الحساب. القيمة الافتراضية هي true. |
| [UndoManager](../../aspose.cells.griddesktop/griddesktop/undomanager/) { get; } | يحصل على مثيل UndoManager. |
| [Worksheets](../../aspose.cells.griddesktop/griddesktop/worksheets/) { get; } | يحصل على الـ Worksheets. |

## الطرق

| الاسم | الوصف |
| --- | --- |
| [Clear](../../aspose.cells.griddesktop/griddesktop/clear/)() | يمسح التحكم GridDesktop. |
| [Copy](../../aspose.cells.griddesktop/griddesktop/copy/)() | ينسخ محتوى الخلية المركزة إلى الحافظة. |
| [Cut](../../aspose.cells.griddesktop/griddesktop/cut/)() | يقص محتوى الخلية المركزة إلى الحافظة. |
| [DoSplit](../../aspose.cells.griddesktop/griddesktop/dosplit/)() | يضبط العرض المنقسم. |
| [EndFormatPainter](../../aspose.cells.griddesktop/griddesktop/endformatpainter/)() | يُخطر GridDesktop بإنهاء FormatPainter. |
| [ExportExcelFile](../../aspose.cells.griddesktop/griddesktop/exportexcelfile/#exportexcelfile)(Stream) | يصدّر إلى تدفق ملف إكسل، بما في ذلك تدفق إدخال/إخراج القرص أو تدفق الذاكرة. |
| [ExportExcelFile](../../aspose.cells.griddesktop/griddesktop/exportexcelfile/#exportexcelfile_2)(string) | يصدّر إلى ملف إكسل. |
| [ExportExcelFile](../../aspose.cells.griddesktop/griddesktop/exportexcelfile/#exportexcelfile_1)(Stream, FileFormatType) | يصدّر إلى تدفق ملف إكسل، بما في ذلك تدفق إدخال/إخراج القرص أو تدفق الذاكرة. |
| [ExportExcelFile](../../aspose.cells.griddesktop/griddesktop/exportexcelfile/#exportexcelfile_3)(string, FileFormatType) | يصدّر إلى ملف إكسل. |
| [ExportPdfFile](../../aspose.cells.griddesktop/griddesktop/exportpdffile/#exportpdffile)(Stream, GridPdfSaveOptions) | يصدّر إلى تدفق ملف PDF، بما في ذلك تدفق إدخال/إخراج القرص أو تدفق الذاكرة. |
| [ExportPdfFile](../../aspose.cells.griddesktop/griddesktop/exportpdffile/#exportpdffile_1)(string, GridPdfSaveOptions) | يصدّر إلى تدفق ملف PDF، بما في ذلك تدفق إدخال/إخراج القرص أو تدفق الذاكرة. |
| [GetActiveWorksheet](../../aspose.cells.griddesktop/griddesktop/getactiveworksheet/)() | يحصل على ورقة العمل النشطة الحالية. |
| [getHScrollBar](../../aspose.cells.griddesktop/griddesktop/gethscrollbar/)() | إرجاع شريط التمرير الأفقي |
| [getVScrollBar](../../aspose.cells.griddesktop/griddesktop/getvscrollbar/)() | إرجاع شريط التمرير العمودي |
| [ImportExcelFile](../../aspose.cells.griddesktop/griddesktop/importexcelfile/#importexcelfile)(Stream) | يستورد من تدفق ملف Excel، بما في ذلك تدفق ملف على القرص أو تدفق الذاكرة. |
| [ImportExcelFile](../../aspose.cells.griddesktop/griddesktop/importexcelfile/#importexcelfile_3)(string) | يستورد من ملف Excel. |
| [ImportExcelFile](../../aspose.cells.griddesktop/griddesktop/importexcelfile/#importexcelfile_1)(Stream, bool) | يستورد من تدفق ملف Excel، بما في ذلك تدفق ملف على القرص أو تدفق الذاكرة. |
| [ImportExcelFile](../../aspose.cells.griddesktop/griddesktop/importexcelfile/#importexcelfile_4)(string, bool) | يستورد من ملف Excel. |
| [ImportExcelFile](../../aspose.cells.griddesktop/griddesktop/importexcelfile/#importexcelfile_5)(string, int) | يستورد ورقة عمل من ملف إكسل. |
| [ImportExcelFile](../../aspose.cells.griddesktop/griddesktop/importexcelfile/#importexcelfile_2)(Stream, string, string, bool, bool) | يستورد من ملف Excel. |
| [ImportExcelFile](../../aspose.cells.griddesktop/griddesktop/importexcelfile/#importexcelfile_6)(string, string, string, bool, bool) | يستورد من ملف Excel. |
| [Invalidate](../../aspose.cells.griddesktop/griddesktop/invalidate/#invalidate)() | تجاوز الإبطال. |
| [OpenFindReplaceDialog](../../aspose.cells.griddesktop/griddesktop/openfindreplacedialog/)(bool) | يفتح حوار البحث والاستبدال للعثور على الخلايا أو استبدالها. |
| [Paste](../../aspose.cells.griddesktop/griddesktop/paste/)() | يلصق محتوى الحافظة إلى الخلية المركّزة. |
| [RefreshControl](../../aspose.cells.griddesktop/griddesktop/refreshcontrol/)() | تحديث عنصر التحكم GridDesktop. |
| [RunAllFormulas](../../aspose.cells.griddesktop/griddesktop/runallformulas/)() | ينفّذ جميع صيغ الخلايا. |
| [SetAllScrollBarsVisible](../../aspose.cells.griddesktop/griddesktop/setallscrollbarsvisible/)() | يضبط جميع أشرطة التمرير مرئية. |
| [SetCustomResourceManager](../../aspose.cells.griddesktop/griddesktop/setcustomresourcemanager/)(ResourceManager) | تعيين مدير موارد مخصص لتنفيذ التعريب المحدد من قبل المستخدم. |
| [ShowStyleDialog](../../aspose.cells.griddesktop/griddesktop/showstyledialog/)() | يفتح حوار النمط لتعيين نمط الخلايا، الخط، الألوان، إلخ. |
| [StartFormatPainter](../../aspose.cells.griddesktop/griddesktop/startformatpainter/)(bool) | يخطر GridDesktop لبدء FormatPainter. |
| [UnDoSplit](../../aspose.cells.griddesktop/griddesktop/undosplit/)() | إلغاء تعيين عرض الانقسام. |
| static [GetVersion](../../aspose.cells.griddesktop/griddesktop/getversion/)() | احصل على نسخة الإصدار. |

## الحقول

| الاسم | الوصف |
| --- | --- |
| [LoadDataFilter](../../aspose.cells.griddesktop/griddesktop/loaddatafilter/) | الخيارات لتصفية البيانات عند تحميل دفتر العمل من القالب. |
| [ShowImportMessage](../../aspose.cells.griddesktop/griddesktop/showimportmessage/) | ما إذا كان يجب إظهار مربع الرسالة عند فشل استيراد الملف، القيمة الافتراضية هي true. |

## الأحداث

| الاسم | الوصف |
| --- | --- |
| event [AfterDeleteColumns](../../aspose.cells.griddesktop/griddesktop/afterdeletecolumns/) | يحدث بعد حذف العمود. |
| event [AfterDeleteRows](../../aspose.cells.griddesktop/griddesktop/afterdeleterows/) | يحدث بعد حذف الصف. |
| event [AfterInsertColumns](../../aspose.cells.griddesktop/griddesktop/afterinsertcolumns/) | يحدث بعد إدراج عمود جديد. |
| event [AfterInsertRows](../../aspose.cells.griddesktop/griddesktop/afterinsertrows/) | يحدث بعد إدراج صف جديد. |
| event [BeforeCalculate](../../aspose.cells.griddesktop/griddesktop/beforecalculate/) | يحدث قبل حساب الصيغة في دفتر العمل. |
| event [BeforeLoadFile](../../aspose.cells.griddesktop/griddesktop/beforeloadfile/) | يحدث قبل تحميل دفتر العمل من الملف. |
| event [CellButtonClick](../../aspose.cells.griddesktop/griddesktop/cellbuttonclick/) | يحدث عندما يتم النقر على زر الخلية. |
| event [CellCheckedChanged](../../aspose.cells.griddesktop/griddesktop/cellcheckedchanged/) | يحدث عندما يتم تغيير خاصية Checked لخلية مربع الاختيار. |
| event [CellClick](../../aspose.cells.griddesktop/griddesktop/cellclick/) | يحدث عندما يتم النقر على الـgridcell. |
| event [CellComboBoxCopy](../../aspose.cells.griddesktop/griddesktop/cellcomboboxcopy/) | يحدث عندما يتم نسخ ComboBox خلية الشبكة. |
| event [CellDataChanged](../../aspose.cells.griddesktop/griddesktop/celldatachanged/) | يحدث عندما يتم تغيير خاصية البيانات لخلية الشبكة. |
| event [CellDoubleClick](../../aspose.cells.griddesktop/griddesktop/celldoubleclick/) | يحدث عندما يتم النقر المزدوج على الـgridcell. |
| event [CellFormatChanged](../../aspose.cells.griddesktop/griddesktop/cellformatchanged/) | يحدث عندما يتم تغيير تنسيق الخلية عبر مربع حوار Format Cells. |
| event [CellKeyPressed](../../aspose.cells.griddesktop/griddesktop/cellkeypressed/) | يحدث عندما يتم ضغط مفتاح بينما تكون الخلية مركزة. |
| event [CellSelectedIndexChanged](../../aspose.cells.griddesktop/griddesktop/cellselectedindexchanged/) | يحدث عندما تم تغيير خاصية SelectedIndex لعنصر تحكم combobox الخلية. |
| event [CellTextBoxChanging](../../aspose.cells.griddesktop/griddesktop/celltextboxchanging/) | يحدث عند كتابة أحرف في خلية الشبكة. |
| event [CellValidationFailed](../../aspose.cells.griddesktop/griddesktop/cellvalidationfailed/) | يحدث عندما تفشل عملية التحقق في خلية الشبكة. |
| event [ColumnHeaderClick](../../aspose.cells.griddesktop/griddesktop/columnheaderclick/) | يحدث عندما يتم النقر على رأس العمود. |
| event [ColumnHeaderDoubleClick](../../aspose.cells.griddesktop/griddesktop/columnheaderdoubleclick/) | يحدث عندما يتم النقر المزدوج على رأس العمود. |
| event [CommentDataChanged](../../aspose.cells.griddesktop/griddesktop/commentdatachanged/) | يحدث عندما يتم تغيير بيانات التعليق. |
| event [FailLoadFile](../../aspose.cells.griddesktop/griddesktop/failloadfile/) |  |
| event [FinishCalculate](../../aspose.cells.griddesktop/griddesktop/finishcalculate/) | يحدث بعد حساب الصيغة في المصنف. |
| event [FinishLoadFile](../../aspose.cells.griddesktop/griddesktop/finishloadfile/) | يحدث عندما يتم تحميل المصنف. |
| event [FocusedCellChanged](../../aspose.cells.griddesktop/griddesktop/focusedcellchanged/) | يحدث عندما يتم تغيير الخلية المركزة. |
| event [PictureClick](../../aspose.cells.griddesktop/griddesktop/pictureclick/) | يحدث عندما يتم النقر على الشكل. |
| event [RowColumnHiddenChanged](../../aspose.cells.griddesktop/griddesktop/rowcolumnhiddenchanged/) | يحدث عندما يتغير حالة إخفاء الصف/العمود. |
| event [RowFilteredEvent](../../aspose.cells.griddesktop/griddesktop/rowfilteredevent/) | يحدث بعد اختيار عنصر تصفية الصف. |
| event [RowHeaderClick](../../aspose.cells.griddesktop/griddesktop/rowheaderclick/) | يحدث عندما يتم النقر على رأس الصف. |
| event [RowHeaderDoubleClick](../../aspose.cells.griddesktop/griddesktop/rowheaderdoubleclick/) | يحدث عندما يتم النقر المزدوج على رأس الصف. |
| event [SelectedCellRangeChanged](../../aspose.cells.griddesktop/griddesktop/selectedcellrangechanged/) | يحدث عندما يتم تغيير نطاق الخلايا المحدد. |
| event [SelectedSheetIndexChanged](../../aspose.cells.griddesktop/griddesktop/selectedsheetindexchanged/) | يحدث عندما يتم تغيير خاصية SelectedSheetIndex. |
| event [ShapeClick](../../aspose.cells.griddesktop/griddesktop/shapeclick/) | يحدث عندما يتم النقر على الشكل. |

### ملاحظات

يرجى الرجوع إلى وثيقة .NET SDK للحصول على مزيد من المعلومات حول System.Windows.Forms.UserControl.

### أمثلة

```csharp
[C#]
gridDesktop1.Worksheets[0].Cells[0, 0].Value = "2";
gridDesktop1.Worksheets[0].Cells[1, 0].Value = "3";
gridDesktop1.Worksheets[0].Cells[2, 1].Value = "=a1*a2";
gridDesktop1.RunAllFormulas();
gridDesktop1.Invalidate();

[Visual Basic]
gridDesktop1.Worksheets(0).Cells(0, 0).Value = "2"
gridDesktop1.Worksheets(0).Cells(1, 0).Value = "3"
gridDesktop1.Worksheets(0).Cells(2, 1).Value = "=a1*a2"
gridDesktop1.RunAllFormulas()
gridDesktop1.Invalidate()

```

### انظر أيضًا

* namespace [Aspose.Cells.GridDesktop](../../aspose.cells.griddesktop/)
* assembly [Aspose.Cells.GridDesktop](../../)


