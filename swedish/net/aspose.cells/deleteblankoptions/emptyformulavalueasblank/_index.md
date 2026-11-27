---
title: "DeleteBlankOptions.EmptyFormulaValueAsBlank"
second_title: "Aspose.Cells för .NET API‑referens"
description: "DeleteBlankOptions egenskap. Anger om en cell ska betraktas som tom när den är en formel och det beräknade resultatet är null eller en tom sträng. Standardvärdet är false"
type: docs
url: /sv/net/aspose.cells/deleteblankoptions/emptyformulavalueasblank/
---
## DeleteBlankOptions.EmptyFormulaValueAsBlank property

Om en cell ska betraktas som tom när den är en formel och det beräknade resultatet är null eller en tom sträng. Standardvärdet är false.

```csharp
public bool EmptyFormulaValueAsBlank { get; set; }
```

### Anmärkningar

Generellt bör användaren se till att formlerna har beräknats innan raderingsoperationen med denna egenskap är sann. Annars kommer alla nyss skapade formler av vanliga API:er såsom [`Formula`](../../cell/formula/) att tas som tomma och kan raderas eftersom deras beräknade resultat är null innan beräkning.

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DeleteBlankOptionsPropertyEmptyFormulaValueAsBlankDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            Cells cells = sheet.Cells;

            // Fyll i exempeldata
            cells["A1"].PutValue("Header");
            cells["A2"].Formula = "=B2";  // Formula returning blank
            cells["A3"].PutValue("Data");
            cells["A4"].Formula = "=1+1"; // Formula with value
            
            // Ta bort tomma rader utan att beakta tomma formler
            Console.WriteLine("Before deletion (normal): " + cells.MaxRow + " rows");
            cells.DeleteBlankRows();
            Console.WriteLine("After normal deletion: " + cells.MaxRow + " rows");

            // Återställ data
            cells.ClearContents(0, 0, cells.MaxRow + 1, cells.MaxColumn + 1);
            cells["A1"].PutValue("Header");
            cells["A2"].Formula = "=B2";
            cells["A3"].PutValue("Data");
            cells["A4"].Formula = "=1+1";

            // Ta bort tomma rader och behandla formler som tomma
            Console.WriteLine("\nBefore deletion (with EmptyFormulaValueAsBlank): " + cells.MaxRow + " rows");
            cells.DeleteBlankRows(new DeleteBlankOptions() { EmptyFormulaValueAsBlank = true });
            Console.WriteLine("After deletion with EmptyFormulaValueAsBlank: " + cells.MaxRow + " rows");
        }
    }
}
```

### Se även

* class [DeleteBlankOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


