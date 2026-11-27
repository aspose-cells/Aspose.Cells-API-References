---
title: "Cells.DeleteBlankColumns"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Cells-metod. Ta bort alla tomma kolumner som inte innehåller någon data"
type: docs
url: /sv/net/aspose.cells/cells/deleteblankcolumns/
---
## DeleteBlankColumns() {#deleteblankcolumns}

Ta bort alla tomma kolumner som inte innehåller någon data.

```csharp
public void DeleteBlankColumns()
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodDeleteBlankColumnsDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Kom åt första arbetsbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till lite testdata med tomma kolumner
            worksheet.Cells["A1"].PutValue("Column A");
            worksheet.Cells["C1"].PutValue("Column C"); // Column B will be blank
            worksheet.Cells["A2"].PutValue("Data A");
            worksheet.Cells["C2"].PutValue("Data C");
            
            // Ta bort tomma kolumner
            worksheet.Cells.DeleteBlankColumns();
            
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

## DeleteBlankColumns(DeleteOptions) {#deleteblankcolumns_1}

Ta bort alla tomma kolumner som inte innehåller någon data.

```csharp
public void DeleteBlankColumns(DeleteOptions options)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| alternativ | DeleteOptions | Alternativen för att radera intervallet. |

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodDeleteBlankColumnsWithDeleteOptionsDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok med exempeldata
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till lite data med tomma kolumner
            worksheet.Cells["A1"].PutValue("Column A");
            worksheet.Cells["C1"].PutValue("Column C"); // Column B is blank
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["C2"].PutValue(3);

            Console.WriteLine("Before deleting blank columns:");
            Console.WriteLine($"MaxDataColumn: {worksheet.Cells.MaxDataColumn}"); // Should be 2 (0-based, column C)

            // Ställ in raderingsalternativ
            DeleteOptions options = new DeleteOptions();
            options.UpdateReference = true;

            // Ta bort tomma kolumner
            worksheet.Cells.DeleteBlankColumns(options);

            Console.WriteLine("After deleting blank columns:");
            Console.WriteLine($"MaxDataColumn: {worksheet.Cells.MaxDataColumn}"); // Should be 1 (0-based, column A and C remain, B was deleted)

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


