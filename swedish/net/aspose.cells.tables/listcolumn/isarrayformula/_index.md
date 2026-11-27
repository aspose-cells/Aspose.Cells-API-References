---
title: "ListColumn.IsArrayFormula"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ListColumn property. Anger om formeln är en arrayformel"
type: docs
url: /sv/net/aspose.cells.tables/listcolumn/isarrayformula/
---
## ListColumn.IsArrayFormula property

Indikerar om formeln är en matrisformel.

```csharp
public bool IsArrayFormula { get; }
```

### Exempel

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
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();

            // Åtkomst till det första kalkylbladet
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata för att skapa en tabell
            worksheet.Cells["A1"].PutValue("ID");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["A3"].PutValue(2);
            worksheet.Cells["B3"].PutValue(20);

            // Skapa ett tabell/list-objekt
            int tableIndex = worksheet.ListObjects.Add(0, 0, 2, 1, true);
            ListObject listObject = worksheet.ListObjects[tableIndex];

            // Lägg till en arrayformel i den andra kolumnen
            listObject.ListColumns[1].Formula = "{=SUM(A2:A3*B2:B3)}";

            try
            {
                // Åtkomst till IsArrayFormula-egenskapen (skrivskyddad)
                bool isArrayFormula = listObject.ListColumns[1].IsArrayFormula;

                // Visa värdet
                Console.WriteLine("IsArrayFormula value: " + isArrayFormula);

                // Spara arbetsboken
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

### Se även

* class [ListColumn](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


