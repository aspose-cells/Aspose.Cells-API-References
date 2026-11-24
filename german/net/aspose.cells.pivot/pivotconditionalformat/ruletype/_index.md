---
title: "PivotConditionalFormat.RuleType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PivotConditionalFormat-Eigenschaft. Regeltyp für das Pivot-Tabellen-Bedingungsformat abrufen und festlegen"
type: docs
url: /de/net/aspose.cells.pivot/pivotconditionalformat/ruletype/
---
## PivotConditionalFormat.RuleType property

Lese und setze den Regeltyp für das bedingte Format der Pivot‑Tabelle.

```csharp
public PivotConditionFormatRuleType RuleType { get; set; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotConditionalFormatPropertyRuleTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Erstelle minimale Daten für die Pivot-Tabelle
                worksheet.Cells["A1"].Value = "Category";
                worksheet.Cells["A2"].Value = "Value";

                // Pivot-Tabelle erstellen
                int pivotIndex = worksheet.PivotTables.Add("A1:A2", "C3", "DemoPivotTable");
                PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

                // Bedingtes Format hinzufügen
                int formatIndex = pivotTable.ConditionalFormats.Add();
                PivotConditionalFormat format = pivotTable.ConditionalFormats[formatIndex];

                // Demonstriere die RuleType-Eigenschaft
                Console.WriteLine("Initial RuleType: " + format.RuleType);
                
                // Setze neuen Regeltyp
                format.RuleType = PivotConditionFormatRuleType.Row;
                Console.WriteLine("Updated RuleType: " + format.RuleType);

                workbook.Save("RuleTypeDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Siehe auch

* enum [PivotConditionFormatRuleType](../../pivotconditionformatruletype/)
* class [PivotConditionalFormat](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


