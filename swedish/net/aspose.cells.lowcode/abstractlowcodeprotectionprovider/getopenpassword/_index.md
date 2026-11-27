---
title: "AbstractLowCodeProtectionProvider.GetOpenPassword"
second_title: "Aspose.Cells för .NET API‑referens"
description: "AbstractLowCodeProtectionProvider metod. Hämtar lösenordet för att öppna kalkylbladsfilen"
type: docs
url: /sv/net/aspose.cells.lowcode/abstractlowcodeprotectionprovider/getopenpassword/
---
## AbstractLowCodeProtectionProvider.GetOpenPassword method

Hämtar lösenordet för att öppna kalkylbladsfilen.

```csharp
public virtual string GetOpenPassword()
```

### Returvärde

Lösenord för att öppna kalkylbladsfilen. Tom betyder inget skydd för att öppna filen.

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class AbstractLowCodeProtectionProviderMethodGetOpenPasswordDemo
    {
        public static void Run()
        {
            try
            {
                // Skapa en instans av skyddsleverantör
                var protectionProvider = new DemoProtectionProvider();

                // Anropa GetOpenPassword-metoden för att hämta lösenordet
                string password = protectionProvider.GetOpenPassword();

                // Skapa en ny arbetsbok och tillämpa lösenordet
                Workbook workbook = new Workbook("sample.xlsx");
                workbook.Settings.Password = password;

                // Spara den lösenordsskyddade arbetsboken
                workbook.Save("MethodGetOpenPasswordDemo.xlsx");

                Console.WriteLine($"Workbook protected with open password: {password}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing demo: {ex.Message}");
            }
        }
    }

    public class DemoProtectionProvider : AbstractLowCodeProtectionProvider
    {
        public override string GetOpenPassword()
        {
            return "AsposeDemo123!";
        }
    }
}
```

### Se även

* class [AbstractLowCodeProtectionProvider](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


