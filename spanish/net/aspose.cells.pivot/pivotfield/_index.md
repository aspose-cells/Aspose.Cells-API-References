---
title: PivotField
second_title: Referencia de API de Aspose.Cells para .NET
description: Representa un campo en un informe de tabla dinámica.
type: docs
weight: 4530
url: /es/net/aspose.cells.pivot/pivotfield/
---
## PivotField class

Representa un campo en un informe de tabla dinámica.

```csharp
public class PivotField
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [AutoShowCount](../../aspose.cells.pivot/pivotfield/autoshowcount) { get; set; } | Representa el número de elementos superiores o inferiores que se muestran automáticamente en el campo de tabla dinámica especificado. |
| [AutoShowField](../../aspose.cells.pivot/pivotfield/autoshowfield) { get; set; } | Representa el índice de campo de exhibición automática. -1 significa PivotField en sí mismo. Debe ser el índice de los campos de datos. |
| [AutoSortField](../../aspose.cells.pivot/pivotfield/autosortfield) { get; set; } | Representa el índice de campo de clasificación automática. -1 significa PivotField en sí mismo, otros significa la posición de los campos de datos. |
| [BaseFieldIndex](../../aspose.cells.pivot/pivotfield/basefieldindex) { get; set; } | Representa el campo base para un cálculo personalizado. |
| [BaseIndex](../../aspose.cells.pivot/pivotfield/baseindex) { get; set; } | Representa el índice de PivotField en la base PivotFields. |
| [BaseItemIndex](../../aspose.cells.pivot/pivotfield/baseitemindex) { get; set; } | Representa el elemento en el campo base para un cálculo personalizado. Válido solo para campos de datos. |
| [BaseItemPosition](../../aspose.cells.pivot/pivotfield/baseitemposition) { get; set; } | Representa el elemento en el campo base para un cálculo personalizado. Válido solo para campos de datos. Debido a que PivotItemPosition.Custom es solo para lectura, si necesita configurar PivotItemPosition.Custom, , configure PivotField.BaseItemIndex atributo. |
| [CurrentPageItem](../../aspose.cells.pivot/pivotfield/currentpageitem) { get; set; } | Representa el elemento de página actual que se muestra para el campo de página (válido solo para campos de página). |
| [DataDisplayFormat](../../aspose.cells.pivot/pivotfield/datadisplayformat) { get; set; } | Representa cómo mostrar los valores contenidos en un campo de datos. |
| [DisplayName](../../aspose.cells.pivot/pivotfield/displayname) { get; set; } | Representa el nombre para mostrar de PivotField. |
| [DragToColumn](../../aspose.cells.pivot/pivotfield/dragtocolumn) { get; set; } | Indica si el campo especificado se puede arrastrar a la posición de la columna. El valor predeterminado es verdadero. |
| [DragToData](../../aspose.cells.pivot/pivotfield/dragtodata) { get; set; } | Indica si el campo especificado se puede arrastrar a la posición de datos. El valor predeterminado es verdadero. |
| [DragToHide](../../aspose.cells.pivot/pivotfield/dragtohide) { get; set; } | Indica si el campo especificado se puede arrastrar a la posición oculta. El valor predeterminado es verdadero. |
| [DragToPage](../../aspose.cells.pivot/pivotfield/dragtopage) { get; set; } | Indica si el campo especificado se puede arrastrar a la posición de la página. El valor predeterminado es verdadero. |
| [DragToRow](../../aspose.cells.pivot/pivotfield/dragtorow) { get; set; } | Indica si el campo especificado se puede arrastrar a la posición de la fila. El valor predeterminado es verdadero. |
| [Function](../../aspose.cells.pivot/pivotfield/function) { get; set; } | Representa la función utilizada para resumir el campo de datos de la tabla dinámica. |
| [InsertBlankRow](../../aspose.cells.pivot/pivotfield/insertblankrow) { get; set; } | Indica si se inserta una línea en blanco después de cada elemento. |
| [IsAscendShow](../../aspose.cells.pivot/pivotfield/isascendshow) { get; set; } | Indica si el campo de tabla dinámica especificado se muestra automáticamente de forma ascendente. |
| [IsAscendSort](../../aspose.cells.pivot/pivotfield/isascendsort) { get; set; } | Indica si el campo de tabla dinámica especificado se ordena automáticamente de forma ascendente. |
| [IsAutoShow](../../aspose.cells.pivot/pivotfield/isautoshow) { get; set; } | Indica si el campo de tabla dinámica especificado se muestra automáticamente, solo válido para excel 2003. |
| [IsAutoSort](../../aspose.cells.pivot/pivotfield/isautosort) { get; set; } | Indica si el campo de tabla dinámica especificado se ordena automáticamente. |
| [IsAutoSubtotals](../../aspose.cells.pivot/pivotfield/isautosubtotals) { get; set; } | Indica si el campo especificado muestra subtotales automáticos. El valor predeterminado es verdadero. |
| [IsCalculatedField](../../aspose.cells.pivot/pivotfield/iscalculatedfield) { get; } | Indica si el campo de tabla dinámica especificado es un campo calculado. |
| [IsIncludeNewItemsInFilter](../../aspose.cells.pivot/pivotfield/isincludenewitemsinfilter) { get; set; } | indica si el campo puede incluir nuevos elementos en el filtro manual El valor predeterminado es falso. |
| [IsInsertPageBreaksBetweenItems](../../aspose.cells.pivot/pivotfield/isinsertpagebreaksbetweenitems) { get; set; } | indica si el campo puede insertar saltos de página entre elementos insertar salto de página después de cada elemento El valor predeterminado es falso. |
| [IsMultipleItemSelectionAllowed](../../aspose.cells.pivot/pivotfield/ismultipleitemselectionallowed) { get; set; } | indica si el campo puede tener varios elementos seleccionados en la página field El valor predeterminado es falso. |
| [IsRepeatItemLabels](../../aspose.cells.pivot/pivotfield/isrepeatitemlabels) { get; set; } | indica si el campo puede repetir elementos label El valor predeterminado es falso. |
| [ItemCount](../../aspose.cells.pivot/pivotfield/itemcount) { get; } | Obtiene el recuento de elementos base de este campo pivote. |
| [Items](../../aspose.cells.pivot/pivotfield/items) { get; } | Consigue todos los elementos básicos; |
| [Name](../../aspose.cells.pivot/pivotfield/name) { get; } | Representa el nombre de PivotField. |
| [Number](../../aspose.cells.pivot/pivotfield/number) { get; set; } | Representa el formato de visualización integrado de números y fechas. |
| [NumberFormat](../../aspose.cells.pivot/pivotfield/numberformat) { get; set; } | Representa el formato de visualización personalizado de números y fechas. |
| [OriginalItems](../../aspose.cells.pivot/pivotfield/originalitems) { get; } | Consigue los elementos base originales; |
| [PivotItems](../../aspose.cells.pivot/pivotfield/pivotitems) { get; } | Obtiene los elementos pivote del campo pivote |
| [Position](../../aspose.cells.pivot/pivotfield/position) { get; } | Representa el índice PivotField en PivotFields. |
| [Range](../../aspose.cells.pivot/pivotfield/range) { get; } | Obtiene el rango de grupo del campo pivote |
| [ShowAllItems](../../aspose.cells.pivot/pivotfield/showallitems) { get; set; } | Indica si se muestran todos los elementos del informe de tabla dinámica, incluso si no contienen datos de resumen. mostrar elementos sin datos El valor predeterminado es falso. |
| [ShowCompact](../../aspose.cells.pivot/pivotfield/showcompact) { get; set; } | Indica si se muestran etiquetas del siguiente campo en la misma columna en la vista de tabla dinámica |
| [ShowInOutlineForm](../../aspose.cells.pivot/pivotfield/showinoutlineform) { get; set; } | Indica si el diseño de este campo en forma de esquema en la vista de tabla dinámica |
| [ShowSubtotalAtTop](../../aspose.cells.pivot/pivotfield/showsubtotalattop) { get; set; } | cuando ShowInOutlineForm es verdadero, luego muestra los subtotales en la parte superior de la lista de elementos en lugar de en la parte inferior |

## Métodos

| Nombre | Descripción |
| --- | --- |
| [AddCalculatedItem](../../aspose.cells.pivot/pivotfield/addcalculateditem)(string, string) | Agregue un elemento calculado al campo dinámico. |
| [GetCalculatedFieldFormula](../../aspose.cells.pivot/pivotfield/getcalculatedfieldformula)() | Obtener la cadena de fórmula del campo calculado especificado . |
| [GetPivotFilterByType](../../aspose.cells.pivot/pivotfield/getpivotfilterbytype)(PivotFilterType) | Obtiene el filtro dinámico del campo dinámico por tipo |
| [GetPivotFilters](../../aspose.cells.pivot/pivotfield/getpivotfilters)() | Obtiene los filtros pivote del campo pivote |
| [GetSubtotals](../../aspose.cells.pivot/pivotfield/getsubtotals)(PivotFieldSubtotalType) | Obtiene si el campo especificado muestra esos subtotales. |
| [HideDetail](../../aspose.cells.pivot/pivotfield/hidedetail)(bool) | Establece si los PivotItems en un campo dinámico son detalles ocultos. Es decir, contraer/expandir este campo. |
| [HideItem](../../aspose.cells.pivot/pivotfield/hideitem#hideitem)(int, bool) | Establece si el PivotItem específico en un campo de datos está oculto. |
| [HideItem](../../aspose.cells.pivot/pivotfield/hideitem#hideitem_1)(string, bool) | Establece si el PivotItem específico en un campo de datos está oculto. |
| [HideItemDetail](../../aspose.cells.pivot/pivotfield/hideitemdetail)(int, bool) | Establece si el PivotItem específico en un campo dinámico es un detalle oculto. |
| [InitPivotItems](../../aspose.cells.pivot/pivotfield/initpivotitems)() | Inicie los elementos pivote del campo pivote |
| [IsHiddenItem](../../aspose.cells.pivot/pivotfield/ishiddenitem)(int) | Indica si el PivotItem específico está oculto. |
| [IsHiddenItemDetail](../../aspose.cells.pivot/pivotfield/ishiddenitemdetail)(int) | Indica si el PivotItem específico es un detalle oculto. |
| [SetSubtotals](../../aspose.cells.pivot/pivotfield/setsubtotals)(PivotFieldSubtotalType, bool) | Establece si el campo especificado muestra esos subtotales. |

### Ejemplos

```csharp

[C#]

Workbook book = new Workbook();
Worksheet sheet = book.Worksheets[0];
Cells cells = sheet.Cells;
cells[0, 0].Value = "fruit";
cells[1, 0].Value = "grape";
cells[2, 0].Value = "blueberry";
cells[3, 0].Value = "kiwi";
cells[4, 0].Value = "cherry";
cells[5, 0].Value = "grape";
cells[6, 0].Value = "blueberry";
cells[7, 0].Value = "kiwi";
cells[8, 0].Value = "cherry";

cells[0, 1].Value = "year";
cells[1, 1].Value = 2020;
cells[2, 1].Value = 2020;
cells[3, 1].Value = 2020;
cells[4, 1].Value = 2020;
cells[5, 1].Value = 2021;
cells[6, 1].Value = 2021;
cells[7, 1].Value = 2021;
cells[8, 1].Value = 2021;

cells[0, 2].Value = "amount";
cells[1, 2].Value = 50;
cells[2, 2].Value = 60;
cells[3, 2].Value = 70;
cells[4, 2].Value = 80;
cells[5, 2].Value = 90;
cells[6, 2].Value = 100;
cells[7, 2].Value = 110;
cells[8, 2].Value = 120;

PivotTableCollection pivots = sheet.PivotTables;

int pivotIndex = pivots.Add("=Sheet1!A1:C9", "A12", "TestPivotTable");
PivotTable pivot = pivots[pivotIndex];
pivot.AddFieldToArea(PivotFieldType.Row, "fruit");
pivot.AddFieldToArea(PivotFieldType.Column, "year");
pivot.AddFieldToArea(PivotFieldType.Data, "amount");

pivot.PivotTableStyleType = PivotTableStyleType.PivotTableStyleMedium10;

//Cambiar los atributos de PivotField
PivotField rowField = pivot.RowFields[0];
rowField.DisplayName = "custom display name";

pivot.RefreshData();
pivot.CalculateData();

//haz tu negocio

book.Save("out.xlsx");

[Visual Basic]

Dim book As Workbook = New Workbook()
Dim sheet As Worksheet = book.Worksheets(0)
Dim cells As Cells = sheet.Cells

cells(0, 0).Value = "fruit"
cells(1, 0).Value = "grape"
cells(2, 0).Value = "blueberry"
cells(3, 0).Value = "kiwi"
cells(4, 0).Value = "cherry"
cells(5, 0).Value = "grape"
cells(6, 0).Value = "blueberry"
cells(7, 0).Value = "kiwi"
cells(8, 0).Value = "cherry"

cells(0, 1).Value = "year"
cells(1, 1).Value = 2020
cells(2, 1).Value = 2020
cells(3, 1).Value = 2020
cells(4, 1).Value = 2020
cells(5, 1).Value = 2021
cells(6, 1).Value = 2021
cells(7, 1).Value = 2021
cells(8, 1).Value = 2021

cells(0, 2).Value = "amount"
cells(1, 2).Value = 50
cells(2, 2).Value = 60
cells(3, 2).Value = 70
cells(4, 2).Value = 80
cells(5, 2).Value = 90
cells(6, 2).Value = 100
cells(7, 2).Value = 110
cells(8, 2).Value = 120

Dim pivots As PivotTableCollection = sheet.PivotTables
Dim pivotIndex As Int32 = pivots.Add("=Sheet1!A1:C9", "A12", "TestPivotTable")
Dim pivot As PivotTable = pivots(pivotIndex)
pivot.AddFieldToArea(PivotFieldType.Row, "fruit")
Pivot.AddFieldToArea(PivotFieldType.Column, "year")
Pivot.AddFieldToArea(PivotFieldType.Data, "amount")

pivot.PivotTableStyleType = PivotTableStyleType.PivotTableStyleMedium10

'Change PivotField's attributes
Dim rowField As PivotField = pivot.RowFields(0)
rowField.DisplayName = "custom display name"

pivot.RefreshData()
pivot.CalculateData()

book.Save("out_vb.xlsx")
```

### Ver también

* espacio de nombres [Aspose.Cells.Pivot](../../aspose.cells.pivot)
* asamblea [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
