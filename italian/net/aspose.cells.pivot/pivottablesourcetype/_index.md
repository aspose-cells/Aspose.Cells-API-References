---
title: "Enum PivotTableSourceType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Aspose.Cells.Pivot.PivotTableSourceType enum. Rappresenta il tipo di origine dati della tabella pivot"
type: docs
url: /it/net/aspose.cells.pivot/pivottablesourcetype/
---
## PivotTableSourceType enumeration

Rappresenta il tipo di origine dati della PivotTable.

```csharp
public enum PivotTableSourceType : byte
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| Sheet | `1` | Specifica che i dati di origine sono un intervallo. |
| External | `2` | Specifica che vengono utilizzati dati di origine esterni. |
| Consolidation | `4` | Specifica che più intervalli di consolidamento sono usati come dati di origine. |
| Scenario | `8` | I dati di origine sono popolati da una struttura interna temporanea. |
| Unknown | `9` | Origine dati sconosciuta. |

### Esempi

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
            // Crea un nuovo workbook per la dimostrazione
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Aggiungi dati di esempio al foglio di lavoro
                worksheet.Cells["A1"].PutValue("Category");
                worksheet.Cells["B1"].PutValue("Value");
                worksheet.Cells["A2"].PutValue("A");
                worksheet.Cells["B2"].PutValue(10);
                worksheet.Cells["A3"].PutValue("B");
                worksheet.Cells["B3"].PutValue(20);
                worksheet.Cells["A4"].PutValue("C");
                worksheet.Cells["B4"].PutValue(30);

                // Crea una raccolta di tabelle pivot
                PivotTableCollection pivotTables = worksheet.PivotTables;

                // Aggiungi una tabella pivot usando Sheet come tipo di origine
                int index = pivotTables.Add("=A1:B4", "D3", "SheetPivotTable");
                PivotTable pivotTable = pivotTables[index];

                // Visualizza il tipo di origine
                Console.WriteLine("Pivot Table Source Type: " + pivotTable.SourceType);

                // Dimostra diversi tipi di origine
                Console.WriteLine("Available PivotTableSourceType values:");
                Console.WriteLine("Sheet: " + PivotTableSourceType.Sheet);
                Console.WriteLine("External: " + PivotTableSourceType.External);
                Console.WriteLine("Consolidation: " + PivotTableSourceType.Consolidation);
                Console.WriteLine("Scenario: " + PivotTableSourceType.Scenario);
                Console.WriteLine("Unknown: " + PivotTableSourceType.Unknown);

                // Salva la cartella di lavoro
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

### Vedi anche

* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)


