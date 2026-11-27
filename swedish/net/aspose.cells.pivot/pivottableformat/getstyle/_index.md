---
title: "PivotTableFormat.GetStyle"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PivotTableFormat‑metod. Hämtar den formaterade stilen"
type: docs
url: /sv/net/aspose.cells.pivot/pivottableformat/getstyle/
---
## PivotTableFormat.GetStyle method

Hämtar den formaterade stilen.

```csharp
public Style GetStyle()
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotTableFormatMethodGetStyleDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata för pivottabell
            worksheet.Cells["A1"].Value = "Fruit";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["A3"].Value = "Orange";
            worksheet.Cells["A4"].Value = "Banana";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["B2"].Value = 1000;
            worksheet.Cells["B3"].Value = 2000;
            worksheet.Cells["B4"].Value = 3000;

            // Skapa pivottabell
            PivotTableCollection pivotTables = worksheet.PivotTables;
            int index = pivotTables.Add("A1:B4", "C3", "PivotTable1");
            PivotTable pivotTable = pivotTables[index];
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // Hämta pivot‑tabellformat
            PivotTableFormatCollection formats = pivotTable.PivotFormats;
            PivotTableFormat format = formats[0];

            try
            {
                // Anropa GetStyle‑metoden
                Style style = format.GetStyle();

                // Egenskaper för visningsstil
                Console.WriteLine("Style properties:");
                Console.WriteLine($"Font Name: {style.Font.Name}");
                Console.WriteLine($"Font Size: {style.Font.Size}");
                Console.WriteLine($"Background Color: {style.BackgroundColor}");

                // Modifiera stilen
                style.Font.Name = "Arial";
                style.Font.Size = 12;
                style.BackgroundColor = System.Drawing.Color.LightBlue;

                // Tillämpa den modifierade stilen tillbaka på formatet
                format.SetStyle(style);

                Console.WriteLine("GetStyle method executed successfully");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetStyle method: {ex.Message}");
            }

            // Spara resultatet
            workbook.Save("PivotTableFormatMethodGetStyleDemo.xlsx");
        }
    }
}
```

### Se även

* class [Style](../../../aspose.cells/style/)
* class [PivotTableFormat](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


