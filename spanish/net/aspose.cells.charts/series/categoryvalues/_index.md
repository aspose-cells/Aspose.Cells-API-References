---
title: "Series.CategoryValues"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Series. Obtiene los valores de categoría reales que se utilizan para trazar cada punto de esta serie en el gráfico"
type: docs
url: /es/net/aspose.cells.charts/series/categoryvalues/
---
## Series.CategoryValues property

Obtiene los valores reales de categoría que se utilizan para trazar cada punto de esta serie en el gráfico.

```csharp
public ChartDataValue[][] CategoryValues { get; }
```

### Observaciones

Esta propiedad ofrece una forma conveniente de obtener los valores reales correspondientes a los datos definidos por [`XValues`](../xvalues/), especialmente cuando la fuente de datos especificada es un enlace externo, una fórmula, ...etc.

### Ejemplos

```csharp
//Demostración para mostrar un caso que requiere esta propiedad:
[C#]

//Ejemplo independiente
Workbook workbook = new Workbook("ExternalSourceChart.xlsx");
Worksheet worksheet = workbook.Worksheets[0];
Chart chart = worksheet.Charts[0];
chart.Calculate();
string XValues = chart.NSeries[0].XValues;
// XValues puede ser como "[External.xlsx]Sheet1!$B$2:$C$6" que es complicado
// para que el usuario obtenga los valores reales (los valores pueden estar vinculados a otro libro de trabajo,
// o almacenado en caché en el libro actual). Aquí puedes usar la propiedad CategoryValues
// para obtener los valores de categoría que se muestran realmente en la interfaz de Excel
// en forma de una matriz bidimensional.
ChartDataValue[][] v1 = chart.NSeries[0].CategoryValues;

```

### Ver también

* class [ChartDataValue](../../chartdatavalue/)
* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


