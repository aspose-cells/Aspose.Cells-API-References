---
title: "Cells.InsertRow"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Cells-metoden. Infogar en ny rad i kalkylbladet"
type: docs
url: /sv/net/aspose.cells/cells/insertrow/
---
## Cells.InsertRow method

Infogar en ny rad i kalkylbladet.

```csharp
public void InsertRow(int rowIndex)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| rowIndex | Int32 | Radindex. |

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodInsertRowWithInt32Demo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Åtkomst till det första kalkylbladet
            Worksheet sheet = workbook.Worksheets[0];
            
            // Hämta cellsamling
            Cells cells = sheet.Cells;
            
            // Infoga exempeldata i rad 6
            cells[6, 0].PutValue("Original Row 6");
            cells[6, 1].PutValue(100);
            
            // Infoga exempeldata i rad 7
            cells[7, 0].PutValue("Original Row 7");
            cells[7, 1].PutValue(200);
            
            // Infoga en ny rad på index 7 (skjuter befintlig rad 7 nedåt)
            cells.InsertRow(7);
            
            // Lägg till data i den nyinfogade raden
            cells[7, 0].PutValue("New Inserted Row");
            cells[7, 1].PutValue(150);
            
            // Spara arbetsboken
            workbook.Save("InsertRowDemo.xlsx");
            
            Console.WriteLine("Row inserted successfully at index 7.");
        }
    }
}
```

### Se även

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


