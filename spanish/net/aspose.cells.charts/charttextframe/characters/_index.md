---
title: "ChartTextFrame.Characters"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método ChartTextFrame. Devuelve un objeto Characters que representa un rango de caracteres dentro del texto"
type: docs
url: /es/net/aspose.cells.charts/charttextframe/characters/
---
## ChartTextFrame.Characters method

Devuelve un objeto Characters que representa un rango de caracteres dentro del texto.

```csharp
public FontSetting Characters(int startIndex, int length)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| startIndex | Int32 | El índice del inicio del carácter. |
| longitud | Int32 | El número de caracteres. |

### Valor de retorno

Objeto Characters.

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartTextFrameMethodCharactersWithInt32Int32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar datos de ejemplo
            worksheet.Cells["A1"].PutValue("Item");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["B1"].PutValue("Quantity");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);

            // Crear gráfico
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B3", true);
            chart.NSeries.CategoryData = "A2:A3";

            // Acceder a las etiquetas de datos y establecer el tamaño de fuente para caracteres específicos
            chart.NSeries[0].Points[0].DataLabels.ShowValue = true;
            chart.NSeries[0].Points[0].DataLabels.Characters(0, 5).Font.Size = 14;
            
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ver también

* class [FontSetting](../../../aspose.cells/fontsetting/)
* class [ChartTextFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


