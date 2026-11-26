---
title: "PivotTableFormat.SetStyle"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método PivotTableFormat. Establece el estilo del área de tabla dinámica"
type: docs
url: /es/net/aspose.cells.pivot/pivottableformat/setstyle/
---
## PivotTableFormat.SetStyle method

Establece el estilo del área de la tabla dinámica.

```csharp
public void SetStyle(Style style)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| estilo | Estilo |  |

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class PivotTableFormatMethodSetStyleWithStyleDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            worksheet.Cells["A1"].Value = "Fruit";
            worksheet.Cells["B1"].Value = "Year";
            worksheet.Cells["C1"].Value = "Amount";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["B2"].Value = 2020;
            worksheet.Cells["C2"].Value = 50;
            worksheet.Cells["A3"].Value = "Banana";
            worksheet.Cells["B3"].Value = 2020;
            worksheet.Cells["C3"].Value = 60;

            int pivotIndex = worksheet.PivotTables.Add("=Sheet1!A1:C3", "E5", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 2);

            PivotTableFormatCollection formatCollection = pivotTable.PivotFormats;
            int formatIndex = formatCollection.Add();
            PivotTableFormat pivotFormat = formatCollection[formatIndex];

            Style style = workbook.CreateStyle();
            style.BackgroundColor = Color.LightBlue;
            style.Font.Color = Color.DarkBlue;
            style.Font.IsBold = true;

            pivotFormat.SetStyle(style);

            workbook.Save("PivotTableSetStyleDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Style](../../../aspose.cells/style/)
* class [PivotTableFormat](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


