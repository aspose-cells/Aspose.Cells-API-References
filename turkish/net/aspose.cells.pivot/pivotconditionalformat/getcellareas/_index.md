---
title: "PivotConditionalFormat.GetCellAreas"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PivotConditionalFormat yöntemi. Bu koşullu biçimin uygulandığı tüm hücre alanlarını alır"
type: docs
url: /tr/net/aspose.cells.pivot/pivotconditionalformat/getcellareas/
---
## PivotConditionalFormat.GetCellAreas method

Bu koşullu biçimin uygulandığı tüm hücre alanlarını alır.

```csharp
public CellArea[] GetCellAreas()
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotConditionalFormatMethodGetCellAreasDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // PivotConditionalFormat için gerekli bir döndürme tablosu oluşturun
                worksheet.Cells["A1"].Value = "Header";
                worksheet.Cells["A2"].Value = "Data";
                int pivotIndex = worksheet.PivotTables.Add("A1:A2", "B3", "PivotTable1");
                PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
                
                // Döndürme tablosunun koleksiyonu aracılığıyla koşullu biçim oluşturun
                int formatIndex = pivotTable.ConditionalFormats.Add();
                PivotConditionalFormat conditionalFormat = pivotTable.ConditionalFormats[formatIndex];
                
                CellArea area = new CellArea();
                area.StartRow = 0;
                area.StartColumn = 0;
                area.EndRow = 2;
                area.EndColumn = 2;
                conditionalFormat.AddCellArea(area);

                CellArea[] resultAreas = conditionalFormat.GetCellAreas();
                
                Console.WriteLine($"Retrieved {resultAreas.Length} cell area(s):");
                foreach (CellArea ca in resultAreas)
                {
                    Console.WriteLine($"Rows {ca.StartRow}-{ca.EndRow}, Cols {ca.StartColumn}-{ca.EndColumn}");
                }

                workbook.Save("GetCellAreasDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling GetCellAreas: {ex.Message}");
            }
        }
    }
}
```

### Ayrıca Bakınız

* struct [CellArea](../../../aspose.cells/cellarea/)
* class [PivotConditionalFormat](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


