---
title: "PivotConditionalFormat.RuleType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PivotConditionalFormat-egenskap. Hämta och ange regeltyp för pivottabellens villkorsformat"
type: docs
url: /sv/net/aspose.cells.pivot/pivotconditionalformat/ruletype/
---
## PivotConditionalFormat.RuleType property

Hämta och ange regeltyp för pivottabellens villkorliga format.

```csharp
public PivotConditionFormatRuleType RuleType { get; set; }
```

### Exempel

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
                // Skapa minimal data för pivottabell
                worksheet.Cells["A1"].Value = "Category";
                worksheet.Cells["A2"].Value = "Value";

                // Skapa pivottabell
                int pivotIndex = worksheet.PivotTables.Add("A1:A2", "C3", "DemoPivotTable");
                PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

                // Lägg till villkorligt format
                int formatIndex = pivotTable.ConditionalFormats.Add();
                PivotConditionalFormat format = pivotTable.ConditionalFormats[formatIndex];

                // Demonstrera RuleType-egenskapen
                Console.WriteLine("Initial RuleType: " + format.RuleType);
                
                // Ange ny regeltyp
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

### Se även

* enum [PivotConditionFormatRuleType](../../pivotconditionformatruletype/)
* class [PivotConditionalFormat](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


