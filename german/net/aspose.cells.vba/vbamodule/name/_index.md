---
title: "VbaModule.Name"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "VbaModule-Eigenschaft. Gibt den Namen des Moduls zurück und legt ihn fest"
type: docs
url: /de/net/aspose.cells.vba/vbamodule/name/
---
## VbaModule.Name property

Liest und schreibt den Namen des Moduls.

```csharp
public string Name { get; set; }
```

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook wb = new Workbook();

            // Fügen Sie ein Arbeitsblatt hinzu und erhalten Sie dessen VBA-Modul
            Worksheet sheet = wb.Worksheets[0];
            int moduleIndex = wb.VbaProject.Modules.Add(sheet);
            VbaModule module = wb.VbaProject.Modules[moduleIndex];

            // Setzen Sie den Modulnamen
            module.Name = "Sheet1";

            // Fügen Sie einfachen VBA-Code zum Modul hinzu
            string vbaCode = "Private Sub Worksheet_SelectionChange(ByVal Target As Range)\r\n" +
                             "    MsgBox \"Sheet name: \" & Me.Name\r\n" +
                             "End Sub\r\n";
            module.Codes = vbaCode;

            // In einen Memory-Stream speichern (zur Demonstration)
            using (MemoryStream ms = new MemoryStream())
            {
                wb.Save(ms, SaveFormat.Xlsm);
            }
        }
    }
}
```

### Siehe auch

* class [VbaModule](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


