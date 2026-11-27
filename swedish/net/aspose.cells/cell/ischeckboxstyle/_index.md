---
title: "Cell.IsCheckBoxStyle"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Cell-egenskap. Anger om cellen är inställd som en check box"
type: docs
url: /sv/net/aspose.cells/cell/ischeckboxstyle/
---
## Cell.IsCheckBoxStyle property

Anger om cellen är inställd som en kryssruta.

```csharp
public bool IsCheckBoxStyle { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellPropertyIsCheckBoxStyleDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Åtkomst till det första kalkylbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Åtkomst till cell B1 och sätt den till checkbox-stil
            Cell cell = worksheet.Cells["B1"];
            cell.IsCheckBoxStyle = true;
            cell.PutValue(true);
            
            // Åtkomst till cell A1 och sätt den till checkbox-stil med ett värde
            cell = worksheet.Cells["A1"];
            cell.IsCheckBoxStyle = true;
            cell.PutValue(false);
            
            // Spara arbetsboken
            workbook.Save("CheckBoxStyleDemo.xlsx");
            
            // Läs in den sparade arbetsboken för att verifiera egenskaperna
            Workbook loadedWorkbook = new Workbook("CheckBoxStyleDemo.xlsx");
            worksheet = loadedWorkbook.Worksheets[0];
            
            // Verifiera att B1 är i checkbox-stil
            cell = worksheet.Cells["B1"];
            Console.WriteLine("Cell B1 IsCheckBoxStyle: " + cell.IsCheckBoxStyle);
            
            // Ändra B1 till icke-checkbox-stil och spara
            cell.IsCheckBoxStyle = false;
            loadedWorkbook.Save("CheckBoxStyleDemo_Modified.xlsx");
        }
    }
}
```

### Se även

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


