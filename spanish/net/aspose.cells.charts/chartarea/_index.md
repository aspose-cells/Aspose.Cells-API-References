---
title: ChartArea
second_title: Referencia de API de Aspose.Cells para .NET
description: Encapsula el objeto que representa el área del gráfico en la hoja de trabajo.
type: docs
weight: 440
url: /es/net/aspose.cells.charts/chartarea/
---
## ChartArea class

Encapsula el objeto que representa el área del gráfico en la hoja de trabajo.

```csharp
public class ChartArea : ChartFrame
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| virtual [Area](../../aspose.cells.charts/chartframe/area) { get; } | Obtiene el[`área`](../chartframe/area) . |
| virtual [AutoScaleFont](../../aspose.cells.charts/chartframe/autoscalefont) { get; set; } | Verdadero si el texto del objeto cambia el tamaño de fuente cuando cambia el tamaño del objeto. El valor por defecto es verdadero. |
| [BackgroundMode](../../aspose.cells.charts/chartframe/backgroundmode) { get; set; } | Obtiene y establece el modo de visualización del fondo |
| virtual [Border](../../aspose.cells.charts/chartframe/border) { get; } | Obtiene el[`borde`](../../aspose.cells.drawing/line) . |
| [DefaultHeight](../../aspose.cells.charts/chartframe/defaultheight) { get; } | Representa la altura de la posición predeterminada |
| [DefaultWidth](../../aspose.cells.charts/chartframe/defaultwidth) { get; } | Representa el ancho de la posición predeterminada |
| [DefaultX](../../aspose.cells.charts/chartframe/defaultx) { get; } | Representa x de la posición predeterminada |
| [DefaultY](../../aspose.cells.charts/chartframe/defaulty) { get; } | Representa y de la posición predeterminada |
| override [Font](../../aspose.cells.charts/chartarea/font) { get; } | Obtiene un[`Font`](./font) objeto del objeto chartarea especificado. |
| override [Height](../../aspose.cells.charts/chartarea/height) { get; set; } | Obtiene o establece el desplazamiento vertical desde su fila de la esquina inferior derecha. |
| virtual [IsAutomaticSize](../../aspose.cells.charts/chartframe/isautomaticsize) { get; set; } | Indica si el marco del gráfico tiene un tamaño automático. |
| [IsDefaultPosBeSet](../../aspose.cells.charts/chartframe/isdefaultposbeset) { get; } | Indica si la posición predeterminada (DefaultX, DefaultY, DefaultWidth y DefaultHeight) está configurada. |
| [IsInnerMode](../../aspose.cells.charts/chartframe/isinnermode) { get; set; } | Indica si el tamaño del área de trazado incluye las marcas y las etiquetas de los ejes. Falso especifica que el tamaño determinará el tamaño del área de trazado, las marcas y las etiquetas de los ejes. |
| [Shadow](../../aspose.cells.charts/chartframe/shadow) { get; set; } | Verdadero si el marco tiene sombra. |
| [ShapeProperties](../../aspose.cells.charts/chartframe/shapeproperties) { get; } | Obtiene el[`ShapeProperties`](../chartframe/shapeproperties) objeto. |
| override [Width](../../aspose.cells.charts/chartarea/width) { get; set; } | Obtiene o establece el desplazamiento horizontal desde su columna de la esquina inferior derecha. |
| override [X](../../aspose.cells.charts/chartarea/x) { get; set; } | Obtiene u obtiene el desplazamiento horizontal de su columna de la esquina superior izquierda. |
| override [Y](../../aspose.cells.charts/chartarea/y) { get; set; } | Obtiene u obtiene el desplazamiento vertical de su fila de la esquina superior izquierda. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| virtual [SetPositionAuto](../../aspose.cells.charts/chartframe/setpositionauto)() | Establece la posición del marco en automático |

### Ejemplos

```csharp

[C#]

// Instanciando un objeto Workbook
Workbook workbook = new Workbook();

//Obteniendo la referencia de la primera hoja de cálculo
Worksheet worksheet = workbook.Worksheets[0];

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

//Obtener el área del gráfico
ChartArea chartArea = chart.ChartArea;

//Establecer el color de primer plano del área del gráfico
chartArea.Area.ForegroundColor = Color.Yellow;

//Configuración de la sombra del área del gráfico
chartArea.Shadow = true;

//Guardando el archivo de Excel
workbook.Save("book1.xls");

[VB.NET]

'Crear una instancia de un objeto Workbook
Dim workbook As Workbook = New Workbook()

'Obtención de la referencia de la primera hoja de cálculo
Dim worksheet As Worksheet = workbook.Worksheets(0)

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

'Obtención del área del gráfico
Dim chartArea As ChartArea = chart.ChartArea

'Establecer el color de primer plano del área del gráfico
chartArea.Area.ForegroundColor = Color.Yellow

'Configuración de la sombra del área del gráfico
chartArea.Shadow = True

'Guardar el archivo de Excel
workbook.Save("book1.xls")
```

### Ver también

* class [ChartFrame](../chartframe)
* espacio de nombres [Aspose.Cells.Charts](../../aspose.cells.charts)
* asamblea [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
