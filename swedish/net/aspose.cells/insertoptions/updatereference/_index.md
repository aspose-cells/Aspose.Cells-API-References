---
title: "InsertOptions.UpdateReference"
second_title: "Aspose.Cells för .NET API‑referens"
description: "InsertOptions‑egenskap. Anger om referenser i andra arbetsblad kommer att uppdateras"
type: docs
url: /sv/net/aspose.cells/insertoptions/updatereference/
---
## InsertOptions.UpdateReference property

Anger om referenser i andra kalkylblad kommer att uppdateras.

```csharp
public bool UpdateReference { get; set; }
```

### Anmärkningar

Från och med 26.7 sätter vi standardvärdet för denna egenskap till true.

### Exempel

```csharp
using System;
using System.Collections.Generic;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class InsertOptionsPropertyUpdateReferenceDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok
            Workbook wb = new Workbook();
            
            // Lägg till ett andra arbetsblad och ange formler som refererar till Sheet1
            Worksheet sheet2 = wb.Worksheets.Add("Sheet2");
            sheet2.Cells["A1"].Formula = "=Sheet1!A10";
            sheet2.Cells["B1"].Formula = "=Sheet1!A5";
            
            // Ange formler i Sheet1
            Worksheet sheet1 = wb.Worksheets[0];
            sheet1.Cells["A1"].Formula = "=A10";
            sheet1.Cells["B1"].Formula = "=A5";

            // Skapa insert‑alternativ med UpdateReference aktiverat
            InsertOptions iopts = new InsertOptions();
            iopts.UpdateReference = true;
            
            // Spåra formelförändringar
            HashSet<string> changedCells = new HashSet<string>();
            iopts.UpdateReference = true;
            
            // Infoga rader som kommer att uppdatera referenser i formler
            sheet1.Cells.InsertRows(5, 3, iopts);
            
            // Skriv ut antalet ändrade celler
            Console.WriteLine("Formulas were automatically updated due to UpdateReference=true");
            
            // Visa de uppdaterade formlerna
            Console.WriteLine("Sheet1 A1 formula: " + sheet1.Cells["A1"].Formula);
            Console.WriteLine("Sheet2 A1 formula: " + sheet2.Cells["A1"].Formula);
        }
    }
}
```

### Se även

* class [InsertOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


