---
title: "VbaModule.Name"
second_title: "Aspose.Cells för .NET API‑referens"
description: "VbaModule-egenskap. Hämtar och anger namnet på modulen"
type: docs
url: /sv/net/aspose.cells.vba/vbamodule/name/
---
## VbaModule.Name property

Hämtar och anger namnet på modulen.

```csharp
public string Name { get; set; }
```

### Exempel

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Vba;

namespace AsposeCellsExamples
{
    public class VbaModulePropertyNameDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook wb = new Workbook();

            // Lägg till ett kalkylblad och hämta dess VBA-modul
            Worksheet sheet = wb.Worksheets[0];
            int moduleIndex = wb.VbaProject.Modules.Add(sheet);
            VbaModule module = wb.VbaProject.Modules[moduleIndex];

            // Ange modulnamnet
            module.Name = "Sheet1";

            // Lägg till enkel VBA-kod i modulen
            string vbaCode = "Private Sub Worksheet_SelectionChange(ByVal Target As Range)\r\n" +
                             "    MsgBox \"Sheet name: \" & Me.Name\r\n" +
                             "End Sub\r\n";
            module.Codes = vbaCode;

            // Spara till minnesström (för demonstration)
            using (MemoryStream ms = new MemoryStream())
            {
                wb.Save(ms, SaveFormat.Xlsm);
            }
        }
    }
}
```

### Se även

* class [VbaModule](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


