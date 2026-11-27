---
title: "Enum PivotTableSourceType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Pivot.PivotTableSourceType enum. Representerar datakälltyp för pivottabellen"
type: docs
url: /sv/net/aspose.cells.pivot/pivottablesourcetype/
---
## PivotTableSourceType enumeration

Representerar datakälltyp för pivottabellen.

```csharp
public enum PivotTableSourceType : byte
```

### Värden

| Namn | Värde | Beskrivning |
| --- | --- | --- |
| Sheet | `1` | Anger att källdata är ett område. |
| External | `2` | Anger att extern källdata används. |
| Consolidation | `4` | Anger att flera konsolideringsområden används som källdata. |
| Scenario | `8` | Källdata fylls i från en tillfällig intern struktur. |
| Unknown | `9` | Okänd datakälla. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotClassPivotTableSourceTypeDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok för demonstration
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Lägg till exempeldata i kalkylbladet
                worksheet.Cells["A1"].PutValue("Category");
                worksheet.Cells["B1"].PutValue("Value");
                worksheet.Cells["A2"].PutValue("A");
                worksheet.Cells["B2"].PutValue(10);
                worksheet.Cells["A3"].PutValue("B");
                worksheet.Cells["B3"].PutValue(20);
                worksheet.Cells["A4"].PutValue("C");
                worksheet.Cells["B4"].PutValue(30);

                // Skapa en pivottabellsamling
                PivotTableCollection pivotTables = worksheet.PivotTables;

                // Lägg till en pivottabell med Sheet som källtyp
                int index = pivotTables.Add("=A1:B4", "D3", "SheetPivotTable");
                PivotTable pivotTable = pivotTables[index];

                // Visa källtypen
                Console.WriteLine("Pivot Table Source Type: " + pivotTable.SourceType);

                // Demonstrera olika källtyper
                Console.WriteLine("Available PivotTableSourceType values:");
                Console.WriteLine("Sheet: " + PivotTableSourceType.Sheet);
                Console.WriteLine("External: " + PivotTableSourceType.External);
                Console.WriteLine("Consolidation: " + PivotTableSourceType.Consolidation);
                Console.WriteLine("Scenario: " + PivotTableSourceType.Scenario);
                Console.WriteLine("Unknown: " + PivotTableSourceType.Unknown);

                // Spara arbetsboken
                workbook.Save("PivotTableSourceTypeDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with PivotTableSourceType: {ex.Message}");
            }
        }
    }
}
```

### Se även

* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)


