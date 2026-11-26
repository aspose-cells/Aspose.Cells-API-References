---
title: "PivotConditionalFormat.GetCellAreas"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод PivotConditionalFormat. Получает все области ячеек, к которым применяется это условное форматирование"
type: docs
url: /ru/net/aspose.cells.pivot/pivotconditionalformat/getcellareas/
---
## PivotConditionalFormat.GetCellAreas method

Получает все ячейковые области, к которым применяется это условное форматирование.

```csharp
public CellArea[] GetCellAreas()
```

### Примеры

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
                // Создайте сводную таблицу, необходимую для PivotConditionalFormat
                worksheet.Cells["A1"].Value = "Header";
                worksheet.Cells["A2"].Value = "Data";
                int pivotIndex = worksheet.PivotTables.Add("A1:A2", "B3", "PivotTable1");
                PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
                
                // Создайте условное форматирование через коллекцию сводной таблицы
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

### См. также

* struct [CellArea](../../../aspose.cells/cellarea/)
* class [PivotConditionalFormat](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


