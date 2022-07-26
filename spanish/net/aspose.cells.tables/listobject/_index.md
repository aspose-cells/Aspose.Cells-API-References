---
title: ListObject
second_title: Referencia de API de Aspose.Cells para .NET
description: Representa un objeto de lista en una hoja de cálculo. El objeto ListObject es miembro de la colección ListObjects. La colección ListObjects contiene todos los objetos de lista en una hoja de cálculo.
type: docs
weight: 5820
url: /es/net/aspose.cells.tables/listobject/
---
## ListObject class

Representa un objeto de lista en una hoja de cálculo. El objeto ListObject es miembro de la colección ListObjects. La colección ListObjects contiene todos los objetos de lista en una hoja de cálculo.

```csharp
public class ListObject
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [AlternativeDescription](../../aspose.cells.tables/listobject/alternativedescription) { get; set; } | Obtiene y establece la descripción alternativa. |
| [AlternativeText](../../aspose.cells.tables/listobject/alternativetext) { get; set; } | Obtiene y establece el texto alternativo. |
| [AutoFilter](../../aspose.cells.tables/listobject/autofilter) { get; } | Obtiene filtro automático. |
| [Comment](../../aspose.cells.tables/listobject/comment) { get; set; } | Obtiene y establece el comentario de la tabla. |
| [DataRange](../../aspose.cells.tables/listobject/datarange) { get; } | Obtiene el rango de datos del ListObject. |
| [DataSourceType](../../aspose.cells.tables/listobject/datasourcetype) { get; } | Obtiene el tipo de fuente de datos de la tabla. |
| [DisplayName](../../aspose.cells.tables/listobject/displayname) { get; set; } | Obtiene y establece el nombre para mostrar. |
| [EndColumn](../../aspose.cells.tables/listobject/endcolumn) { get; } | Obtiene la última columna del rango. |
| [EndRow](../../aspose.cells.tables/listobject/endrow) { get; } | Obtiene la última fila del rango. |
| [ListColumns](../../aspose.cells.tables/listobject/listcolumns) { get; } | Obtiene ListColumns de ListObject. |
| [QueryTable](../../aspose.cells.tables/listobject/querytable) { get; } | Obtiene el QueryTable vinculado. |
| [ShowHeaderRow](../../aspose.cells.tables/listobject/showheaderrow) { get; set; } | Obtiene y establece si este ListObject muestra la fila de encabezado. |
| [ShowTableStyleColumnStripes](../../aspose.cells.tables/listobject/showtablestylecolumnstripes) { get; set; } | Indica si se aplica el formato de franja de columna. |
| [ShowTableStyleFirstColumn](../../aspose.cells.tables/listobject/showtablestylefirstcolumn) { get; set; } | Indica si la primera columna de la tabla debe tener el estilo aplicado. |
| [ShowTableStyleLastColumn](../../aspose.cells.tables/listobject/showtablestylelastcolumn) { get; set; } | Indica si la última columna de la tabla debe tener el estilo aplicado. |
| [ShowTableStyleRowStripes](../../aspose.cells.tables/listobject/showtablestylerowstripes) { get; set; } | Indica si se aplica el formato de franja de fila. |
| [ShowTotals](../../aspose.cells.tables/listobject/showtotals) { get; set; } | Obtiene y establece si este ListObject muestra la fila total. |
| [StartColumn](../../aspose.cells.tables/listobject/startcolumn) { get; } | Obtiene la columna inicial del rango. |
| [StartRow](../../aspose.cells.tables/listobject/startrow) { get; } | Obtiene la fila inicial del rango. |
| [TableStyleName](../../aspose.cells.tables/listobject/tablestylename) { get; set; } | Obtiene y establece el nombre de estilo de la tabla. |
| [TableStyleType](../../aspose.cells.tables/listobject/tablestyletype) { get; set; } | Obtiene y el estilo de tabla integrado. |
| [XmlMap](../../aspose.cells.tables/listobject/xmlmap) { get; } | Obtiene un[`XmlMap`](./xmlmap)usado para esta lista. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| [ApplyStyleToRange](../../aspose.cells.tables/listobject/applystyletorange)() | Aplicar el estilo de tabla al rango. |
| [ConvertToRange](../../aspose.cells.tables/listobject/converttorange#converttorange)() | Convierte la tabla a rango. |
| [ConvertToRange](../../aspose.cells.tables/listobject/converttorange#converttorange_1)(TableToRangeOptions) | Convierte la tabla a rango. |
| [Filter](../../aspose.cells.tables/listobject/filter)() | Filtra la tabla. |
| [PutCellValue](../../aspose.cells.tables/listobject/putcellvalue)(int, int, object) | Poner el valor a la celda. |
| [Resize](../../aspose.cells.tables/listobject/resize)(int, int, int, int, bool) | Cambiar el tamaño del rango del objeto de la lista. |
| [UpdateColumnName](../../aspose.cells.tables/listobject/updatecolumnname)() | Actualiza el nombre de todas las columnas de la lista de la hoja de cálculo. |

### Ejemplos

```csharp

[C#]


Workbook workbook = new Workbook();
Cells cells = workbook.Worksheets[0].Cells;
for (int i = 0; i  <5; i++)
{
cells[0,i].PutValue(CellsHelper.ColumnIndexToName(i));
 }
for (int row = 1; row  <10; row++)
{
 for (int column = 0; column  <5; column++)
{
cells[row, column].PutValue(row * column);
 }
 }
ListObjectCollection tables = workbook.Worksheets[0].ListObjects;
int index = tables.Add(0, 0, 9, 4, true);
ListObject table = tables[0];
table.ShowTotals = true;
table.ListColumns[4].TotalsCalculation = Aspose.Cells.Tables.TotalsCalculation.Sum;
workbook.Save(@"Book1.xlsx");


[Visual Basic]

Dim workbook As Workbook = New Workbook()
Dim cells As Cells = workbook.Worksheets(0).Cells
For i As Int32 = 0 To 4
 cells(0, i).PutValue(CellsHelper.ColumnIndexToName(i))
Next
For row As Int32 = 1 To 9
 For column As Int32 = 0 To 4
  cells(row, column).PutValue(row * column)
Next
Next
Dim tables As ListObjectCollection = workbook.Worksheets(0).ListObjects
Dim index As Int32 = tables.Add(0, 0, 9, 4, True)
Dim table As ListObject = tables(0)
table.ShowTotals = True
table.ListColumns(4).TotalsCalculation = Aspose.Cells.Tables.TotalsCalculation.Sum
workbook.Save("Book1.xlsx")
```

### Ver también

* espacio de nombres [Aspose.Cells.Tables](../../aspose.cells.tables)
* asamblea [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
