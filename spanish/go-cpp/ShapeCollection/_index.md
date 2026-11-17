---
title: "Clase ShapeCollection"
linktitle: "ShapeCollection"
second_title: "Aspose.Cells for Go via C++ API Reference"
description: "Clase ShapeCollection. Encapsula el objeto que representa shapecollection en Go."
type: docs
weight: 200
url: /es/go-cpp/shapecollection/
---

## ShapeCollection class

Represents all the shape in a worksheet/chart.

```go

type ShapeCollection struct  {
	ptr unsafe.Pointer
}

```
## Constructors

| Method | Description |
| --- | --- |

## Methods

| Method | Description |
| --- | --- |
| [IsNull](./isnull/) | Checks whether the implementation object is nullptr. |
| [Get_Int](./get_int/) | Obtiene el objeto Shape en el índice específico de la lista. |
| [Get_String](./get_string/) | Obtiene el objeto Shape por el nombre de la forma. |
| [AddCopy_Shape_Int_Int_Int_Int](./addcopy_shape_int_int_int_int/) | Añade y copia una forma a la hoja de cálculo. |
| [AddCopy_Shape_Int_Int_Int_Int_CopyOptions](./addcopy_shape_int_int_int_int_copyoptions/) | Añade y copia una forma a la hoja de cálculo. |
| [AddCheckBox](./addcheckbox/) | Añade una casilla de verificación a la hoja de cálculo. |
| [AddTextBox](./addtextbox/) | Añade un cuadro de texto a la hoja de cálculo. |
| [AddEquation](./addequation/) | Añade un objeto de ecuación a la hoja de cálculo. |
| [AddLaTeXEquation](./addlatexequation/) | Agrega un objeto de ecuación a la hoja de cálculo usando cadenas con formato LaTeX. |
| [AddSpinner](./addspinner/) | Agrega un Spinner a la hoja de cálculo. |
| [AddScrollBar](./addscrollbar/) | Agrega un ScrollBar a la hoja de cálculo. |
| [AddRadioButton](./addradiobutton/) | Agrega un RadioButton a la hoja de cálculo. |
| [AddListBox](./addlistbox/) | Agrega un ListBox a la hoja de cálculo. |
| [AddComboBox](./addcombobox/) | Agrega un ComboBox a la hoja de cálculo. |
| [AddGroupBox](./addgroupbox/) | Agrega un GroupBox a la hoja de cálculo. |
| [AddButton](./addbutton/) | Agrega un Button a la hoja de cálculo. |
| [AddLabel](./addlabel/) | Agrega un Label a la hoja de cálculo. |
| [AddLabelInChart](./addlabelinchart/) | Agrega un label al gráfico. |
| [AddTextBoxInChart](./addtextboxinchart/) | Agrega un textbox al gráfico. |
| [AddTextEffectInChart](./addtexteffectinchart/) | Inserta un objeto WordArt al gráfico |
| [AddTextEffect](./addtexteffect/) | Inserta un objeto WordArt. |
| [AddWordArt](./addwordart/) | Agrega WordArt predefinido desde Excel 2007. |
| [AddRectangle](./addrectangle/) | Agrega un RectangleShape a la hoja de cálculo. |
| [AddOval](./addoval/) | Agrega un Oval a la hoja de cálculo. |
| [AddLine](./addline/) | Agrega un LineShape a la hoja de cálculo. |
| [AddFreeFloatingShape](./addfreefloatingshape/) | Agrega una forma flotante libre a la hoja de cálculo. Solo se aplica a formas de línea/imagen. |
| [AddShapeInChart_MsoDrawingType_PlacementType_Int_Int_Int_Int_Stream](./addshapeinchart_msodrawingtype_placementtype_int_int_int_int_stream/) | Agrega una forma al gráfico. Todas las unidades son 1/4000 del área del gráfico. |
| [AddShapeInChart_MsoDrawingType_PlacementType_Int_Int_Int_Int](./addshapeinchart_msodrawingtype_placementtype_int_int_int_int/) | Agrega una forma al gráfico. Todas las unidades son 1/4000 del área del gráfico. |
| [AddShapeInChartByScale_MsoDrawingType_PlacementType_Double_Double_Double_Double](./addshapeinchartbyscale_msodrawingtype_placementtype_double_double_double_double/) | Agrega una forma al gráfico. Todas las unidades son escala porcentual del área del gráfico. |
| [AddShapeInChartByScale_MsoDrawingType_PlacementType_Double_Double_Double_Double_Stream](./addshapeinchartbyscale_msodrawingtype_placementtype_double_double_double_double_stream/) | Agrega una forma al gráfico. Todas las unidades son 1/4000 del área del gráfico. |
| [AddArc](./addarc/) | Agrega un ArcShape a la hoja de cálculo. |
| [AddShape](./addshape/) | Agrega una Shape a la hoja de cálculo. |
| [AddAutoShape](./addautoshape/) | Agrega un AutoShape a la hoja de cálculo. |
| [AddAutoShapeInChart](./addautoshapeinchart/) | Agrega un AutoShape al gráfico. |
| [AddActiveXControl](./addactivexcontrol/) | Crea un control Activex. |
| [AddPicture_Int_Int_Int_Int_Stream](./addpicture_int_int_int_int_stream/) | Adds a picture to the collection. |
| [AddPicture_Int_Int_Stream_Int_Int](./addpicture_int_int_stream_int_int/) | Adds a picture to the collection. |
| [AddSvg](./addsvg/) | Agrega una imagen svg. |
| [AddIcons](./addicons/) | Agrega una imagen svg. |
| [AddLinkedPicture](./addlinkedpicture/) | Agrega una imagen vinculada. |
| [AddOleObjectWithLinkedImage](./addoleobjectwithlinkedimage/) | Agrega una imagen vinculada. |
| [AddPictureInChart](./addpictureinchart/) | Agrega una imagen al gráfico. |
| [AddOleObject](./addoleobject/) | Agrega un OleObject. |
| [CopyCommentsInRange](./copycommentsinrange/) | Copiar todos los comentarios en el rango. |
| [CopyInRange](./copyinrange/) | Copiar formas en el rango al rango de destino. |
| [DeleteInRange](./deleteinrange/) | Eliminar formas en el rango. Las formas de comentario no se eliminarán. |
| [DeleteShape](./deleteshape/) | Eliminar una forma. Si la forma está en el grupo o es una forma de comentario, no se eliminará. |
| [Group](./group/) | Agrupar las formas. |
| [Ungroup](./ungroup/) | Desagrupar los elementos de forma. |
| [RemoveAt](./removeat/) | Eliminar la forma. |
| [Remove](./remove/) | Eliminar la forma. |
| [Clear](./clear/) | Borrar todas las formas en la hoja de cálculo. |
| [UpdateSelectedValue](./updateselectedvalue/) | Actualizar el valor seleccionado con el valor de la celda vinculada o del rango de la forma. |
| [AddFreeform](./addfreeform/) | Agrega una forma libre a la hoja de cálculo. |
| [AddSignatureLine](./addsignatureline/) | Agrega una línea de firma a la hoja de cálculo. |
| [GetCount](./getcount/) | Gets the number of elements contained in the instance. |
