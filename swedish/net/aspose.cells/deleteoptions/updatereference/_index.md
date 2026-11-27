---
title: "DeleteOptions.UpdateReference"
second_title: "Aspose.Cells för .NET API‑referens"
description: "DeleteOptions property. Anger om referenser ska uppdateras i andra kalkylblad"
type: docs
url: /sv/net/aspose.cells/deleteoptions/updatereference/
---
## DeleteOptions.UpdateReference property

Indikerar om referenser ska uppdateras i andra kalkylblad.

```csharp
public bool UpdateReference { get; set; }
```

### Anmärkningar

Från och med 26.7 sätter vi standardvärdet för denna egenskap till true.

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DeleteOptionsPropertyUpdateReferenceDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok med exempeldata
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata och formler
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["B1"].PutValue(20);
            worksheet.Cells["C1"].Formula = "=A1+B1";
            worksheet.Cells["A2"].PutValue(30);
            worksheet.Cells["B2"].PutValue(40);
            worksheet.Cells["C2"].Formula = "=A2+B2";

            // Skapa raderingsalternativ med UpdateReference satt till true
            DeleteOptions deleteOptions = new DeleteOptions();
            deleteOptions.UpdateReference = true;

            // Ta bort kolumn A som refereras i formler
            worksheet.Cells.DeleteColumns(0, 1, deleteOptions);

            // Spara arbetsboken
            workbook.Save("output.xlsx");
        }
    }
}
```

### Se även

* class [DeleteOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


