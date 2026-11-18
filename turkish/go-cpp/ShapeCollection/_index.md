---
title: "ShapeCollection Sınıfı"
linktitle: "ShapeCollection"
second_title: "C++ API Referansı aracılığıyla Go için Aspose.Cells"
description: "ShapeCollection sınıfı. Go'da shapecollection'ı temsil eden nesneyi kapsüller."
type: docs
weight: 200
url: /tr/go-cpp/shapecollection/
---

## ShapeCollection class

Bir çalışma sayfası/çarttaki tüm şekilleri temsil eder.

```go

type ShapeCollection struct  {
	ptr unsafe.Pointer
}

```
## Yapıcılar

| Metot | Açıklama |
| --- | --- |

## Metotlar

| Metot | Açıklama |
| --- | --- |
| [IsNull](./isnull/) | Uygulama nesnesinin nullptr olup olmadığını kontrol eder. |
| [Get_Int](./get_int/) | Listedeki belirli indeksteki Shape nesnesini alır. |
| [Get_String](./get_string/) | Şeklin adıyla Shape nesnesini alır. |
| [AddCopy_Shape_Int_Int_Int_Int](./addcopy_shape_int_int_int_int/) | Çalışma sayfasına bir şekil ekler ve kopyalar. |
| [AddCopy_Shape_Int_Int_Int_Int_CopyOptions](./addcopy_shape_int_int_int_int_copyoptions/) | Çalışma sayfasına bir şekil ekler ve kopyalar. |
| [AddCheckBox](./addcheckbox/) | Çalışma sayfasına bir onay kutusu ekler. |
| [AddTextBox](./addtextbox/) | Çalışma sayfasına bir metin kutusu ekler. |
| [AddEquation](./addequation/) | Çalışma sayfasına bir denklem nesnesi ekler. |
| [AddLaTeXEquation](./addlatexequation/) | Çalışma sayfasına LaTeX formatındaki dizgileri kullanarak bir denklem nesnesi ekler. |
| [AddSpinner](./addspinner/) | Çalışma sayfasına bir Spinner ekler. |
| [AddScrollBar](./addscrollbar/) | Çalışma sayfasına bir ScrollBar ekler. |
| [AddRadioButton](./addradiobutton/) | Çalışma sayfasına bir RadioButton ekler. |
| [AddListBox](./addlistbox/) | Çalışma sayfasına bir ListBox ekler. |
| [AddComboBox](./addcombobox/) | Çalışma sayfasına bir ComboBox ekler. |
| [AddGroupBox](./addgroupbox/) | Çalışma sayfasına bir GroupBox ekler. |
| [AddButton](./addbutton/) | Çalışma sayfasına bir Button ekler. |
| [AddLabel](./addlabel/) | Çalışma sayfasına bir Label ekler. |
| [AddLabelInChart](./addlabelinchart/) | Grafiğe bir label ekler. |
| [AddTextBoxInChart](./addtextboxinchart/) | Grafiğe bir textbox ekler. |
| [AddTextEffectInChart](./addtexteffectinchart/) | Grafiğe bir WordArt nesnesi ekler. |
| [AddTextEffect](./addtexteffect/) | Bir WordArt nesnesi ekler. |
| [AddWordArt](./addwordart/) | Excel 2007'den beri önceden tanımlı WordArt ekler. |
| [AddRectangle](./addrectangle/) | Çalışma sayfasına bir RectangleShape ekler. |
| [AddOval](./addoval/) | Çalışma sayfasına bir Oval ekler. |
| [AddLine](./addline/) | Çalışma sayfasına bir LineShape ekler. |
| [AddFreeFloatingShape](./addfreefloatingshape/) | Çalışma sayfasına serbest yüzen bir şekil ekler. Yalnızca çizgi/görsel şekil için geçerlidir. |
| [AddShapeInChart_MsoDrawingType_PlacementType_Int_Int_Int_Int_Stream](./addshapeinchart_msodrawingtype_placementtype_int_int_int_int_stream/) | Grafiğe bir şekil ekle. Tüm birimler grafik alanının 1/4000'idir. |
| [AddShapeInChart_MsoDrawingType_PlacementType_Int_Int_Int_Int](./addshapeinchart_msodrawingtype_placementtype_int_int_int_int/) | Grafiğe bir şekil ekle. Tüm birimler grafik alanının 1/4000'idir. |
| [AddShapeInChartByScale_MsoDrawingType_PlacementType_Double_Double_Double_Double](./addshapeinchartbyscale_msodrawingtype_placementtype_double_double_double_double/) | Grafiğe bir şekil ekle. Tüm birim grafik alanının yüzde ölçeğidir. |
| [AddShapeInChartByScale_MsoDrawingType_PlacementType_Double_Double_Double_Double_Stream](./addshapeinchartbyscale_msodrawingtype_placementtype_double_double_double_double_stream/) | Grafiğe bir şekil ekle. Tüm birimler grafik alanının 1/4000'idir. |
| [AddArc](./addarc/) | Çalışma sayfasına bir ArcShape ekler. |
| [AddShape](./addshape/) | Çalışma sayfasına bir Shape ekler. |
| [AddAutoShape](./addautoshape/) | Çalışma sayfasına bir AutoShape ekler. |
| [AddAutoShapeInChart](./addautoshapeinchart/) | Grafiğe bir AutoShape ekler. |
| [AddActiveXControl](./addactivexcontrol/) | Bir Activex Control oluşturur. |
| [AddPicture_Int_Int_Int_Int_Stream](./addpicture_int_int_int_int_stream/) | Koleksiyona bir resim ekler. |
| [AddPicture_Int_Int_Stream_Int_Int](./addpicture_int_int_stream_int_int/) | Koleksiyona bir resim ekler. |
| [AddSvg](./addsvg/) | svg görüntüsü ekler. |
| [AddIcons](./addicons/) | svg görüntüsü ekler. |
| [AddLinkedPicture](./addlinkedpicture/) | Bağlantılı bir resim ekle. |
| [AddOleObjectWithLinkedImage](./addoleobjectwithlinkedimage/) | Bağlantılı bir resim ekle. |
| [AddPictureInChart](./addpictureinchart/) | Grafiğe bir resim ekler. |
| [AddOleObject](./addoleobject/) | Bir OleObject ekler. |
| [CopyCommentsInRange](./copycommentsinrange/) | Aralıktaki tüm yorumları kopyala. |
| [CopyInRange](./copyinrange/) | Aralıktaki şekilleri hedef aralığa kopyala. |
| [DeleteInRange](./deleteinrange/) | Aralıktaki şekilleri sil. Yorum şekilleri silinmeyecek. |
| [DeleteShape](./deleteshape/) | Bir şekli sil. Şekil grup içinde ise veya bir yorum şekli ise silinmeyecek. |
| [Group](./group/) | Şekilleri grupla. |
| [Ungroup](./ungroup/) | Şekil öğelerinin grubunu aç. |
| [RemoveAt](./removeat/) | Şekli kaldır. |
| [Remove](./remove/) | Şekli kaldır. |
| [Clear](./clear/) | Çalışma sayfasındaki tüm şekilleri temizle. |
| [UpdateSelectedValue](./updateselectedvalue/) | Seçili değeri, şeklin bağlantılı hücresi veya aralığının değeriyle güncelle. |
| [AddFreeform](./addfreeform/) | Çalışma sayfasına serbest şekil ekler. |
| [AddSignatureLine](./addsignatureline/) | Çalışma sayfasına İmza Satırı ekler. |
| [GetCount](./getcount/) | Örnekte bulunan öğe sayısını alır. |
