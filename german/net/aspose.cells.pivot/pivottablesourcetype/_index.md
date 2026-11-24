---
title: "Enum PivotTableSourceType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Pivot.PivotTableSourceType enum. Stellt den Datentyp der Datenquelle der Pivot‑Tabelle dar."
type: docs
url: /de/net/aspose.cells.pivot/pivottablesourcetype/
---
## PivotTableSourceType enumeration

Stellt den Datentyp der Datenquelle einer PivotTable dar.

```csharp
public enum PivotTableSourceType : byte
```

### Werte

| Name | Wert | Beschreibung |
| --- | --- | --- |
| Sheet | `1` | Gibt an, dass die Quelldaten ein Bereich sind. |
| External | `2` | Gibt an, dass externe Quelldaten verwendet werden. |
| Consolidation | `4` | Gibt an, dass mehrere Konsolidierungsbereiche als Quelldaten verwendet werden. |
| Scenario | `8` | Die Quelldaten werden aus einer temporären internen Struktur befüllt. |
| Unknown | `9` | Unbekannte Datenquelle. |

### Beispiele

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
            // Erstellt ein neues Arbeitsbuch für die Demonstration
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Beispieldaten zum Arbeitsblatt hinzufügen
                worksheet.Cells["A1"].PutValue("Category");
                worksheet.Cells["B1"].PutValue("Value");
                worksheet.Cells["A2"].PutValue("A");
                worksheet.Cells["B2"].PutValue(10);
                worksheet.Cells["A3"].PutValue("B");
                worksheet.Cells["B3"].PutValue(20);
                worksheet.Cells["A4"].PutValue("C");
                worksheet.Cells["B4"].PutValue(30);

                // Erstelle eine Pivot‑Tabellensammlung
                PivotTableCollection pivotTables = worksheet.PivotTables;

                // Füge eine Pivot‑Tabelle hinzu, die Sheet als Quelltyp verwendet
                int index = pivotTables.Add("=A1:B4", "D3", "SheetPivotTable");
                PivotTable pivotTable = pivotTables[index];

                // Zeige den Quelltyp an
                Console.WriteLine("Pivot Table Source Type: " + pivotTable.SourceType);

                // Demonstriere verschiedene Quelltypen
                Console.WriteLine("Available PivotTableSourceType values:");
                Console.WriteLine("Sheet: " + PivotTableSourceType.Sheet);
                Console.WriteLine("External: " + PivotTableSourceType.External);
                Console.WriteLine("Consolidation: " + PivotTableSourceType.Consolidation);
                Console.WriteLine("Scenario: " + PivotTableSourceType.Scenario);
                Console.WriteLine("Unknown: " + PivotTableSourceType.Unknown);

                // Speichere die Arbeitsmappe
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

### Siehe auch

* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)


