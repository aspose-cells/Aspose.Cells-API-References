---
title: "Classe ShapeCollection"
linktitle: "ShapeCollection"
second_title: "Riferimento API C++ di Aspose.Cells per Go"
description: "Classe ShapeCollection. Incapsula l'oggetto che rappresenta shapecollection in Go."
type: docs
weight: 200
url: /it/go-cpp/shapecollection/
---

## ShapeCollection class

Rappresenta tutte le forme in un foglio di lavoro/grafico.

```go

type ShapeCollection struct  {
	ptr unsafe.Pointer
}

```
## Costruttori

| Metodo | Descrizione |
| --- | --- |

## Metodi

| Metodo | Descrizione |
| --- | --- |
| [IsNull](./isnull/) | Verifica se l'oggetto di implementazione è nullptr. |
| [Get_Int](./get_int/) | Ottiene l'oggetto Shape all'indice specifico nella lista. |
| [Get_String](./get_string/) | Ottiene l'oggetto Shape per il nome della forma. |
| [AddCopy_Shape_Int_Int_Int_Int](./addcopy_shape_int_int_int_int/) | Aggiunge e copia una forma nel foglio di lavoro. |
| [AddCopy_Shape_Int_Int_Int_Int_CopyOptions](./addcopy_shape_int_int_int_int_copyoptions/) | Aggiunge e copia una forma nel foglio di lavoro. |
| [AddCheckBox](./addcheckbox/) | Aggiunge una casella di controllo al foglio di lavoro. |
| [AddTextBox](./addtextbox/) | Aggiunge una casella di testo al foglio di lavoro. |
| [AddEquation](./addequation/) | Aggiunge un oggetto equazione al foglio di lavoro. |
| [AddLaTeXEquation](./addlatexequation/) | Aggiunge un oggetto equazione al foglio di lavoro usando stringhe in formato LaTeX. |
| [AddSpinner](./addspinner/) | Aggiunge uno Spinner al foglio di lavoro. |
| [AddScrollBar](./addscrollbar/) | Aggiunge una ScrollBar al foglio di lavoro. |
| [AddRadioButton](./addradiobutton/) | Aggiunge un RadioButton al foglio di lavoro. |
| [AddListBox](./addlistbox/) | Aggiunge una ListBox al foglio di lavoro. |
| [AddComboBox](./addcombobox/) | Aggiunge una ComboBox al foglio di lavoro. |
| [AddGroupBox](./addgroupbox/) | Aggiunge una GroupBox al foglio di lavoro. |
| [AddButton](./addbutton/) | Aggiunge un Button al foglio di lavoro. |
| [AddLabel](./addlabel/) | Aggiunge un Label al foglio di lavoro. |
| [AddLabelInChart](./addlabelinchart/) | Aggiunge una etichetta al grafico. |
| [AddTextBoxInChart](./addtextboxinchart/) | Aggiunge una casella di testo al grafico. |
| [AddTextEffectInChart](./addtexteffectinchart/) | Inserisce un oggetto WordArt al grafico |
| [AddTextEffect](./addtexteffect/) | Inserisce un oggetto WordArt. |
| [AddWordArt](./addwordart/) | Aggiunge WordArt predefinito da Excel 2007.s |
| [AddRectangle](./addrectangle/) | Aggiunge una RectangleShape al foglio di lavoro. |
| [AddOval](./addoval/) | Aggiunge un Ovale al foglio di lavoro. |
| [AddLine](./addline/) | Aggiunge una LineShape al foglio di lavoro. |
| [AddFreeFloatingShape](./addfreefloatingshape/) | Aggiunge una forma fluttuante al foglio di lavoro.Si applica solo per forme linea/immagine. |
| [AddShapeInChart_MsoDrawingType_PlacementType_Int_Int_Int_Int_Stream](./addshapeinchart_msodrawingtype_placementtype_int_int_int_int_stream/) | Aggiungi una forma al grafico .Tutte le unità sono 1/4000 dell'area del grafico. |
| [AddShapeInChart_MsoDrawingType_PlacementType_Int_Int_Int_Int](./addshapeinchart_msodrawingtype_placementtype_int_int_int_int/) | Aggiungi una forma al grafico .Tutte le unità sono 1/4000 dell'area del grafico. |
| [AddShapeInChartByScale_MsoDrawingType_PlacementType_Double_Double_Double_Double](./addshapeinchartbyscale_msodrawingtype_placementtype_double_double_double_double/) | Aggiungi una forma al grafico. Tutte le unità sono in scala percentuale dell'area del grafico. |
| [AddShapeInChartByScale_MsoDrawingType_PlacementType_Double_Double_Double_Double_Stream](./addshapeinchartbyscale_msodrawingtype_placementtype_double_double_double_double_stream/) | Aggiungi una forma al grafico .Tutte le unità sono 1/4000 dell'area del grafico. |
| [AddArc](./addarc/) | Aggiunge una ArcShape al foglio di lavoro. |
| [AddShape](./addshape/) | Aggiunge una Shape al foglio di lavoro. |
| [AddAutoShape](./addautoshape/) | Aggiunge una AutoShape al foglio di lavoro. |
| [AddAutoShapeInChart](./addautoshapeinchart/) | Aggiunge una AutoShape al grafico. |
| [AddActiveXControl](./addactivexcontrol/) | Crea un controllo Activex. |
| [AddPicture_Int_Int_Int_Int_Stream](./addpicture_int_int_int_int_stream/) | Aggiunge un'immagine alla collezione. |
| [AddPicture_Int_Int_Stream_Int_Int](./addpicture_int_int_stream_int_int/) | Aggiunge un'immagine alla collezione. |
| [AddSvg](./addsvg/) | Aggiunge un'immagine svg. |
| [AddIcons](./addicons/) | Aggiunge un'immagine svg. |
| [AddLinkedPicture](./addlinkedpicture/) | Aggiungi un'immagine collegata. |
| [AddOleObjectWithLinkedImage](./addoleobjectwithlinkedimage/) | Aggiungi un'immagine collegata. |
| [AddPictureInChart](./addpictureinchart/) | Aggiunge un'immagine al grafico. |
| [AddOleObject](./addoleobject/) | Aggiunge un OleObject. |
| [CopyCommentsInRange](./copycommentsinrange/) | Copia tutti i commenti nell'intervallo. |
| [CopyInRange](./copyinrange/) | Copia le forme nell'intervallo all'intervallo di destinazione. |
| [DeleteInRange](./deleteinrange/) | Elimina le forme nell'intervallo.Comment le forme dei commenti non verranno eliminate. |
| [DeleteShape](./deleteshape/) | Elimina una forma. Se la forma è nel gruppo o è una forma di commento, non verrà eliminata. |
| [Group](./group/) | Raggruppa le forme. |
| [Ungroup](./ungroup/) | Separa gli elementi della forma. |
| [RemoveAt](./removeat/) | Rimuovi la forma. |
| [Remove](./remove/) | Rimuovi la forma. |
| [Clear](./clear/) | Cancella tutte le forme nel foglio di lavoro. |
| [UpdateSelectedValue](./updateselectedvalue/) | Aggiorna il valore selezionato con il valore della cella collegata o dell'intervallo della forma. |
| [AddFreeform](./addfreeform/) | Aggiunge una forma libera al foglio di lavoro. |
| [AddSignatureLine](./addsignatureline/) | Aggiunge una linea di firma al foglio di lavoro. |
| [GetCount](./getcount/) | Ottiene il numero di elementi contenuti nell'istanza. |
