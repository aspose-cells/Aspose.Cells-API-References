---
title: "ListColumn.IsArrayFormula"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "proprietà ListColumn. Indica se la formula è una formula array"
type: docs
url: /it/net/aspose.cells.tables/listcolumn/isarrayformula/
---
## ListColumn.IsArrayFormula property

Indica se la formula è una formula di matrice.

```csharp
public bool IsArrayFormula { get; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Tables;
    using System;

    public class ListColumnPropertyIsArrayFormulaDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();

            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio per creare una tabella
            worksheet.Cells["A1"].PutValue("ID");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["A3"].PutValue(2);
            worksheet.Cells["B3"].PutValue(20);

            // Crea un oggetto tabella/elenco
            int tableIndex = worksheet.ListObjects.Add(0, 0, 2, 1, true);
            ListObject listObject = worksheet.ListObjects[tableIndex];

            // Aggiungi una formula array alla seconda colonna
            listObject.ListColumns[1].Formula = "{=SUM(A2:A3*B2:B3)}";

            try
            {
                // Accedi alla proprietà IsArrayFormula (di sola lettura)
                bool isArrayFormula = listObject.ListColumns[1].IsArrayFormula;

                // Visualizza il valore
                Console.WriteLine("IsArrayFormula value: " + isArrayFormula);

                // Salva la cartella di lavoro
                workbook.Save("IsArrayFormulaDemo.xlsx");
                Console.WriteLine("Demo completed successfully.");
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

* class [ListColumn](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


