---
title: "VbaModule.BinaryCodes"
second_title: "Aspose.Cells för .NET API‑referens"
description: "VbaModule-egenskap. Hämtar och anger de binära koderna för modulen"
type: docs
url: /sv/net/aspose.cells.vba/vbamodule/binarycodes/
---
## VbaModule.BinaryCodes property

Hämtar och anger de binära koderna för modulen.

```csharp
public byte[] BinaryCodes { get; }
```

### Exempel

```csharp
using System;
using System.Text;
using Aspose.Cells;
using Aspose.Cells.Vba;

namespace AsposeCellsExamples
{
    public class VbaModulePropertyBinaryCodesDemo
    {
        public static void Run()
        {
            // Läs in arbetsboken med VBA-projektet
            Workbook workbook = new Workbook("example.xlsm");
            
            // Åtkomst till VBA-projektet
            VbaProject vbaProject = workbook.VbaProject;
            
            // Hämta binära koder från den första modulen
            byte[] binaryCodes = vbaProject.Modules[0].BinaryCodes;
            
            // Konvertera till sträng med kinesisk kodning (936)
            string codeContent = Encoding.GetEncoding(936).GetString(binaryCodes);
            
            // Skriv ut innehållet som innehåller kinesiska tecken
            Console.WriteLine("VBA Module Content:");
            Console.WriteLine(codeContent);
        }
    }
}
```

### Se även

* class [VbaModule](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


