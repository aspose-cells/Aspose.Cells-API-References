---
title: "VbaProject.IsValidSigned"
second_title: "Aspose.Cells för .NET API‑referens"
description: "VbaProject-egenskap. Anger om signaturen för VBA-projektet är giltig eller inte"
type: docs
url: /sv/net/aspose.cells.vba/vbaproject/isvalidsigned/
---
## VbaProject.IsValidSigned property

Anger om signaturen för VBA-projektet är giltig eller inte.

```csharp
public bool IsValidSigned { get; }
```

### Exempel

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
            // Läs in en exempelarbetsbok med signerat VBA-projekt
            Workbook wb = new Workbook("example.xlsm");
            
            // Kontrollera om VBA-projektet är signerat och om signaturen är giltig
            Console.WriteLine("Is VBA Project Signed: " + wb.VbaProject.IsSigned);
            Console.WriteLine("Is Signature Valid: " + wb.VbaProject.IsValidSigned);

            // Spara och ladda om för att verifiera att signaturen kvarstår
            MemoryStream ms = new MemoryStream();
            wb.Save(ms, SaveFormat.Excel97To2003);
            
            Workbook validateWb = new Workbook(ms);
            Console.WriteLine("After Reload - Is VBA Project Signed: " + validateWb.VbaProject.IsSigned);
            Console.WriteLine("After Reload - Is Signature Valid: " + validateWb.VbaProject.IsValidSigned);
        }
    }
}
```

### Se även

* class [VbaProject](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


