---
title: "ShapeCollection Klasse"
linktitle: "ShapeCollection"
second_title: "Aspose.Cells für Go über C++‑API‑Referenz"
description: "ShapeCollection Klasse. Kapselt das Objekt, das shapecollection in Go darstellt."
type: docs
weight: 200
url: /de/go-cpp/shapecollection/
---

## ShapeCollection class

Stellt alle Formen in einem Arbeitsblatt/Diagramm dar.

```go

type ShapeCollection struct  {
	ptr unsafe.Pointer
}

```
## Konstruktoren

| Methode | Beschreibung |
| --- | --- |

## Methoden

| Methode | Beschreibung |
| --- | --- |
| [IsNull](./isnull/) | Überprüft, ob das Implementierungsobjekt nullptr ist. |
| [Get_Int](./get_int/) | Liefert das Shape-Objekt am angegebenen Index in der Liste. |
| [Get_String](./get_string/) | Liefert das Shape-Objekt anhand des Namens des Shapes. |
| [AddCopy_Shape_Int_Int_Int_Int](./addcopy_shape_int_int_int_int/) | Fügt ein Shape hinzu und kopiert es in das Arbeitsblatt. |
| [AddCopy_Shape_Int_Int_Int_Int_CopyOptions](./addcopy_shape_int_int_int_int_copyoptions/) | Fügt ein Shape hinzu und kopiert es in das Arbeitsblatt. |
| [AddCheckBox](./addcheckbox/) | Fügt ein Kontrollkästchen zum Arbeitsblatt hinzu. |
| [AddTextBox](./addtextbox/) | Fügt ein Textfeld zum Arbeitsblatt hinzu. |
| [AddEquation](./addequation/) | Fügt ein Gleichungsobjekt zum Arbeitsblatt hinzu. |
| [AddLaTeXEquation](./addlatexequation/) | Fügt ein Gleichungsobjekt zum Arbeitsblatt hinzu, wobei LaTeX-Formatzeichenfolgen verwendet werden. |
| [AddSpinner](./addspinner/) | Fügt einen Spinner zum Arbeitsblatt hinzu. |
| [AddScrollBar](./addscrollbar/) | Fügt eine Bildlaufleiste zum Arbeitsblatt hinzu. |
| [AddRadioButton](./addradiobutton/) | Fügt einen RadioButton zum Arbeitsblatt hinzu. |
| [AddListBox](./addlistbox/) | Fügt eine ListBox zum Arbeitsblatt hinzu. |
| [AddComboBox](./addcombobox/) | Fügt eine ComboBox zum Arbeitsblatt hinzu. |
| [AddGroupBox](./addgroupbox/) | Fügt eine GroupBox zum Arbeitsblatt hinzu. |
| [AddButton](./addbutton/) | Fügt einen Button zum Arbeitsblatt hinzu. |
| [AddLabel](./addlabel/) | Fügt ein Label zum Arbeitsblatt hinzu. |
| [AddLabelInChart](./addlabelinchart/) | Fügt dem Diagramm eine Beschriftung hinzu. |
| [AddTextBoxInChart](./addtextboxinchart/) | Fügt dem Diagramm ein Textfeld hinzu. |
| [AddTextEffectInChart](./addtexteffectinchart/) | Fügt dem Diagramm ein WordArt-Objekt ein |
| [AddTextEffect](./addtexteffect/) | Fügt ein WordArt-Objekt ein. |
| [AddWordArt](./addwordart/) | Fügt vordefiniertes WordArt seit Excel 2007 hinzu. |
| [AddRectangle](./addrectangle/) | Fügt dem Arbeitsblatt ein RectangleShape hinzu. |
| [AddOval](./addoval/) | Fügt dem Arbeitsblatt ein Oval hinzu. |
| [AddLine](./addline/) | Fügt dem Arbeitsblatt ein LineShape hinzu. |
| [AddFreeFloatingShape](./addfreefloatingshape/) | Fügt dem Arbeitsblatt eine frei schwebende Form hinzu. Gilt nur für Linien-/Bildformen. |
| [AddShapeInChart_MsoDrawingType_PlacementType_Int_Int_Int_Int_Stream](./addshapeinchart_msodrawingtype_placementtype_int_int_int_int_stream/) | Füge dem Diagramm eine Form hinzu. Alle Einheiten sind 1/4000 der Diagrammfläche. |
| [AddShapeInChart_MsoDrawingType_PlacementType_Int_Int_Int_Int](./addshapeinchart_msodrawingtype_placementtype_int_int_int_int/) | Füge dem Diagramm eine Form hinzu. Alle Einheiten sind 1/4000 der Diagrammfläche. |
| [AddShapeInChartByScale_MsoDrawingType_PlacementType_Double_Double_Double_Double](./addshapeinchartbyscale_msodrawingtype_placementtype_double_double_double_double/) | Füge dem Diagramm eine Form hinzu. Alle Einheiten sind prozentual zur Diagrammfläche. |
| [AddShapeInChartByScale_MsoDrawingType_PlacementType_Double_Double_Double_Double_Stream](./addshapeinchartbyscale_msodrawingtype_placementtype_double_double_double_double_stream/) | Füge dem Diagramm eine Form hinzu. Alle Einheiten sind 1/4000 der Diagrammfläche. |
| [AddArc](./addarc/) | Fügt dem Arbeitsblatt ein ArcShape hinzu. |
| [AddShape](./addshape/) | Fügt dem Arbeitsblatt eine Form hinzu. |
| [AddAutoShape](./addautoshape/) | Fügt dem Arbeitsblatt ein AutoShape hinzu. |
| [AddAutoShapeInChart](./addautoshapeinchart/) | Fügt dem Diagramm ein AutoShape hinzu. |
| [AddActiveXControl](./addactivexcontrol/) | Erstellt ein Activex-Steuerelement. |
| [AddPicture_Int_Int_Int_Int_Stream](./addpicture_int_int_int_int_stream/) | Fügt ein Bild zur Sammlung hinzu. |
| [AddPicture_Int_Int_Stream_Int_Int](./addpicture_int_int_stream_int_int/) | Fügt ein Bild zur Sammlung hinzu. |
| [AddSvg](./addsvg/) | Fügt ein SVG-Bild hinzu. |
| [AddIcons](./addicons/) | Fügt ein SVG-Bild hinzu. |
| [AddLinkedPicture](./addlinkedpicture/) | Füge ein verknüpftes Bild hinzu. |
| [AddOleObjectWithLinkedImage](./addoleobjectwithlinkedimage/) | Füge ein verknüpftes Bild hinzu. |
| [AddPictureInChart](./addpictureinchart/) | Fügt dem Diagramm ein Bild hinzu. |
| [AddOleObject](./addoleobject/) | Fügt ein OleObject hinzu. |
| [CopyCommentsInRange](./copycommentsinrange/) | Kopiere alle Kommentare im Bereich. |
| [CopyInRange](./copyinrange/) | Kopiere Formen im Bereich zum Zielbereich. |
| [DeleteInRange](./deleteinrange/) | Lösche Formen im Bereich. Kommentarformen werden nicht gelöscht. |
| [DeleteShape](./deleteshape/) | Lösche eine Form. Wenn die Form in einer Gruppe ist oder eine Kommentarform ist, wird sie nicht gelöscht. |
| [Group](./group/) | Gruppiere die Formen. |
| [Ungroup](./ungroup/) | Entgruppiert die Formelemente. |
| [RemoveAt](./removeat/) | Entferne die Form. |
| [Remove](./remove/) | Entferne die Form. |
| [Clear](./clear/) | Lösche alle Formen im Arbeitsblatt. |
| [UpdateSelectedValue](./updateselectedvalue/) | Aktualisiere den ausgewählten Wert anhand des Werts der verknüpften Zelle oder des Bereichs der Form. |
| [AddFreeform](./addfreeform/) | Fügt dem Arbeitsblatt eine Freihandform hinzu. |
| [AddSignatureLine](./addsignatureline/) | Fügt dem Arbeitsblatt eine Signaturzeile hinzu. |
| [GetCount](./getcount/) | Liefert die Anzahl der im Objekt enthaltenen Elemente. |
