---
title: "VbaProject.IsValidSigned"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "VbaProject-Eigenschaft. Gibt an, ob die Signatur des VBA-Projekts gültig ist oder nicht."
type: docs
url: /de/net/aspose.cells.vba/vbaproject/isvalidsigned/
---
## VbaProject.IsValidSigned property

Gibt an, ob die Signatur des VBA-Projekts gültig ist oder nicht.

```csharp
public bool IsValidSigned { get; }
```

### Beispiele

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class VbaProjectPropertyIsValidSignedDemo
    {
        public static void Run()
        {
            // Laden Sie eine Beispielarbeitsmappe mit signiertem VBA-Projekt.
            Workbook wb = new Workbook("example.xlsm");
            
            // Überprüfen Sie, ob das VBA-Projekt signiert ist und die Signatur gültig ist.
            Console.WriteLine("Is VBA Project Signed: " + wb.VbaProject.IsSigned);
            Console.WriteLine("Is Signature Valid: " + wb.VbaProject.IsValidSigned);

            // Speichern und erneut laden, um zu überprüfen, ob die Signatur erhalten bleibt.
            MemoryStream ms = new MemoryStream();
            wb.Save(ms, SaveFormat.Excel97To2003);
            
            Workbook validateWb = new Workbook(ms);
            Console.WriteLine("After Reload - Is VBA Project Signed: " + validateWb.VbaProject.IsSigned);
            Console.WriteLine("After Reload - Is Signature Valid: " + validateWb.VbaProject.IsValidSigned);
        }
    }
}
```

### Siehe auch

* class [VbaProject](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


