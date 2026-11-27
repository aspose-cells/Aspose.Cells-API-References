---
title: "AbstractLowCodeProtectionProvider.GetWorkbookPassword"
second_title: "Aspose.Cells för .NET API‑referens"
description: "AbstractLowCodeProtectionProvider-metod. Hämtar lösenordet för att skydda arbetsboken med angiven skyddstyp"
type: docs
url: /sv/net/aspose.cells.lowcode/abstractlowcodeprotectionprovider/getworkbookpassword/
---
## AbstractLowCodeProtectionProvider.GetWorkbookPassword method

Hämtar lösenordet för att skydda arbetsboken med angiven skyddstyp.

```csharp
public virtual string GetWorkbookPassword()
```

### Returvärde

Lösenord för att skydda workbooken.

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class AbstractLowCodeProtectionProviderMethodGetWorkbookPasswordDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            var provider = new DemoProtectionProvider();

            try
            {
                string password = provider.GetWorkbookPassword();
                ProtectionType protectionType = provider.GetWorkbookProtectionType();

                workbook.Protect(protectionType, password);
                Console.WriteLine($"Workbook protected with password: {password}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }

            workbook.Save("ProtectedWorkbook.xlsx");

        }
    }

    public class DemoProtectionProvider : AbstractLowCodeProtectionProvider
    {
        public override string GetWorkbookPassword()
        {
            return "Aspose1234!";
        }

        public override ProtectionType GetWorkbookProtectionType()
        {
            return ProtectionType.Structure;
        }
        
    }
}
```

### Se även

* class [AbstractLowCodeProtectionProvider](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


