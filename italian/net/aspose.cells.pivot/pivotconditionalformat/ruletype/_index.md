---
title: "PivotConditionalFormat.RuleType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà PivotConditionalFormat. Ottieni e imposta il tipo di regola per il formato condizionale della tabella pivot"
type: docs
url: /it/net/aspose.cells.pivot/pivotconditionalformat/ruletype/
---
## PivotConditionalFormat.RuleType property

Ottieni e imposta il tipo di regola per il formato condizionale della tabella pivot.

```csharp
public PivotConditionFormatRuleType RuleType { get; set; }
```

### Esempi

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
                // Crea dati minimi per la tabella pivot
                worksheet.Cells["A1"].Value = "Category";
                worksheet.Cells["A2"].Value = "Value";

                // Crea tabella pivot
                int pivotIndex = worksheet.PivotTables.Add("A1:A2", "C3", "DemoPivotTable");
                PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

                // Aggiungi formato condizionale
                int formatIndex = pivotTable.ConditionalFormats.Add();
                PivotConditionalFormat format = pivotTable.ConditionalFormats[formatIndex];

                // Dimostra la proprietà RuleType
                Console.WriteLine("Initial RuleType: " + format.RuleType);
                
                // Imposta un nuovo tipo di regola
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

### Vedi anche

* enum [PivotConditionFormatRuleType](../../pivotconditionformatruletype/)
* class [PivotConditionalFormat](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


