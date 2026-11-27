---
title: "Cell.IsInTable"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Cell‑egenskap. Anger om den här cellen är en del av tabellformeln"
type: docs
url: /sv/net/aspose.cells/cell/isintable/
---
## Cell.IsInTable property

Anger om den här cellen är en del av en tabellformel.

```csharp
[Obsolete("Use IsTableFormula instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool IsInTable { get; }
```

### Anmärkningar

OBS: Den här klassen är nu föråldrad. Använd istället Cell.IsTableFormula för att kontrollera om cellformeln är en del av tabellformeln. Denna egenskap kommer att tas bort 12 månader senare från och med maj 2018. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Tables;
    using System;

    public class CellPropertyIsInTableDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();

            // Åtkomst till det första kalkylbladet
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata i kalkylbladet
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Price");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["B2"].PutValue(1.5);
            worksheet.Cells["A3"].PutValue("Banana");
            worksheet.Cells["B3"].PutValue(0.8);

            // Skapa en tabell från dataområdet
            int tableIndex = worksheet.ListObjects.Add(0, 0, 3, 1, true);
            ListObject table = worksheet.ListObjects[tableIndex];

            try
            {
                // Kontrollera IsInTable‑egenskapen för celler inom och utanför tabellen
                Cell cellInTable = worksheet.Cells["A2"];
                Cell cellOutsideTable = worksheet.Cells["C2"];

                Console.WriteLine("Cell A2 (inside table):");
                Console.WriteLine("  Value: " + cellInTable.StringValue);
                Console.WriteLine("  IsInTable: " + cellInTable.IsInTable);

                Console.WriteLine("\nCell C2 (outside table):");
                Console.WriteLine("  Value: " + cellOutsideTable.StringValue);
                Console.WriteLine("  IsInTable: " + cellOutsideTable.IsInTable);

                // Spara arbetsboken
                workbook.Save("IsInTableDemo.xlsx");
                Console.WriteLine("\nWorkbook saved successfully.");
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

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


