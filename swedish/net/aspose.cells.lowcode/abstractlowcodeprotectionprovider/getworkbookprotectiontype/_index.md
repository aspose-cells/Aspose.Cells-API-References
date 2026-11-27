---
title: "AbstractLowCodeProtectionProvider.GetWorkbookProtectionType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "AbstractLowCodeProtectionProvider-metod. Hämtar skyddstypen för att skydda arbetsboken"
type: docs
url: /sv/net/aspose.cells.lowcode/abstractlowcodeprotectionprovider/getworkbookprotectiontype/
---
## AbstractLowCodeProtectionProvider.GetWorkbookProtectionType method

Hämtar skyddstypen för att skydda arbetsboken.

```csharp
public virtual ProtectionType GetWorkbookProtectionType()
```

### Returvärde

Skyddstyp för att skydda arbetsboken. Ingen betyder att arbetsboken inte är skyddad.

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class AbstractLowCodeProtectionProviderMethodGetWorkbookProtectionTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            
            var provider = new CustomProtectionProvider();

            try
            {
                workbook.Protect(provider.GetWorkbookProtectionType(), provider.GetWorkbookPassword());
                
                ProtectionType protectionType = provider.GetWorkbookProtectionType();
                Console.WriteLine($"Workbook protection type: {protectionType}");
                Console.WriteLine($"Protection status: {workbook.Settings.IsProtected}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetWorkbookProtectionType: {ex.Message}");
            }

            workbook.Save("WorkbookProtectionDemo.xlsx");
        }


        private class CustomProtectionProvider : AbstractLowCodeProtectionProvider
        {
            public override ProtectionType GetWorkbookProtectionType()
            {
                return ProtectionType.Structure;
            }

            public override string GetWorkbookPassword()
            {
                return "aspose123";
            }
        }
    }
}
```

### Se även

* enum [ProtectionType](../../../aspose.cells/protectiontype/)
* class [AbstractLowCodeProtectionProvider](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


