---
title: "VbaProject.ValidatePassword"
second_title: "Aspose.Cells för .NET API‑referens"
description: "VbaProject metod. Validerar skyddslösenordet"
type: docs
url: /sv/net/aspose.cells.vba/vbaproject/validatepassword/
---
## VbaProject.ValidatePassword method

Validerar skyddslösenordet.

```csharp
public bool ValidatePassword(string password)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| lösenord | String | lösenordet |

### Returvärde

Om lösenordet är skyddslösenordet för detta VBA-projekt

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class VbaProjectMethodValidatePasswordWithStringDemo
    {
        public static void Run()
        {
            // Skapa arbetsbokobjekt från exempel‑Excel‑fil med VBA-projekt
            Workbook workbook = new Workbook("example.xlsm");
            
            // Validera VBA-projektets lösenord
            bool isValid = workbook.VbaProject.ValidatePassword("test");
            
            // Skriv ut valideringsresultatet
            Console.WriteLine("Password validation result: " + isValid);
        }
    }
}
```

### Se även

* class [VbaProject](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


