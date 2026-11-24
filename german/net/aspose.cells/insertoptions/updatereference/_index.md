---
title: "InsertOptions.UpdateReference"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "InsertOptions-Eigenschaft. Gibt an, ob Verweise in anderen Arbeitsblättern aktualisiert werden"
type: docs
url: /de/net/aspose.cells/insertoptions/updatereference/
---
## InsertOptions.UpdateReference property

Gibt an, ob Verweise in anderen Arbeitsblättern aktualisiert werden.

```csharp
public bool UpdateReference { get; set; }
```

### Hinweise

Ab Version 26.7 setzen wir den Standardwert dieser Eigenschaft auf true.

### Beispiele

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
            // Erstelle eine Arbeitsmappe
            Workbook wb = new Workbook();
            
            // Fügen Sie ein zweites Arbeitsblatt hinzu und setzen Sie Formeln, die auf Sheet1 verweisen
            Worksheet sheet2 = wb.Worksheets.Add("Sheet2");
            sheet2.Cells["A1"].Formula = "=Sheet1!A10";
            sheet2.Cells["B1"].Formula = "=Sheet1!A5";
            
            // Setzen Sie Formeln in Sheet1
            Worksheet sheet1 = wb.Worksheets[0];
            sheet1.Cells["A1"].Formula = "=A10";
            sheet1.Cells["B1"].Formula = "=A5";

            // Erstellen Sie InsertOptions mit aktivierter UpdateReference
            InsertOptions iopts = new InsertOptions();
            iopts.UpdateReference = true;
            
            // Verfolgen Sie Änderungen von Formeln
            HashSet<string> changedCells = new HashSet<string>();
            iopts.UpdateReference = true;
            
            // Zeilen einfügen, die Verweise in Formeln aktualisieren
            sheet1.Cells.InsertRows(5, 3, iopts);
            
            // Geben Sie die Anzahl der geänderten Zellen aus
            Console.WriteLine("Formulas were automatically updated due to UpdateReference=true");
            
            // Zeigen Sie die aktualisierten Formeln an
            Console.WriteLine("Sheet1 A1 formula: " + sheet1.Cells["A1"].Formula);
            Console.WriteLine("Sheet2 A1 formula: " + sheet2.Cells["A1"].Formula);
        }
    }
}
```

### Siehe auch

* class [InsertOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


