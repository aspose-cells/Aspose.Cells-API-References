---
title: "Cells.DeleteBlankRows"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Cells-metod. Ta bort alla tomma rader som inte innehåller någon data eller annat objekt"
type: docs
url: /sv/net/aspose.cells/cells/deleteblankrows/
---
## DeleteBlankRows() {#deleteblankrows}

Ta bort alla tomma rader som inte innehåller någon data eller annat objekt.

```csharp
public void DeleteBlankRows()
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodDeleteBlankRowsDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok med exempeldata
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Lägg till lite data med tomma rader
            cells["A1"].PutValue("Header");
            cells["A2"].PutValue("Data1");
            cells["A4"].PutValue("Data2"); // Blank row at A3
            cells["A6"].PutValue("Data3"); // Blank row at A5

            Console.WriteLine("Before deleting blank rows:");
            for (int i = 0; i < 7; i++)
            {
                Console.WriteLine($"Row {i + 1}: {cells[i, 0].StringValue}");
            }

            // Ta bort tomma rader
            cells.DeleteBlankRows();

            Console.WriteLine("\nAfter deleting blank rows:");
            for (int i = 0; i < cells.MaxDataRow + 1; i++)
            {
                Console.WriteLine($"Row {i + 1}: {cells[i, 0].StringValue}");
            }

            // Spara arbetsboken
            workbook.Save("output.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Se även

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## DeleteBlankRows(DeleteOptions) {#deleteblankrows_1}

Ta bort alla tomma rader som inte innehåller någon data eller vissa speciella objekt såsom synlig kommentar, pivottabell.

```csharp
public void DeleteBlankRows(DeleteOptions options)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| alternativ | DeleteOptions | Alternativen för att radera intervallet. |

### Anmärkningar

För tomma rader som ska tas bort krävs det inte bara att [`IsBlank`](../../row/isblank/) är true, utan också att det inte finns någon synlig kommentar definierad för någon cell i dessa rader, och ingen pivottabell vars område skär dem.

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodDeleteBlankRowsWithDeleteOptionsDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Kom åt första arbetsbladet
            Worksheet sheet = workbook.Worksheets[0];
            
            // Lägg till lite testdata med tomma rader
            sheet.Cells["A1"].PutValue("Data1");
            sheet.Cells["A3"].PutValue("Data2");
            sheet.Cells["A5"].PutValue("Data3");
            
            // Skapa raderingsalternativ
            DeleteOptions options = new DeleteOptions();
            options.UpdateReference = true;
            
            // Ta bort tomma rader
            sheet.Cells.DeleteBlankRows(options);
            
            // Spara arbetsboken
            workbook.Save("output.xlsx");
        }
    }
}
```

### Se även

* class [DeleteOptions](../../deleteoptions/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


