---
title: AbstractLowCodeProtectionProvider.GetWorksheetProtectionType
second_title: Aspose.Cells for .NET API Reference
description: AbstractLowCodeProtectionProvider method. Gets the protection type to protect the specified worksheet
type: docs
url: /net/aspose.cells.lowcode/abstractlowcodeprotectionprovider/getworksheetprotectiontype/
---
## AbstractLowCodeProtectionProvider.GetWorksheetProtectionType method

Gets the protection type to protect the specified worksheet.

```csharp
public virtual ProtectionType GetWorksheetProtectionType(string sheetName)
```

### Return Value

Protection type to protect the specified worksheet. None means no protection for the worksheet.

### Examples

```csharp
namespace AsposeCellsExamples.AbstractLowCodeProtectionProviderMethodGetWorksheetProtectionTypeWithStringDemo
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class AbstractLowCodeProtectionProviderMethodGetWorksheetProtectionTypeWithStringDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            string sheetName = worksheet.Name;

            // Create an instance of AbstractLowCodeProtectionProvider
            AbstractLowCodeProtectionProvider protectionProvider = new AbstractLowCodeProtectionProvider();

            try
            {
                // Call GetWorksheetProtectionType with the sheet name parameter
                ProtectionType protectionType = protectionProvider.GetWorksheetProtectionType(sheetName);

                // Display the result
                Console.WriteLine($"Worksheet '{sheetName}' protection type: {protectionType}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error retrieving protection type: {ex.Message}");
            }

            // Save the workbook
            workbook.Save("GetWorksheetProtectionTypeDemo.xlsx");
        }
    }
}
```

### See Also

* enum [ProtectionType](../../../aspose.cells/protectiontype/)
* class [AbstractLowCodeProtectionProvider](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


