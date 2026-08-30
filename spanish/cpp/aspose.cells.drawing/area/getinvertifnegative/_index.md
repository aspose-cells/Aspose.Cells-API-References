---
title: Aspose::Cells::Drawing::Area::GetInvertIfNegative method
linktitle: GetInvertIfNegative
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Drawing::Area::GetInvertIfNegative method. If the property is true and the value of chart point is a negative number, the foreground color and background color will be exchanged in C++.'
type: docs
weight: 1200
url: /es/cpp/aspose.cells.drawing/area/getinvertifnegative/
---
## Area::GetInvertIfNegative method


If the property is true and the value of chart point is a negative number, the foreground color and background color will be exchanged.

```cpp
bool Aspose::Cells::Drawing::Area::GetInvertIfNegative()
```


## Examples


```cpp
Aspose::Cells::Startup();
//Instanciando un objeto Workbook
Workbook workbook;
//Agregar una nueva hoja de cálculo al objeto Workbook
int sheetIndex = workbook.GetWorksheets().Add();
//Obteniendo la referencia de la hoja recién añadida pasando su índice de hoja
Worksheet worksheet = workbook.GetWorksheets().Get(sheetIndex);
//Agregar un valor de muestra a la celda "A1"
worksheet.GetCells().Get(u"A1").PutValue(50);
//Agregar un valor de muestra a la celda "A2"
worksheet.GetCells().Get(u"A2").PutValue(-100);
//Agregar un valor de muestra a la celda "A3"
worksheet.GetCells().Get(u"A3").PutValue(150);
//Agregar un gráfico a la hoja de cálculo
int chartIndex = worksheet.GetCharts().Add(ChartType::Column, 5, 0, 15, 5);
//Acceder a la instancia del gráfico recién añadido
Chart chart = worksheet.GetCharts().Get(chartIndex);
//Agregar NSeries (fuente de datos del gráfico) al gráfico que abarca desde la celda \"A1\" hasta \"A3\"
chart.GetNSeries().Add(u"A1:A3", true);
bool isNegative = chart.GetNSeries().Get(0).GetArea().GetInvertIfNegative();
Aspose::Cells::Cleanup();
```

## See Also

* Class [Area](../)
* Namespace [Aspose::Cells::Drawing](../../)
* Library [Aspose.Cells for C++](../../../)
