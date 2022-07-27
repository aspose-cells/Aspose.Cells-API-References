---
title: ShapeCollection
second_title: Referencia de API de Aspose.Cells para .NET
description: Representa todas las formas en una hoja de cálculo/gráfico.
type: docs
weight: 2650
url: /es/net/aspose.cells.drawing/shapecollection/
---
## ShapeCollection class

Representa todas las formas en una hoja de cálculo/gráfico.

```csharp
public class ShapeCollection : CollectionBase<Shape>
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase`1/capacity) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase`1/count) { get; } |  |
| [Item](../../aspose.cells.drawing/shapecollection/item) { get; } | Obtiene el objeto de forma en el índice específico. (2 indexers) |
| [Item](../../aspose.cells/collectionbase`1/item) { get; set; } |  |

## Métodos

| Nombre | Descripción |
| --- | --- |
| [AddActiveXControl](../../aspose.cells.drawing/shapecollection/addactivexcontrol)(ControlType, int, int, int, int, int, int) | Crea un Control Activex. |
| [AddArc](../../aspose.cells.drawing/shapecollection/addarc)(int, int, int, int, int, int) | Agrega un ArcShape a la hoja de trabajo. |
| [AddAutoShape](../../aspose.cells.drawing/shapecollection/addautoshape)(AutoShapeType, int, int, int, int, int, int) | Agrega una autoforma a la hoja de trabajo. |
| [AddAutoShapeInChart](../../aspose.cells.drawing/shapecollection/addautoshapeinchart)(AutoShapeType, int, int, int, int) | Agrega una autoforma al gráfico. |
| [AddButton](../../aspose.cells.drawing/shapecollection/addbutton)(int, int, int, int, int, int) | Agrega un Botón a la hoja de cálculo. |
| [AddCheckBox](../../aspose.cells.drawing/shapecollection/addcheckbox)(int, int, int, int, int, int) | Agrega una casilla de verificación a la hoja de cálculo. |
| [AddComboBox](../../aspose.cells.drawing/shapecollection/addcombobox)(int, int, int, int, int, int) | Agrega un ComboBox a la hoja de trabajo. |
| [AddCopy](../../aspose.cells.drawing/shapecollection/addcopy)(Shape, int, int, int, int) | Agrega y copia una forma a la hoja de trabajo. |
| [AddFreeFloatingShape](../../aspose.cells.drawing/shapecollection/addfreefloatingshape)(MsoDrawingType, int, int, int, int, byte[], bool) | Agrega una forma flotante libre a la hoja de cálculo. Solo se aplica a la forma de línea/imagen. |
| [AddGroupBox](../../aspose.cells.drawing/shapecollection/addgroupbox)(int, int, int, int, int, int) | Agrega un GroupBox a la hoja de trabajo. |
| [AddIcons](../../aspose.cells.drawing/shapecollection/addicons)(int, int, int, int, int, int, byte[], byte[]) | Agrega imagen svg. |
| [AddLabel](../../aspose.cells.drawing/shapecollection/addlabel)(int, int, int, int, int, int) | Agrega una etiqueta a la hoja de cálculo. |
| [AddLabelInChart](../../aspose.cells.drawing/shapecollection/addlabelinchart)(int, int, int, int) | Agrega una etiqueta al gráfico. |
| [AddLine](../../aspose.cells.drawing/shapecollection/addline)(int, int, int, int, int, int) | Agrega una forma de línea a la hoja de trabajo. |
| [AddLinkedPicture](../../aspose.cells.drawing/shapecollection/addlinkedpicture)(int, int, int, int, string) | Agregar una imagen vinculada. |
| [AddListBox](../../aspose.cells.drawing/shapecollection/addlistbox)(int, int, int, int, int, int) | Agrega un ListBox a la hoja de trabajo. |
| [AddOleObject](../../aspose.cells.drawing/shapecollection/addoleobject)(int, int, int, int, int, int, byte[]) |  |
| [AddOleObjectWithLinkedImage](../../aspose.cells.drawing/shapecollection/addoleobjectwithlinkedimage)(int, int, int, int, string) | Agregar una imagen vinculada. |
| [AddOval](../../aspose.cells.drawing/shapecollection/addoval)(int, int, int, int, int, int) | Agrega un óvalo a la hoja de cálculo. |
| [AddPicture](../../aspose.cells.drawing/shapecollection/addpicture#addpicture)(int, int, int, int, Stream) | Agrega una imagen a la colección. |
| [AddPicture](../../aspose.cells.drawing/shapecollection/addpicture#addpicture_1)(int, int, Stream, int, int) | Agrega una imagen a la colección. |
| [AddPictureInChart](../../aspose.cells.drawing/shapecollection/addpictureinchart)(int, int, Stream, int, int) | Agrega una imagen al gráfico. |
| [AddRadioButton](../../aspose.cells.drawing/shapecollection/addradiobutton)(int, int, int, int, int, int) | Agrega un RadioButton a la hoja de trabajo. |
| [AddRectangle](../../aspose.cells.drawing/shapecollection/addrectangle)(int, int, int, int, int, int) | Agrega un RectangleShape a la hoja de trabajo. |
| [AddScrollBar](../../aspose.cells.drawing/shapecollection/addscrollbar)(int, int, int, int, int, int) | Agrega una barra de desplazamiento a la hoja de cálculo. |
| [AddShape](../../aspose.cells.drawing/shapecollection/addshape)(MsoDrawingType, int, int, int, int, int, int) | Agrega una Forma a la hoja de cálculo. |
| [AddShapeInChart](../../aspose.cells.drawing/shapecollection/addshapeinchart#addshapeinchart)(MsoDrawingType, PlacementType, int, int, int, int) | Agregue una forma al gráfico. Todas las unidades son 1/4000 del área del gráfico. |
| [AddShapeInChart](../../aspose.cells.drawing/shapecollection/addshapeinchart#addshapeinchart_1)(MsoDrawingType, PlacementType, int, int, int, int, byte[]) | Agregue una forma al gráfico. Todas las unidades son 1/4000 del área del gráfico. |
| [AddShapeInChartByScale](../../aspose.cells.drawing/shapecollection/addshapeinchartbyscale#addshapeinchartbyscale)(MsoDrawingType, PlacementType, double, double, double, double) | Agrega una forma al gráfico. Todas las unidades son la escala porcentual del área del gráfico. |
| [AddShapeInChartByScale](../../aspose.cells.drawing/shapecollection/addshapeinchartbyscale#addshapeinchartbyscale_1)(MsoDrawingType, PlacementType, double, double, double, double, byte[]) | Agregue una forma al gráfico. Todas las unidades son 1/4000 del área del gráfico. |
| [AddSpinner](../../aspose.cells.drawing/shapecollection/addspinner)(int, int, int, int, int, int) | Agrega un Spinner a la hoja de trabajo. |
| [AddSvg](../../aspose.cells.drawing/shapecollection/addsvg)(int, int, int, int, int, int, byte[], byte[]) | Agrega imagen svg. |
| [AddTextBox](../../aspose.cells.drawing/shapecollection/addtextbox)(int, int, int, int, int, int) | Agrega un cuadro de texto a la hoja de cálculo. |
| [AddTextBoxInChart](../../aspose.cells.drawing/shapecollection/addtextboxinchart)(int, int, int, int) | Agrega un cuadro de texto al gráfico. |
| [AddTextEffect](../../aspose.cells.drawing/shapecollection/addtexteffect)(MsoPresetTextEffect, string, string, int, bool, bool, int, int, int, int, int, int) | Inserta un objeto de WordArt. |
| [AddTextEffectInChart](../../aspose.cells.drawing/shapecollection/addtexteffectinchart)(MsoPresetTextEffect, string, string, int, bool, bool, int, int, int, int) | Inserta un objeto de WordArt en el gráfico |
| [AddWordArt](../../aspose.cells.drawing/shapecollection/addwordart)(PresetWordArtStyle, string, int, int, int, int, int, int) | Agrega WordArt predeterminado desde Excel 2007.s |
| [BinarySearch](../../aspose.cells/collectionbase`1/binarysearch)(Shape) |  |
| [BinarySearch](../../aspose.cells/collectionbase`1/binarysearch)(Shape, IComparer&lt;Shape&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase`1/binarysearch)(int, int, Shape, IComparer&lt;Shape&gt;) |  |
| [Clear](../../aspose.cells.drawing/shapecollection/clear#clear)() | Borrar todas las formas. (2 methods) |
| [Contains](../../aspose.cells/collectionbase`1/contains)(Shape) |  |
| [CopyCommentsInRange](../../aspose.cells.drawing/shapecollection/copycommentsinrange)(ShapeCollection, CellArea, int, int) | Copia todos los comentarios del rango. |
| [CopyInRange](../../aspose.cells.drawing/shapecollection/copyinrange)(ShapeCollection, CellArea, int, int, bool) | Copie formas en el rango al rango de destino. |
| [CopyTo](../../aspose.cells/collectionbase`1/copyto)(Shape[]) |  |
| [CopyTo](../../aspose.cells/collectionbase`1/copyto)(Shape[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase`1/copyto)(int, Shape[], int, int) |  |
| [DeleteInRange](../../aspose.cells.drawing/shapecollection/deleteinrange)(CellArea) | Eliminar formas en el rango. Las formas de comentarios no se eliminarán. |
| [DeleteShape](../../aspose.cells.drawing/shapecollection/deleteshape)(Shape) | Eliminar una forma. Si la forma está en el grupo o es una forma de comentario, no se eliminará. |
| [Exists](../../aspose.cells/collectionbase`1/exists)(Predicate&lt;Shape&gt;) |  |
| [Find](../../aspose.cells/collectionbase`1/find)(Predicate&lt;Shape&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase`1/findall)(Predicate&lt;Shape&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase`1/findindex)(Predicate&lt;Shape&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase`1/findindex)(int, Predicate&lt;Shape&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase`1/findindex)(int, int, Predicate&lt;Shape&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase`1/findlast)(Predicate&lt;Shape&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase`1/findlastindex)(Predicate&lt;Shape&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase`1/findlastindex)(int, Predicate&lt;Shape&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase`1/findlastindex)(int, int, Predicate&lt;Shape&gt;) |  |
| [GetEnumerator](../../aspose.cells/collectionbase`1/getenumerator)() |  |
| [Group](../../aspose.cells.drawing/shapecollection/group)(Shape[]) | Agrupa las formas. |
| [IndexOf](../../aspose.cells/collectionbase`1/indexof)(Shape) |  |
| [IndexOf](../../aspose.cells/collectionbase`1/indexof)(Shape, int) |  |
| [IndexOf](../../aspose.cells/collectionbase`1/indexof)(Shape, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase`1/lastindexof)(Shape) |  |
| [LastIndexOf](../../aspose.cells/collectionbase`1/lastindexof)(Shape, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase`1/lastindexof)(Shape, int, int) |  |
| [Remove](../../aspose.cells.drawing/shapecollection/remove)(Shape) | Eliminar la forma. |
| [RemoveAt](../../aspose.cells.drawing/shapecollection/removeat#removeat)(int) | Eliminar la forma. (2 methods) |
| [Ungroup](../../aspose.cells.drawing/shapecollection/ungroup)(GroupShape) | Desagrupa los elementos de forma. |
| [UpdateSelectedValue](../../aspose.cells.drawing/shapecollection/updateselectedvalue)() | Actualiza el valor seleccionado por el valor de la celda vinculada de las formas. |

### Ejemplos

```csharp

[C#]

// Instanciando un objeto Workbook
Workbook workbook = new Workbook();

// obtener ShapeCollection
ShapeCollection shapes = workbook.Worksheets[0].Shapes;

//haz tu negocio

//Guardar el archivo de Excel.
workbook.Save("result.xlsx");
```

### Ver también

* class [CollectionBase&lt;T&gt;](../../aspose.cells/collectionbase-1)
* class [Shape](../shape)
* espacio de nombres [Aspose.Cells.Drawing](../../aspose.cells.drawing)
* asamblea [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
