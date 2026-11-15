---
title: "فئة ShapeCollection"
linktitle: "ShapeCollection"
second_title: "مرجع API لـ Aspose.Cells for Go عبر C++"
description: "فئة ShapeCollection. يغلف الكائن الذي يمثل shapecollection في Go."
type: docs
weight: 200
url: /ar/go-cpp/shapecollection/
---

## ShapeCollection class

يمثل جميع الأشكال في ورقة العمل/المخطط.

```go

type ShapeCollection struct  {
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
| [Get_Int](./get_int/) | يحصل على كائن Shape في الفهرس المحدد في القائمة. |
| [Get_String](./get_string/) | يحصل على كائن Shape حسب اسم الشكل. |
| [AddCopy_Shape_Int_Int_Int_Int](./addcopy_shape_int_int_int_int/) | يضيف وينسخ شكلًا إلى ورقة العمل. |
| [AddCopy_Shape_Int_Int_Int_Int_CopyOptions](./addcopy_shape_int_int_int_int_copyoptions/) | يضيف وينسخ شكلًا إلى ورقة العمل. |
| [AddCheckBox](./addcheckbox/) | يضيف مربع اختيار إلى ورقة العمل. |
| [AddTextBox](./addtextbox/) | يضيف مربع نص إلى ورقة العمل. |
| [AddEquation](./addequation/) | يضيف كائن معادلة إلى ورقة العمل. |
| [AddLaTeXEquation](./addlatexequation/) | يضيف كائن معادلة إلى ورقة العمل باستخدام سلاسل تنسيق LaTeX. |
| [AddSpinner](./addspinner/) | يضيف عنصر Spinner إلى ورقة العمل. |
| [AddScrollBar](./addscrollbar/) | يضيف عنصر ScrollBar إلى ورقة العمل. |
| [AddRadioButton](./addradiobutton/) | يضيف عنصر RadioButton إلى ورقة العمل. |
| [AddListBox](./addlistbox/) | يضيف عنصر ListBox إلى ورقة العمل. |
| [AddComboBox](./addcombobox/) | يضيف عنصر ComboBox إلى ورقة العمل. |
| [AddGroupBox](./addgroupbox/) | يضيف عنصر GroupBox إلى ورقة العمل. |
| [AddButton](./addbutton/) | يضيف عنصر Button إلى ورقة العمل. |
| [AddLabel](./addlabel/) | يضيف عنصر Label إلى ورقة العمل. |
| [AddLabelInChart](./addlabelinchart/) | يضيف عنصر label إلى المخطط. |
| [AddTextBoxInChart](./addtextboxinchart/) | يضيف عنصر textbox إلى المخطط. |
| [AddTextEffectInChart](./addtexteffectinchart/) | يدرج كائن WordArt إلى المخطط |
| [AddTextEffect](./addtexteffect/) | يدرج كائن WordArt. |
| [AddWordArt](./addwordart/) | يضيف WordArt مسبق الإعداد منذ Excel 2007.s |
| [AddRectangle](./addrectangle/) | يضيف RectangleShape إلى ورقة العمل. |
| [AddOval](./addoval/) | يضيف Oval إلى ورقة العمل. |
| [AddLine](./addline/) | يضيف LineShape إلى ورقة العمل. |
| [AddFreeFloatingShape](./addfreefloatingshape/) | يضيف شكلًا عائمًا حرًا إلى ورقة العمل.ينطبق فقط على شكل الخط/الصورة. |
| [AddShapeInChart_MsoDrawingType_PlacementType_Int_Int_Int_Int_Stream](./addshapeinchart_msodrawingtype_placementtype_int_int_int_int_stream/) | أضف شكلًا إلى المخطط .كل وحدة هي 1/4000 من مساحة المخطط. |
| [AddShapeInChart_MsoDrawingType_PlacementType_Int_Int_Int_Int](./addshapeinchart_msodrawingtype_placementtype_int_int_int_int/) | أضف شكلًا إلى المخطط .كل وحدة هي 1/4000 من مساحة المخطط. |
| [AddShapeInChartByScale_MsoDrawingType_PlacementType_Double_Double_Double_Double](./addshapeinchartbyscale_msodrawingtype_placementtype_double_double_double_double/) | أضف شكلًا إلى المخطط. كل وحدة هي نسبة مئوية من مساحة المخطط. |
| [AddShapeInChartByScale_MsoDrawingType_PlacementType_Double_Double_Double_Double_Stream](./addshapeinchartbyscale_msodrawingtype_placementtype_double_double_double_double_stream/) | أضف شكلًا إلى المخطط .كل وحدة هي 1/4000 من مساحة المخطط. |
| [AddArc](./addarc/) | يضيف ArcShape إلى ورقة العمل. |
| [AddShape](./addshape/) | يضيف Shape إلى ورقة العمل. |
| [AddAutoShape](./addautoshape/) | يضيف AutoShape إلى ورقة العمل. |
| [AddAutoShapeInChart](./addautoshapeinchart/) | يضيف AutoShape إلى المخطط. |
| [AddActiveXControl](./addactivexcontrol/) | ينشئ Activex Control. |
| [AddPicture_Int_Int_Int_Int_Stream](./addpicture_int_int_int_int_stream/) | يضيف صورة إلى المجموعة. |
| [AddPicture_Int_Int_Stream_Int_Int](./addpicture_int_int_stream_int_int/) | يضيف صورة إلى المجموعة. |
| [AddSvg](./addsvg/) | يضيف صورة svg. |
| [AddIcons](./addicons/) | يضيف صورة svg. |
| [AddLinkedPicture](./addlinkedpicture/) | أضف صورة مرتبطة. |
| [AddOleObjectWithLinkedImage](./addoleobjectwithlinkedimage/) | أضف صورة مرتبطة. |
| [AddPictureInChart](./addpictureinchart/) | يضيف صورة إلى المخطط. |
| [AddOleObject](./addoleobject/) | يضيف كائن OleObject. |
| [CopyCommentsInRange](./copycommentsinrange/) | نسخ جميع التعليقات في النطاق. |
| [CopyInRange](./copyinrange/) | نسخ الأشكال في النطاق إلى النطاق الوجهة. |
| [DeleteInRange](./deleteinrange/) | احذف الأشكال في النطاق. لن يتم حذف أشكال التعليق. |
| [DeleteShape](./deleteshape/) | احذف شكلاً. إذا كان الشكل في مجموعة أو كان شكل تعليق، فلن يتم حذفه. |
| [Group](./group/) | تجميع الأشكال. |
| [Ungroup](./ungroup/) | إلغاء تجميع عناصر الشكل. |
| [RemoveAt](./removeat/) | إزالة الشكل. |
| [Remove](./remove/) | إزالة الشكل. |
| [Clear](./clear/) | مسح جميع الأشكال في ورقة العمل. |
| [UpdateSelectedValue](./updateselectedvalue/) | تحديث القيمة المحددة بقيمة الخلية المرتبطة أو نطاق الشكل. |
| [AddFreeform](./addfreeform/) | يضيف شكلاً حرًا إلى ورقة العمل. |
| [AddSignatureLine](./addsignatureline/) | يضيف سطر توقيع إلى ورقة العمل. |
| [GetCount](./getcount/) | يحصل على عدد العناصر الموجودة في المثيل. |
