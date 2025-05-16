---
title: AbstractLowCodeProtectionProvider.GetWorkbookPassword
second_title: Aspose.Cells for .NET API Reference
description: AbstractLowCodeProtectionProvider method. Gets the password to protect the workbook with specified protection type
type: docs
url: /net/aspose.cells.lowcode/abstractlowcodeprotectionprovider/getworkbookpassword/
---
## AbstractLowCodeProtectionProvider.GetWorkbookPassword method

Gets the password to protect the workbook with specified protection type.

```csharp
public virtual string GetWorkbookPassword()
```

### Return Value

Password to protect the workbook.

### Examples

```csharp
namespace AsposeCellsExamples.AbstractLowCodeProtectionProviderMethodGetWorkbookPasswordDemo
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
        public override string GetWorkbookPassword() => "Aspose1234!";
        
        public override ProtectionType GetWorkbookProtectionType() => ProtectionType.Structure;

        // Required overrides with default implementations
        public override string GetOpenPassword() => null;
        public override string GetWritePassword() => null;
        public override string GetWorksheetPassword(string sheetName) => null;
        public override ProtectionType GetWorksheetProtectionType(string sheetName) => ProtectionType.None;
    }
}
```

### See Also

* class [AbstractLowCodeProtectionProvider](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


