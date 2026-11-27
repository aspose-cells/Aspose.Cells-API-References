---
title: "VbaProject.IsSigned"
second_title: "Aspose.Cells för .NET API‑referens"
description: "VbaProject-egenskap. Anger om VBAcode är signerad eller inte"
type: docs
url: /sv/net/aspose.cells.vba/vbaproject/issigned/
---
## VbaProject.IsSigned property

Anger om VBA-kod är signerat eller inte.

```csharp
public bool IsSigned { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class VbaProjectPropertyIsSignedDemo
    {
        public static void Run()
        {
            // Läs in en exempel-Excel-fil med VBA-projekt
            Workbook workbook = new Workbook("example.xlsm");
            
            // Kontrollera om VBA-projektet är signerat
            if (workbook.VbaProject.IsSigned)
            {
                Console.WriteLine("VBA project is signed.");
                Console.WriteLine("Signature is valid: " + workbook.VbaProject.IsValidSigned);
            }
            else
            {
                Console.WriteLine("VBA project is not signed.");
            }
        }
    }
}
```

### Se även

* class [VbaProject](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


