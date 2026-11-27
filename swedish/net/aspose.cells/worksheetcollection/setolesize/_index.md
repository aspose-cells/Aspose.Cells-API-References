---
title: "WorksheetCollection.SetOleSize"
second_title: "Aspose.Cells för .NET API‑referens"
description: "WorksheetCollection-metod. Anger visad storlek när Workbook-filen används som ett Ole-objekt"
type: docs
url: /sv/net/aspose.cells/worksheetcollection/setolesize/
---
## WorksheetCollection.SetOleSize method

Ställer in visad storlek när Workbook‑filen används som ett Ole‑objekt.

```csharp
public void SetOleSize(int startRow, int endRow, int startColumn, int endColumn)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| startRow | Int32 | Startradindex. |
| endRow | Int32 | Slutradindex. |
| startColumn | Int32 | Startkolumnindex. |
| endColumn | Int32 | Slutkolumnindex. |

### Anmärkningar

Denna metod används vanligtvis för att justera visningsstorleken i ppt-fil eller doc-fil.

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetCollectionMethodSetOleSizeWithInt32Int32Int32Int32Demo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Ange OLE-storlek för kalkylbladen
            workbook.Worksheets.SetOleSize(0, 10, 0, 10);
            
            // Spara arbetsboken
            workbook.Save("output.xlsx");
            
            // Verifiera OLE-storleken
            Workbook loadedWorkbook = new Workbook("output.xlsx");
            CellArea oleSize = (CellArea)loadedWorkbook.Worksheets.OleSize;
            Console.WriteLine("OLE Size - StartRow: {0}, EndRow: {1}, StartColumn: {2}, EndColumn: {3}", 
                oleSize.StartRow, oleSize.EndRow, oleSize.StartColumn, oleSize.EndColumn);
        }
    }
}
```

### Se även

* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


