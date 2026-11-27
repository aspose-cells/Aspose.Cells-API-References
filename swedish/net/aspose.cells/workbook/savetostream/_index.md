---
title: "Workbook.SaveToStream"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Workbook-metod. Sparar Excel-fil till ett MemoryStream-objekt som en Excel972003 xls-fil och returnerar den"
type: docs
url: /sv/net/aspose.cells/workbook/savetostream/
---
## Workbook.SaveToStream method

Sparar Excel-filen till ett MemoryStream-objekt som en Excel97-2003 xls-fil och returnerar den.

```csharp
public MemoryStream SaveToStream()
```

### Returvärde

MemoryStream-objekt som innehåller en xls Excel-fil.

### Anmärkningar

Denna metod tillhandahåller samma funktion som Save-metoden och sparar endast arbetsboken som en Excel97-2003 xls-fil. Den är främst avsedd för anrop från COM-klienter.

### Exempel

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodSaveToStreamDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook start = new Workbook();
            
            // Öppna första kalkylbladet och lägg till lite exempeldata
            Worksheet worksheet = start.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(20);

            // Spara arbetsboken till minnesström
            MemoryStream stream = start.SaveToStream();

            // Skapa ny arbetsbok från strömmen
            Workbook workbook = new Workbook(stream);

            // Modifiera den nya arbetsboken
            Worksheet newWorksheet = workbook.Worksheets[0];
            var area = CellArea.CreateCellArea(3, 0, 3, 1);
            newWorksheet.Cells.InsertRange(area, 3, ShiftType.Down, true);

            newWorksheet.Cells["A4"].PutValue("D");
            newWorksheet.Cells["B4"].PutValue(40);
            newWorksheet.Cells["A5"].PutValue("E");
            newWorksheet.Cells["B5"].PutValue(50);
            newWorksheet.Cells["A6"].PutValue("F");
            newWorksheet.Cells["B6"].PutValue(60);

            // Spara den modifierade arbetsboken
            workbook.Save("output.xlsx");
        }
    }
}
```

### Se även

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


