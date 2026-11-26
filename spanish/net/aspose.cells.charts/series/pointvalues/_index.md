---
title: "Series.PointValues"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Series. Obtiene los valores reales que se utilizan para trazar cada punto de esta serie en el gráfico"
type: docs
url: /es/net/aspose.cells.charts/series/pointvalues/
---
## Series.PointValues property

Obtiene los valores reales que se utilizan para trazar cada punto de esta serie en el gráfico.

```csharp
public ChartDataValue[] PointValues { get; }
```

### Observaciones

Esta propiedad ofrece una forma conveniente de obtener los valores reales correspondientes a los datos definidos por [`Values`](../values/), especialmente cuando la fuente de datos especificada es un enlace externo, una fórmula, ...etc.

### Ejemplos

```csharp
//Demostración para mostrar un caso que requiere esta propiedad:
[C#]

Workbook workbook = new Workbook("ExternalSourceChart.xlsx");
Worksheet worksheet = workbook.Worksheets[0];
Chart chart = worksheet.Charts[0];
chart.Calculate();
string Values = chart.NSeries[0].Values;
// Los valores podrían ser como "[External.xlsx]Sheet1!$A$1:$A$6" lo cual es complicado
// para que el usuario obtenga los valores reales (los valores pueden estar vinculados a otro libro de trabajo,
// o almacenados en caché en el libro de trabajo actual). Aquí puede usar la propiedad PointValues
// para obtener los valores que se muestran realmente en la interfaz de Excel
// en forma de una matriz.
ChartDataValue[] v1 = chart.NSeries[0].PointValues;

```

### Ver también

* class [ChartDataValue](../../chartdatavalue/)
* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


