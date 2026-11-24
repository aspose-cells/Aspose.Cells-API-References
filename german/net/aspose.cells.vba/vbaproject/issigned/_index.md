---
title: "VbaProject.IsSigned"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "VbaProject-Eigenschaft. Gibt an, ob VBAcode signiert ist oder nicht."
type: docs
url: /de/net/aspose.cells.vba/vbaproject/issigned/
---
## VbaProject.IsSigned property

Gibt an, ob VBAcode signiert ist oder nicht.

```csharp
public bool IsSigned { get; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class VbaProjectPropertyIsSignedDemo
    {
        public static void Run()
        {
            // Laden Sie eine Beispiel-Excel-Datei mit VBA-Projekt.
            Workbook workbook = new Workbook("example.xlsm");
            
            // Überprüfen Sie, ob das VBA-Projekt signiert ist.
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

### Siehe auch

* class [VbaProject](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


