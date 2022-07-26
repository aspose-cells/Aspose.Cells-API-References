---
title: DataBar
second_title: Referencia de API de Aspose.Cells para .NET
description: Describe la regla de formato condicional de DataBar. Esta regla de formato condicional muestra una barra de datos graduada en el rango de celdas.
type: docs
weight: 1240
url: /es/net/aspose.cells/databar/
---
## DataBar class

Describe la regla de formato condicional de DataBar. Esta regla de formato condicional muestra una barra de datos graduada en el rango de celdas.

```csharp
public class DataBar
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [AxisColor](../../aspose.cells/databar/axiscolor) { get; set; } | Obtiene el color del eje para celdas con formato condicional como barras de datos. |
| [AxisPosition](../../aspose.cells/databar/axisposition) { get; set; } | Obtiene o establece la posición del eje de las barras de datos especificadas por una regla de formato condicional. |
| [BarBorder](../../aspose.cells/databar/barborder) { get; } | Obtiene un objeto que especifica el borde de una barra de datos. |
| [BarFillType](../../aspose.cells/databar/barfilltype) { get; set; } | Obtiene o establece cómo se llena de color una barra de datos. |
| [Color](../../aspose.cells/databar/color) { get; set; } | Obtener o establecer el Color de esta barra de datos. |
| [Direction](../../aspose.cells/databar/direction) { get; set; } | Obtiene o establece la dirección en la que se muestra la barra de datos. |
| [MaxCfvo](../../aspose.cells/databar/maxcfvo) { get; } | Obtener o establecer el objeto de valor máximo de este DataBar. No se puede establecer un valor nulo o CFValueObject con el tipo FormatConditionValueType.Min. |
| [MaxLength](../../aspose.cells/databar/maxlength) { get; set; } | Representa la longitud máxima de la barra de datos. |
| [MinCfvo](../../aspose.cells/databar/mincfvo) { get; } | Obtener o establecer el objeto de valor mínimo de este DataBar. No se puede establecer un valor nulo o CFValueObject con el tipo FormatConditionValueType.Max. |
| [MinLength](../../aspose.cells/databar/minlength) { get; set; } | Representa la longitud mínima de la barra de datos. |
| [NegativeBarFormat](../../aspose.cells/databar/negativebarformat) { get; } | Obtiene el objeto NegativeBarFormat asociado con una regla de formato condicional de la barra de datos. |
| [ShowValue](../../aspose.cells/databar/showvalue) { get; set; } | Obtener o establecer el indicador que indica si mostrar los valores de las celdas en las que se aplica esta barra de datos. El valor predeterminado es verdadero. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| [ToImage](../../aspose.cells/databar/toimage)(Cell, ImageOrPrintOptions) | Representar barra de datos en matriz de bytes de celda a imagen. |

### Ejemplos

```csharp

[C#]

// Instanciando un objeto Workbook
Workbook workbook = new Workbook();

Worksheet sheet = workbook.Worksheets[0];

//Agrega un formato condicional vacío
int index = sheet.ConditionalFormattings.Add();

FormatConditionCollection fcs = sheet.ConditionalFormattings[index];

//Establece el rango de formato condicional.
CellArea ca = new CellArea();

ca.StartRow = 0;

ca.EndRow = 2;

ca.StartColumn = 0;

ca.EndColumn = 0;

fcs.AddArea(ca);

//Agrega condición.
int idx = fcs.AddCondition(FormatConditionType.DataBar);

fcs.AddArea(ca);

FormatCondition cond = fcs[idx];

//Obtener la barra de datos
DataBar dataBar = cond.DataBar;

dataBar.Color = Color.Orange;

//Establecer propiedades de la barra de datos
dataBar.MinCfvo.Type = FormatConditionValueType.Percentile;

dataBar.MinCfvo.Value = 30;

dataBar.ShowValue = false;

dataBar.BarBorder.Type = DataBarBorderType.Solid;

dataBar.BarBorder.Color = Color.Plum;

 dataBar.BarFillType = DataBarFillType.Solid;
  
 dataBar.AxisColor = Color.Red;
 
 dataBar.AxisPosition = DataBarAxisPosition.Midpoint;
 
 dataBar.NegativeBarFormat.ColorType = DataBarNegativeColorType.Color;
 
 dataBar.NegativeBarFormat.Color = Color.White;
 
 dataBar.NegativeBarFormat.BorderColorType = DataBarNegativeColorType.Color;
 
 dataBar.NegativeBarFormat.BorderColor = Color.Yellow;
 
//Poner valores de celda
Aspose.Cells.Cell cell1 = sheet.Cells["A1"];

cell1.PutValue(10);

Aspose.Cells.Cell cell2 = sheet.Cells["A2"];

cell2.PutValue(120);

Aspose.Cells.Cell cell3 = sheet.Cells["A3"];

cell3.PutValue(260);

//Guardando el archivo de Excel
workbook.Save("book1.xlsx");

[VB.NET]

'Crear una instancia de un objeto Workbook
Dim workbook As Workbook = New Workbook()

Dim sheet As Worksheet = workbook.Worksheets(0)

'Agrega un formato condicional vacío
Dim index As Integer = sheet.ConditionalFormattings.Add()

Dim fcs As FormatConditionCollection = sheet.ConditionalFormattings(index)

'Establece el rango de formato condicional.
Dim ca As New CellArea()

ca.StartRow = 0

ca.EndRow = 2

ca.StartColumn = 0

ca.EndColumn = 0

fcs.AddArea(ca)

'Agrega condición.
Dim idx As Integer = fcs.AddCondition(FormatConditionType.DataBar)

fcs.AddArea(ca)

Dim cond As FormatCondition = fcs(idx)

'Obtener barra de datos
Dim dataBar As DataBar = cond.DataBar

dataBar.Color = Color.Orange

'Establecer las propiedades de la barra de datos
dataBar.MinCfvo.Type = FormatConditionValueType.Percentile

dataBar.MinCfvo.Value = 30

dataBar.ShowValue = False

dataBar.BarBorder.Type = DataBarBorderType.Solid

dataBar.BarBorder.Color = Color.Plum

 dataBar.BarFillType = DataBarFillType.Solid
  
 dataBar.AxisColor = Color.Red
 
 dataBar.AxisPosition = DataBarAxisPosition.Midpoint
 
 dataBar.NegativeBarFormat.ColorType = DataBarNegativeColorType.Color
 
 dataBar.NegativeBarFormat.Color = Color.White
 
 dataBar.NegativeBarFormat.BorderColorType = DataBarNegativeColorType.Color
 
 dataBar.NegativeBarFormat.BorderColor = Color.Yellow

'Poner valores de celda
Dim cell1 As Aspose.Cells.Cell = sheet.Cells("A1")

cell1.PutValue(10)

Dim cell2 As Aspose.Cells.Cell = sheet.Cells("A2")

cell2.PutValue(120)

Dim cell3 As Aspose.Cells.Cell = sheet.Cells("A3")

cell3.PutValue(260)

'Guardar el archivo de Excel
workbook.Save("book1.xlsx")

```

### Ver también

* espacio de nombres [Aspose.Cells](../../aspose.cells)
* asamblea [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
