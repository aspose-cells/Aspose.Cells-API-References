---
title: "WriteProtection.ValidatePassword"
second_title: "Aspose.Cells för .NET API‑referens"
description: "WriteProtection-metoden. Returnerar true om det angivna lösenordet är samma som skrivskyddslösenordet som filen skyddades med"
type: docs
url: /sv/net/aspose.cells/writeprotection/validatepassword/
---
## WriteProtection.ValidatePassword method

Returnerar true om det angivna lösenordet är samma som skrivskyddslösenordet som filen skyddades med.

```csharp
public bool ValidatePassword(string password)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| lösenord | String | Det angivna lösenordet. |

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WriteProtectionMethodValidatePasswordWithStringDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Ange lösenord för skrivskydd
            workbook.Settings.WriteProtection.Password = "1234";
            
            // Validera lösenord
            Console.WriteLine("Password '1234' is valid: " + 
                workbook.Settings.WriteProtection.ValidatePassword("1234"));
            Console.WriteLine("Password 'wrong' is valid: " + 
                workbook.Settings.WriteProtection.ValidatePassword("wrong"));
        }
    }
}
```

### Se även

* class [WriteProtection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


