---
title: "فئة Cells"
linktitle: "الخلايا"
second_title: "مرجع API لـ Aspose.Cells for Go عبر C++"
description: "فئة Cells. تغلف الكائن الذي يمثل الخلايا في Go."
type: docs
weight: 200
url: /ar/go-cpp/cells/
---

## Cells class

يغلف مجموعة من الكائنات المتعلقة بالخلية، مثل <see cref=\"Cell\"/>، <see cref=\"Row\"/>، ... إلخ.

```go

type Cells struct  {
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
| [GetOdsCellFields](./getodscellfields/) | يحصل على قائمة الحقول في ods. |
| [Dispose](./dispose/) | يؤدي مهامًا محددة من قبل التطبيق مرتبطة بتحرير أو إطلاق أو إعادة ضبط الموارد غير المُدارة. |
| [GetCount](./getcount/) | يحصل على العدد الإجمالي لكائنات Cell المُنشأة. |
| [GetCountLarge](./getcountlarge/) | يحصل على العدد الإجمالي لكائنات Cell المُنشأة. |
| [GetEnumerator](./getenumerator/) | يحصل على مُعدِّد الخلايا. |
| [GetRows](./getrows/) | يحصل على مجموعة كائنات Row التي تمثل الصفوف الفردية في ورقة العمل هذه. |
| [GetMergedAreas](./getmergedareas/) | يحصل على جميع الخلايا المدمجة. |
| [CheckCell](./checkcell/) | يحصل على عنصر Cell أو null عند فهرس صف الخلية والعمود المحددين. |
| [CheckRow](./checkrow/) | يحصل على عنصر Row أو null عند فهرس صف الخلية المحدد. |
| [CheckColumn](./checkcolumn/) | يحصل على عنصر Column أو null عند فهرس العمود المحدد. |
| [IsRowHidden](./isrowhidden/) | يتحقق مما إذا كان الصف عند الفهرس المحدد مخفيًا. |
| [IsColumnHidden](./iscolumnhidden/) | يتحقق مما إذا كان العمود عند الفهرس المحدد مخفيًا. |
| [AddRange](./addrange/) | يضيف مرجع كائن نطاق إلى الخلايا |
| [CreateRange_String_String](./createrange_string_string/) | ينشئ كائن Range من نطاق من الخلايا. |
| [CreateRange_Int_Int_Int_Int](./createrange_int_int_int_int/) | ينشئ كائن Range من نطاق من الخلايا. |
| [CreateRange_String](./createrange_string/) | ينشئ كائن Range من عنوان النطاق. |
| [CreateRange_Int_Int_Bool](./createrange_int_int_bool/) | ينشئ كائن Range من صفوف الخلايا أو أعمدة الخلايا. |
| [Get_Int_Int](./get_int_int/) | يحصل على عنصر Cell في فهرس صف الخلية المحدد وفهرس العمود. |
| [Get_String](./get_string/) | يحصل على عنصر Cell بالاسم المحدد للخلية. |
| [GetMultiThreadReading](./getmultithreadreading/) | يحصل أو يضبط ما إذا كان نموذج بيانات الخلايا يجب أن يدعم القراءة متعددة الخيوط. القيمة الافتراضية لهذه الخاصية هي false. |
| [SetMultiThreadReading](./setmultithreadreading/) | يحصل أو يضبط ما إذا كان نموذج بيانات الخلايا يجب أن يدعم القراءة متعددة الخيوط. القيمة الافتراضية لهذه الخاصية هي false. |
| [GetMemorySetting](./getmemorysetting/) | يحصل أو يضبط خيار استخدام الذاكرة لهذه الخلايا. |
| [SetMemorySetting](./setmemorysetting/) | يحصل أو يضبط خيار استخدام الذاكرة لهذه الخلايا. |
| [Clear](./clear/) | يمسح جميع بيانات ورقة العمل. |
| [GetStyle](./getstyle/) | يحصل ويضبط النمط الافتراضي لورقة العمل. |
| [SetStyle](./setstyle/) | يحصل ويضبط النمط الافتراضي لورقة العمل. |
|[IsDefaultColumnHidden](./isdefaultcolumnhidden/) |  | 
|[SetIsDefaultColumnHidden](./setisdefaultcolumnhidden/) |  | 
| [GetStandardWidthInch](./getstandardwidthinch/) | يحصل أو يضبط عرض العمود الافتراضي في ورقة العمل، بوحدة البوصة. |
| [SetStandardWidthInch](./setstandardwidthinch/) | يحصل أو يضبط عرض العمود الافتراضي في ورقة العمل، بوحدة البوصة. |
| [GetStandardWidthPixels](./getstandardwidthpixels/) | يحصل أو يضبط عرض العمود الافتراضي في ورقة العمل، بوحدة البكسل. |
| [SetStandardWidthPixels](./setstandardwidthpixels/) | يحصل أو يضبط عرض العمود الافتراضي في ورقة العمل، بوحدة البكسل. |
| [GetStandardWidth](./getstandardwidth/) | يحصل أو يضبط عرض العمود الافتراضي في ورقة العمل، بوحدة الأحرف. |
| [SetStandardWidth](./setstandardwidth/) | يحصل أو يضبط عرض العمود الافتراضي في ورقة العمل، بوحدة الأحرف. |
| [GetStandardHeight](./getstandardheight/) | يحصل أو يضبط ارتفاع الصف الافتراضي في هذه الورقة، بوحدة النقاط. |
| [SetStandardHeight](./setstandardheight/) | يحصل أو يضبط ارتفاع الصف الافتراضي في هذه الورقة، بوحدة النقاط. |
| [GetStandardHeightPixels](./getstandardheightpixels/) | يحصل أو يضبط ارتفاع الصف الافتراضي في هذه الورقة، بوحدة البكسل. |
| [SetStandardHeightPixels](./setstandardheightpixels/) | يحصل أو يضبط ارتفاع الصف الافتراضي في هذه الورقة، بوحدة البكسل. |
| [GetStandardHeightInch](./getstandardheightinch/) | يحصل أو يضبط ارتفاع الصف الافتراضي في هذه الورقة، بوحدة البوصة. |
| [SetStandardHeightInch](./setstandardheightinch/) | يحصل أو يضبط ارتفاع الصف الافتراضي في هذه الورقة، بوحدة البوصة. |
| [ImportFormulaArray](./importformulaarray/) | يستورد مصفوفة من الصيغ إلى ورقة العمل. |
| [TextToColumns](./texttocolumns/) | يقسم المحتوى في العمود المحدد إلى عدة أعمدة.. |
| [ImportCSV_String_String_Bool_Int_Int](./importcsv_string_string_bool_int_int/) | استيراد ملف CSV إلى الخلايا. |
| [ImportCSV_Stream_String_Bool_Int_Int](./importcsv_stream_string_bool_int_int/) | استيراد ملف CSV إلى الخلايا. |
| [ImportCSV_String_TxtLoadOptions_Int_Int](./importcsv_string_txtloadoptions_int_int/) | استيراد ملف CSV إلى الخلايا. |
| [ImportCSV_Stream_TxtLoadOptions_Int_Int](./importcsv_stream_txtloadoptions_int_int/) | استيراد ملف CSV إلى الخلايا. |
| [GetPreserveString](./getpreservestring/) | يحصل أو يضبط قيمة تشير إلى ما إذا كانت جميع قيم ورقة العمل تُحفظ كسلاسل. القيمة الافتراضية هي false. |
| [SetPreserveString](./setpreservestring/) | يحصل أو يضبط قيمة تشير إلى ما إذا كانت جميع قيم ورقة العمل تُحفظ كسلاسل. القيمة الافتراضية هي false. |
| [Merge_Int_Int_Int_Int](./merge_int_int_int_int/) | يدمج نطاقًا محددًا من الخلايا في خلية واحدة. |
| [Merge_Int_Int_Int_Int_Bool](./merge_int_int_int_int_bool/) | يدمج نطاقًا محددًا من الخلايا في خلية واحدة. |
| [Merge_Int_Int_Int_Int_Bool_Bool](./merge_int_int_int_int_bool_bool/) | يدمج نطاقًا محددًا من الخلايا في خلية واحدة. |
| [UnMerge](./unmerge/) | يفك دمج نطاق محدد من الخلايا المدمجة. |
| [ClearMergedCells](./clearmergedcells/) | يمسح جميع النطاقات المدمجة. |
| [HideRow](./hiderow/) | يخفي صفًا. |
| [UnhideRow](./unhiderow/) | يكشف عن صف. |
| [HideRows](./hiderows/) | يخفي عدة صفوف. |
| [UnhideRows](./unhiderows/) | يفك إخفاء الصفوف المخفية. |
| [SetRowHeightPixel](./setrowheightpixel/) | يضبط ارتفاع الصف بوحدة البكسل. |
| [SetRowHeightInch](./setrowheightinch/) | يضبط ارتفاع الصف بوحدة البوصة. |
| [SetRowHeight](./setrowheight/) | يضبط ارتفاع الصف المحدد. |
| [GetRowHeight_Int_Bool_CellsUnitType](./getrowheight_int_bool_cellsunittype/) | يحصل على ارتفاع الصف. |
| [GetColumnWidth_Int_Bool_CellsUnitType](./getcolumnwidth_int_bool_cellsunittype/) | يحصل على عرض العمود. |
| [HideColumn](./hidecolumn/) | يخفي عمودًا. |
| [UnhideColumn](./unhidecolumn/) | يفك إخفاء عمود |
| [HideColumns](./hidecolumns/) | إخفاء عدة أعمدة. |
| [UnhideColumns](./unhidecolumns/) | إلغاء إخفاء عدة أعمدة. |
| [GetRowHeight_Int](./getrowheight_int/) | يحصل على ارتفاع صف محدد بوحدة النقاط. |
| [GetViewRowHeight](./getviewrowheight/) | يحصل على ارتفاع صف محدد. |
| [GetRowHeightInch](./getrowheightinch/) | يحصل على ارتفاع صف محدد بوحدة البوصة. |
| [GetViewRowHeightInch](./getviewrowheightinch/) | يحصل على ارتفاع صف محدد بوحدة البوصة. |
| [GetRowHeightPixel](./getrowheightpixel/) | يحصل على ارتفاع صف محدد بوحدة البكسل. |
| [SetColumnWidthPixel](./setcolumnwidthpixel/) | يضبط عرض العمود بوحدة البكسل في العرض العادي. |
| [SetColumnWidthInch](./setcolumnwidthinch/) | يضبط عرض العمود بوحدة البوصة في العرض العادي. |
| [SetColumnWidth](./setcolumnwidth/) | يضبط عرض العمود المحدد في العرض العادي. |
| [GetColumnWidthPixel](./getcolumnwidthpixel/) | يحصل على عرض العمود المحدد في العرض العادي بوحدة البكسل. |
| [GetColumnWidth_Int](./getcolumnwidth_int/) | يحصل على عرض (بوحدة الأحرف) العمود المحدد في العرض العادي |
| [GetViewColumnWidthPixel](./getviewcolumnwidthpixel/) | احصل على العرض في نوع عرض مختلف. |
| [SetViewColumnWidthPixel](./setviewcolumnwidthpixel/) | يضبط عرض العمود في عرض مختلف. |
| [GetMinRow](./getminrow/) | الحد الأدنى لفهرس الصف للخلية التي تحتوي على بيانات أو نمط. |
| [GetMaxRow](./getmaxrow/) | الحد الأقصى لفهرس الصف للخلية التي تحتوي على بيانات أو نمط. |
| [GetMinColumn](./getmincolumn/) | الحد الأدنى لفهرس العمود لتلك الخلايا التي تم إنشاءها في المجموعة (لا تشمل العمود الذي تم تعريف النمط له لكامل العمود ولكن لم يتم إنشاء أي خلية فيه). |
| [GetMaxColumn](./getmaxcolumn/) | الحد الأقصى لمؤشر العمود لتلك الخلايا التي تم إنشاؤها في المجموعة(لا يشمل العمود الذي تم تعريف النمط له لكامل العمود ولكن لم يتم إنشاء أي خلية فيه). |
| [GetMinDataRow](./getmindatarow/) | الحد الأدنى لمؤشر الصف للخلية التي تحتوي على بيانات. |
| [GetMaxDataRow](./getmaxdatarow/) | الحد الأقصى لمؤشر الصف للخلية التي تحتوي على بيانات. |
| [GetMinDataColumn](./getmindatacolumn/) | الحد الأدنى لمؤشر العمود للخلية التي تحتوي على بيانات. |
| [GetMaxDataColumn](./getmaxdatacolumn/) | الحد الأقصى لمؤشر العمود للخلية التي تحتوي على بيانات. |
| [GetLastDataRow](./getlastdatarow/) | يحصل على مؤشر الصف الأخير للخلية التي تحتوي على بيانات في العمود المحدد. |
| [GetFirstDataRow](./getfirstdatarow/) | يحصل على مؤشر الصف الأول للخلية التي تحتوي على بيانات في العمود المحدد. |
| [IsDefaultRowHeightMatched](./isdefaultrowheightmatched/) | يشير إلى أن ارتفاع الصف وارتفاع الخط الافتراضي متطابقان |
| [SetIsDefaultRowHeightMatched](./setisdefaultrowheightmatched/) | يشير إلى أن ارتفاع الصف وارتفاع الخط الافتراضي متطابقان |
| [IsDefaultRowHidden](./isdefaultrowhidden/) | يشير إلى ما إذا كان الصف مخفيًا بشكل افتراضي. |
| [SetIsDefaultRowHidden](./setisdefaultrowhidden/) | يشير إلى ما إذا كان الصف مخفيًا بشكل افتراضي. |
| [GetColumns](./getcolumns/) | يحصل على مجموعة كائنات العمود التي تمثل الأعمدة الفردية في ورقة العمل هذه. |
| [ApplyColumnStyle](./applycolumnstyle/) | يطبق التنسيقات على عمود كامل. |
| [ApplyRowStyle](./applyrowstyle/) | يطبق التنسيقات على صف كامل. |
| [ApplyStyle](./applystyle/) | يطبق التنسيقات على ورقة عمل كاملة. |
| [CopyColumns_Cells_Int_Int_Int_PasteOptions](./copycolumns_cells_int_int_int_pasteoptions/) | ينسخ البيانات والتنسيقات لعمود كامل. |
| [CopyColumn](./copycolumn/) | ينسخ البيانات والتنسيقات لعمود كامل. |
| [CopyColumns_Cells_Int_Int_Int](./copycolumns_cells_int_int_int/) | ينسخ البيانات والتنسيقات لأعمدة كاملة. |
| [CopyColumns_Cells_Int_Int_Int_Int](./copycolumns_cells_int_int_int_int/) | ينسخ البيانات والتنسيقات للأعمدة كلها. |
| [CopyRow](./copyrow/) | ينسخ البيانات والتنسيقات لصف كامل. |
| [CopyRows_Cells_Int_Int_Int](./copyrows_cells_int_int_int/) | ينسخ البيانات والتنسيقات لبعض الصفوف الكاملة. |
| [CopyRows_Cells_Int_Int_Int_CopyOptions](./copyrows_cells_int_int_int_copyoptions/) | ينسخ البيانات والتنسيقات لبعض الصفوف الكاملة. |
| [CopyRows_Cells_Int_Int_Int_CopyOptions_PasteOptions](./copyrows_cells_int_int_int_copyoptions_pasteoptions/) | ينسخ البيانات والتنسيقات لبعض الصفوف الكاملة. |
| [GetGroupedRowOutlineLevel](./getgroupedrowoutlinelevel/) | يحصل على مستوى المخطط (مستند إلى الصفر) للصف. |
| [GetGroupedColumnOutlineLevel](./getgroupedcolumnoutlinelevel/) | يحصل على مستوى المخطط (مستند إلى الصفر) للعمود. |
| [GetMaxGroupedColumnOutlineLevel](./getmaxgroupedcolumnoutlinelevel/) | يحصل على الحد الأقصى لمستوى مخطط العمود المجمّع (مستند إلى الصفر). |
| [GetMaxGroupedRowOutlineLevel](./getmaxgroupedrowoutlinelevel/) | يحصل على الحد الأقصى لمستوى مخطط الصف المجمّع (مستند إلى الصفر). |
| [ShowGroupDetail](./showgroupdetail/) | يوسع الصفوف/الأعمدة المجمعة. |
| [HideGroupDetail](./hidegroupdetail/) | يطوي الصفوف/الأعمدة المجمعة. |
| [UngroupColumns](./ungroupcolumns/) | يفك تجميع الأعمدة. |
| [GroupColumns_Int_Int](./groupcolumns_int_int/) | يجمع الأعمدة. |
| [GroupColumns_Int_Int_Bool](./groupcolumns_int_int_bool/) | يجمع الأعمدة. |
| [UngroupRows_Int_Int_Bool](./ungrouprows_int_int_bool/) | يفك تجميع الصفوف. |
| [UngroupRows_Int_Int](./ungrouprows_int_int/) | يفك تجميع الصفوف. |
| [GroupRows_Int_Int_Bool](./grouprows_int_int_bool/) | يجمع الصفوف. |
| [GroupRows_Int_Int](./grouprows_int_int/) | يجمع الصفوف. |
| [DeleteColumn_Int_Bool](./deletecolumn_int_bool/) | يحذف عمودًا. |
| [DeleteColumn_Int](./deletecolumn_int/) | يحذف عمودًا. |
| [DeleteColumns_Int_Int_Bool](./deletecolumns_int_int_bool/) | يحذف عدة أعمدة. |
| [DeleteColumns_Int_Int_DeleteOptions](./deletecolumns_int_int_deleteoptions/) | يحذف عدة أعمدة. |
| [IsDeletingRangeEnabled](./isdeletingrangeenabled/) | تحقق مما إذا كان يمكن حذف النطاق. |
| [DeleteRow_Int](./deleterow_int/) | يحذف صفًا. |
| [DeleteRow_Int_Bool](./deleterow_int_bool/) | يحذف صفًا. |
| [DeleteRows_Int_Int](./deleterows_int_int/) | يحذف عدة صفوف. |
| [DeleteRows_Int_Int_Bool](./deleterows_int_int_bool/) | يحذف عدة صفوف في ورقة العمل. |
| [DeleteRows_Int_Int_DeleteOptions](./deleterows_int_int_deleteoptions/) | يحذف عدة صفوف في ورقة العمل. |
| [DeleteBlankColumns](./deleteblankcolumns/) | احذف جميع الأعمدة الفارغة التي لا تحتوي على أي بيانات. |
| [DeleteBlankColumns_DeleteOptions](./deleteblankcolumns_deleteoptions/) | احذف جميع الأعمدة الفارغة التي لا تحتوي على أي بيانات. |
| [IsBlankColumn](./isblankcolumn/) | يتحقق مما إذا كان العمود المحدد فارغًا (لا يحتوي على أي بيانات). |
| [DeleteBlankRows](./deleteblankrows/) | احذف جميع الصفوف الفارغة التي لا تحتوي على أي بيانات أو كائن آخر. |
| [DeleteBlankRows_DeleteOptions](./deleteblankrows_deleteoptions/) | احذف جميع الصفوف الفارغة التي لا تحتوي على أي بيانات أو بعض الكائنات الخاصة مثل التعليق الظاهر، جدول محوري. |
| [InsertColumns_Int_Int](./insertcolumns_int_int/) | يدخل بعض الأعمدة في ورقة العمل. |
| [InsertColumns_Int_Int_Bool](./insertcolumns_int_int_bool/) | يدخل بعض الأعمدة في ورقة العمل. |
| [InsertColumns_Int_Int_InsertOptions](./insertcolumns_int_int_insertoptions/) | يدخل بعض الأعمدة في ورقة العمل. |
| [InsertColumn_Int_Bool](./insertcolumn_int_bool/) | يدخل عمودًا جديدًا في ورقة العمل. |
| [InsertColumn_Int](./insertcolumn_int/) | يدخل عمودًا جديدًا في ورقة العمل. |
| [InsertRows_Int_Int_Bool](./insertrows_int_int_bool/) | يدخل عدة صفوف في ورقة العمل. |
| [InsertRows_Int_Int_InsertOptions](./insertrows_int_int_insertoptions/) | يدخل عدة صفوف في ورقة العمل. |
| [InsertRows_Int_Int](./insertrows_int_int/) | يدخل عدة صفوف في ورقة العمل. |
| [InsertRow](./insertrow/) | يدخل صفًا جديدًا في ورقة العمل. |
| [GetRanges](./getranges/) | يحصل على مجموعة كائنات النطاق التي تم إنشاؤها في وقت التشغيل. |
| [ClearRange_CellArea](./clearrange_cellarea/) | يمسح محتوى وتنسيق نطاق. |
| [ClearRange_Int_Int_Int_Int](./clearrange_int_int_int_int/) | يمسح محتوى وتنسيق نطاق. |
| [ClearContents_CellArea](./clearcontents_cellarea/) | يمسح محتوى نطاق. |
| [ClearContents_Int_Int_Int_Int](./clearcontents_int_int_int_int/) | يمسح محتوى نطاق. |
| [ClearFormats_CellArea](./clearformats_cellarea/) | يمسح تنسيق نطاق. |
| [ClearFormats_Int_Int_Int_Int](./clearformats_int_int_int_int/) | يمسح تنسيق نطاق. |
| [GetLastCell](./getlastcell/) | يحصل على الخلية الأخيرة في هذه ورقة العمل. |
| [LinkToXmlMap](./linktoxmlmap/) | رابط إلى خريطة XML. |
| [GetMaxDisplayRange](./getmaxdisplayrange/) | يحصل على النطاق الأقصى الذي يشمل البيانات والخلايا المدمجة والأشكال. |
| [GetFirstCell](./getfirstcell/) | يحصل على الخلية الأولى في هذه ورقة العمل. |
| [Find_Object_Cell](./find_object_cell/) | يجد الخلية التي تحتوي على كائن الإدخال. |
| [Find_Object_Cell_FindOptions](./find_object_cell_findoptions/) | يجد الخلية التي تحتوي على كائن الإدخال. |
| [EndCellInRow_Int](./endcellinrow_int/) | يحصل على الخلية الأخيرة في هذا الصف. |
| [EndCellInColumn_Int](./endcellincolumn_int/) | يحصل على الخلية الأخيرة في هذا العمود. |
| [EndCellInColumn_Int_Int_Int_Int](./endcellincolumn_int_int_int_int/) | يحصل على الخلية الأخيرة ذات أعلى فهرس عمود في هذا النطاق. |
| [EndCellInRow_Int_Int_Int_Int](./endcellinrow_int_int_int_int/) | يحصل على الخلية الأخيرة ذات أعلى فهرس صف في هذا النطاق. |
| [MoveRange](./moverange/) | ينقل النطاق. |
| [InsertCutCells](./insertcutcells/) | إدراج نطاق مقطوع. |
| [InsertRange_CellArea_Int_ShiftType_Bool](./insertrange_cellarea_int_shifttype_bool/) | يدرج نطاقًا من الخلايا ويُحرك الخلايا وفقًا لخيار التحريك. |
| [InsertRange_CellArea_ShiftType](./insertrange_cellarea_shifttype/) | يدرج نطاقًا من الخلايا ويُحرك الخلايا وفقًا لخيار التحريك. |
| [InsertRange_CellArea_Int_ShiftType](./insertrange_cellarea_int_shifttype/) | يدرج نطاقًا من الخلايا ويُحرك الخلايا وفقًا لخيار التحريك. |
| [DeleteRange](./deleterange/) | يحذف نطاقًا من الخلايا ويُحرك الخلايا وفقًا لخيار التحريك. |
| [ExportArray](./exportarray/) | يصدّر البيانات في مجموعة الخلايا إلى كائن مصفوفة ثنائية الأبعاد. |
| [RetrieveSubtotalSetting](./retrievesubtotalsetting/) | يسترجع إعدادات المجاميع الفرعية للنطاق. |
| [Subtotal_CellArea_Int_ConsolidationFunction_int32Array](./subtotal_cellarea_int_consolidationfunction_int32array/) | ينشئ مجاميع فرعية للنطاق. |
| [Subtotal_CellArea_Int_ConsolidationFunction_int32Array_Bool_Bool_Bool](./subtotal_cellarea_int_consolidationfunction_int32array_bool_bool_bool/) | ينشئ مجاميع فرعية للنطاق. |
| [RemoveFormulas](./removeformulas/) | يزيل جميع الصيغ ويستبدلها بقيمة الصيغة. |
| [RemoveDuplicates](./removeduplicates/) | يزيل الصفوف المكررة في الورقة. |
| [RemoveDuplicates_Int_Int_Int_Int](./removeduplicates_int_int_int_int/) | يزيل القيم المكررة في النطاق. |
| [RemoveDuplicates_Int_Int_Int_Int_Bool_int32Array](./removeduplicates_int_int_int_int_bool_int32array/) | يزيل البيانات المكررة في النطاق. |
| [ConvertStringToNumericValue](./convertstringtonumericvalue/) | يحوّل جميع البيانات النصية في ورقة العمل إلى قيمة رقمية إذا أمكن. |
| [GetDependents](./getdependents/) | احصل على جميع الخلايا التي تشير إلى الخلية المحددة. |
| [GetDependentsInCalculation](./getdependentsincalculation/) | يحصل على جميع الخلايا التي تعتمد نتيجتها المحسوبة على خلية محددة. |
| [GetCellsWithPlaceInCellPicture](./getcellswithplaceincellpicture/) | يحصل على جميع الخلايا التي تحتوي على صورة مدمجة. |
| [GetCellStyle](./getcellstyle/) | احصل على نمط الخلية المعطاة. |
| [GetCellDisplayStyle_Int_Int](./getcelldisplaystyle_int_int/) | احصل على نمط العرض للخلية المعطاة. |
| [GetCellDisplayStyle_Int_Int_BorderType](./getcelldisplaystyle_int_int_bordertype/) | احصل على نمط العرض للخلية المعطاة. |
