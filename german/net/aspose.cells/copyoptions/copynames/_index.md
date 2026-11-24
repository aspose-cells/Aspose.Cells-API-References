---
title: "CopyOptions.CopyNames"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "CopyOptions-Eigenschaft. Gibt an, ob die Namen kopiert werden."
type: docs
url: /de/net/aspose.cells/copyoptions/copynames/
---
## CopyOptions.CopyNames property

Gibt an, ob die Namen kopiert werden.

```csharp
public bool CopyNames { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CopyOptionsPropertyCopyNamesDemo
    {
        public static void Run()
        {
            // Erstelle eine Quell-Arbeitsmappe mit benannten Bereichen.
            Workbook sourceWorkbook = new Workbook();
            Worksheet sourceSheet = sourceWorkbook.Worksheets[0];
            
            // Erstelle einen benannten Bereich in der Quell-Arbeitsmappe.
            sourceSheet.Cells["A1"].PutValue("Test Value");
            int index = sourceWorkbook.Worksheets.Names.Add("SourceName");
            sourceWorkbook.Worksheets.Names[index].RefersTo = "=Sheet1!$A$1";

            // Erstelle eine Ziel-Arbeitsmappe.
            Workbook destWorkbook = new Workbook();
            
            // Arbeitsblatt kopieren mit CopyNames=true.
            destWorkbook.Worksheets[0].Copy(sourceSheet, new CopyOptions { CopyNames = true });

            // Überprüfe, ob der benannte Bereich kopiert wurde.
            Name copiedName = destWorkbook.Worksheets.Names["SourceName"];
            if (copiedName != null)
            {
                Console.WriteLine("Named range copied successfully: " + copiedName.RefersTo);
            }
            else
            {
                Console.WriteLine("Named range was not copied");
            }
        }
    }
}
```

### Siehe auch

* class [CopyOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


