---
title: "ShapeCollection-klass"
linktitle: "ShapeCollection"
second_title: "Aspose.Cells för Go via C++ API-referens"
description: "ShapeCollection-klass. Inkapslar objektet som representerar shapecollection i Go."
type: docs
weight: 200
url: /sv/go-cpp/shapecollection/
---

## ShapeCollection class

Representerar alla former i ett arbetsblad/diagram.

```go

type ShapeCollection struct  {
	ptr unsafe.Pointer
}

```
## Konstruktörer

| Metod | Beskrivning |
| --- | --- |

## Metoder

| Metod | Beskrivning |
| --- | --- |
| [IsNull](./isnull/) | Kontrollerar om implementeringsobjektet är nullptr. |
| [Get_Int](./get_int/) | Hämtar Shape-objektet på det specifika indexet i listan. |
| [Get_String](./get_string/) | Hämtar Shape-objektet efter namnet på formen. |
| [AddCopy_Shape_Int_Int_Int_Int](./addcopy_shape_int_int_int_int/) | Lägger till och kopierar en form till kalkylbladet. |
| [AddCopy_Shape_Int_Int_Int_Int_CopyOptions](./addcopy_shape_int_int_int_int_copyoptions/) | Lägger till och kopierar en form till kalkylbladet. |
| [AddCheckBox](./addcheckbox/) | Lägger till en kryssruta i kalkylbladet. |
| [AddTextBox](./addtextbox/) | Lägger till en textruta i kalkylbladet. |
| [AddEquation](./addequation/) | Lägger till ett ekvationsobjekt i kalkylbladet. |
| [AddLaTeXEquation](./addlatexequation/) | Lägger till ett ekvationsobjekt i kalkylbladet med LaTeX-formatsträngar. |
| [AddSpinner](./addspinner/) | Lägger till en spinner i kalkylbladet. |
| [AddScrollBar](./addscrollbar/) | Lägger till en rullningslist i kalkylbladet. |
| [AddRadioButton](./addradiobutton/) | Lägger till en radioknapp i kalkylbladet. |
| [AddListBox](./addlistbox/) | Lägger till en listbox i kalkylbladet. |
| [AddComboBox](./addcombobox/) | Lägger till en kombinationsruta i kalkylbladet. |
| [AddGroupBox](./addgroupbox/) | Lägger till en gruppbox i kalkylbladet. |
| [AddButton](./addbutton/) | Lägger till en knapp i kalkylbladet. |
| [AddLabel](./addlabel/) | Lägger till en etikett i kalkylbladet. |
| [AddLabelInChart](./addlabelinchart/) | Lägger till en etikett i diagrammet. |
| [AddTextBoxInChart](./addtextboxinchart/) | Lägger till en textruta i diagrammet. |
| [AddTextEffectInChart](./addtexteffectinchart/) | Infogar ett WordArt-objekt i diagrammet |
| [AddTextEffect](./addtexteffect/) | Infogar ett WordArt-objekt. |
| [AddWordArt](./addwordart/) | Lägger till förinställt WordArt sedan Excel 2007. |
| [AddRectangle](./addrectangle/) | Lägger till en RectangleShape i kalkylbladet. |
| [AddOval](./addoval/) | Lägger till en Oval i kalkylbladet. |
| [AddLine](./addline/) | Lägger till en LineShape i kalkylbladet. |
| [AddFreeFloatingShape](./addfreefloatingshape/) | Lägger till en fri flytande form i kalkylbladet. Gäller endast för linje-/bildform. |
| [AddShapeInChart_MsoDrawingType_PlacementType_Int_Int_Int_Int_Stream](./addshapeinchart_msodrawingtype_placementtype_int_int_int_int_stream/) | Lägg till en form i diagrammet. Alla enheter är 1/4000 av diagramområdet. |
| [AddShapeInChart_MsoDrawingType_PlacementType_Int_Int_Int_Int](./addshapeinchart_msodrawingtype_placementtype_int_int_int_int/) | Lägg till en form i diagrammet. Alla enheter är 1/4000 av diagramområdet. |
| [AddShapeInChartByScale_MsoDrawingType_PlacementType_Double_Double_Double_Double](./addshapeinchartbyscale_msodrawingtype_placementtype_double_double_double_double/) | Lägg till en form i diagrammet. Alla enheter är i procentuell skala av diagramområdet. |
| [AddShapeInChartByScale_MsoDrawingType_PlacementType_Double_Double_Double_Double_Stream](./addshapeinchartbyscale_msodrawingtype_placementtype_double_double_double_double_stream/) | Lägg till en form i diagrammet. Alla enheter är 1/4000 av diagramområdet. |
| [AddArc](./addarc/) | Lägger till en ArcShape i kalkylbladet. |
| [AddShape](./addshape/) | Lägger till en Shape i kalkylbladet. |
| [AddAutoShape](./addautoshape/) | Lägger till en AutoShape i kalkylbladet. |
| [AddAutoShapeInChart](./addautoshapeinchart/) | Lägger till en AutoShape i diagrammet. |
| [AddActiveXControl](./addactivexcontrol/) | Skapar en Activex Control. |
| [AddPicture_Int_Int_Int_Int_Stream](./addpicture_int_int_int_int_stream/) | Lägger till en bild i samlingen. |
| [AddPicture_Int_Int_Stream_Int_Int](./addpicture_int_int_stream_int_int/) | Lägger till en bild i samlingen. |
| [AddSvg](./addsvg/) | Lägger till en svg-bild. |
| [AddIcons](./addicons/) | Lägger till en svg-bild. |
| [AddLinkedPicture](./addlinkedpicture/) | Lägg till en länkad bild. |
| [AddOleObjectWithLinkedImage](./addoleobjectwithlinkedimage/) | Lägg till en länkad bild. |
| [AddPictureInChart](./addpictureinchart/) | Lägger till en bild i diagrammet. |
| [AddOleObject](./addoleobject/) | Lägger till ett OleObject. |
| [CopyCommentsInRange](./copycommentsinrange/) | Kopiera alla kommentarer i området. |
| [CopyInRange](./copyinrange/) | Kopiera former i området till målområdet. |
| [DeleteInRange](./deleteinrange/) | Ta bort former i området. Kommentarformer kommer inte att tas bort. |
| [DeleteShape](./deleteshape/) | Ta bort en form. Om formen är i en grupp eller är en kommentarform, kommer den inte att tas bort. |
| [Group](./group/) | Gruppera formerna. |
| [Ungroup](./ungroup/) | Avgruppera formobjekten. |
| [RemoveAt](./removeat/) | Ta bort formen. |
| [Remove](./remove/) | Ta bort formen. |
| [Clear](./clear/) | Rensa alla former i kalkylbladet. |
| [UpdateSelectedValue](./updateselectedvalue/) | Uppdatera det valda värdet med värdet från den länkade cellen eller området för formen. |
| [AddFreeform](./addfreeform/) | Lägger till en frihandsform i kalkylbladet. |
| [AddSignatureLine](./addsignatureline/) | Lägger till en Signature Line i kalkylbladet. |
| [GetCount](./getcount/) | Hämtar antalet element som finns i instansen. |
