---
title: Area
second_title: Referencia de API de Aspose.Cells para .NET
description: Encapsula el objeto que representa un formato de área.
type: docs
weight: 1760
url: /es/net/aspose.cells.drawing/area/
---
## Area class

Encapsula el objeto que representa un formato de área.

```csharp
public class Area
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [BackgroundColor](../../aspose.cells.drawing/area/backgroundcolor) { get; set; } | Obtiene o establece el fondoColor del[`Area`](../area) . |
| [FillFormat](../../aspose.cells.drawing/area/fillformat) { get; } | Representa un objeto que contiene propiedades de formato de relleno para el gráfico o la forma especificados. |
| [ForegroundColor](../../aspose.cells.drawing/area/foregroundcolor) { get; set; } | Obtiene o establece el primer planoColor . |
| [Formatting](../../aspose.cells.drawing/area/formatting) { get; set; } | Representa el formato del área. |
| [InvertIfNegative](../../aspose.cells.drawing/area/invertifnegative) { get; set; } | Si la propiedad es verdadera y el valor del punto del gráfico es un número negativo, se intercambiarán el color frontal y el color de fondo. |
| [Transparency](../../aspose.cells.drawing/area/transparency) { get; set; } | Devuelve o establece el grado de transparencia del área como un valor de 0,0 (opaco) a 1,0 (transparente). |

### Ejemplos

```csharp

[C#]
// Instanciando un objeto Workbook
Workbook workbook = new Workbook();
// Agregar una nueva hoja de trabajo al objeto Workbook
int sheetIndex = workbook.Worksheets.Add();
//Obteniendo la referencia de la hoja de trabajo recién agregada pasando su índice de hoja
Worksheet worksheet = workbook.Worksheets[sheetIndex];
// Agregar un valor de muestra a la celda "A1"
worksheet.Cells["A1"].PutValue(50);
// Agregar un valor de muestra a la celda "A2"
worksheet.Cells["A2"].PutValue(100);
// Agregar un valor de muestra a la celda "A3"
worksheet.Cells["A3"].PutValue(150);
// Agregar un valor de muestra a la celda "B1"
worksheet.Cells["B1"].PutValue(60);
// Agregar un valor de muestra a la celda "B2"
worksheet.Cells["B2"].PutValue(32);
// Agregar un valor de muestra a la celda "B3"
worksheet.Cells["B3"].PutValue(50);
//Añadiendo un gráfico a la hoja de trabajo
int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
//Accediendo a la instancia del gráfico recién agregado
Chart chart = worksheet.Charts[chartIndex];
// Agregar NSeries (fuente de datos del gráfico) al gráfico que va desde la celda "A1" hasta la celda "B3"
chart.NSeries.Add("A1:B3", true);
//Establecer el color de primer plano del área de trazado
chart.PlotArea.Area.ForegroundColor = Color.Blue;
//Establecer el color de primer plano del área del gráfico
chart.ChartArea.Area.ForegroundColor = Color.Yellow;
//Configuración del color de primer plano de la primera área de NSeries
chart.NSeries[0].Area.ForegroundColor = Color.Red;
//Establecer el color de primer plano del área del primer punto NSeries
chart.NSeries[0].Points[0].Area.ForegroundColor = Color.Cyan;
//Guardando el archivo de Excel
workbook.Save("book1.xls");

[Visual Basic]

'Crear una instancia de un objeto Workbook
Dim workbook As Workbook = New Workbook()
'Agregar una nueva hoja de cálculo al objeto Workbook
Dim sheetIndex As Integer = workbook.Worksheets.Add()
'Obtener la referencia de la hoja de trabajo recién agregada pasando su índice de hoja
Dim worksheet As Worksheet = workbook.Worksheets(sheetIndex)
'Adding a sample value to "A1" cell
worksheet.Cells("A1").PutValue(50)
'Adding a sample value to "A2" cell
worksheet.Cells("A2").PutValue(100)
'Adding a sample value to "A3" cell
worksheet.Cells("A3").PutValue(150)
'Adding a sample value to "B1" cell
worksheet.Cells("B1").PutValue(60)
'Adding a sample value to "B2" cell
worksheet.Cells("B2").PutValue(32)
'Adding a sample value to "B3" cell
worksheet.Cells("B3").PutValue(50)
'Adición de un gráfico a la hoja de cálculo
Dim chartIndex As Integer = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5)
'Acceso a la instancia del gráfico recién agregado
Dim chart As Chart = worksheet.Charts(chartIndex)
'Adding NSeries (chart data source) to the chart ranging from "A1" cell to "B3"
chart.NSeries.Add("A1:B3", True)
'Configuración del color de primer plano del área de trazado
chart.PlotArea.Area.ForegroundColor = Color.Blue
'Establecer el color de primer plano del área del gráfico
chart.ChartArea.Area.ForegroundColor = Color.Yellow
'Configuración del color de primer plano de la primera área de NSeries
chart.NSeries(0).Area.ForegroundColor = Color.Red
'Configuración del color de primer plano del área del primer punto NSeries
chart.NSeries(0).Points(0).Area.ForegroundColor = Color.Cyan
'Guardar el archivo de Excel
workbook.Save("book1.xls")
```

### Ver también

* espacio de nombres [Aspose.Cells.Drawing](../../aspose.cells.drawing)
* asamblea [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
