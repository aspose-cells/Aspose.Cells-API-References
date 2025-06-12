---
title: WriteProtection.Password
second_title: Aspose.Cells for .NET API Reference
description: WriteProtection property. Sets the protected password to modify the file
type: docs
url: /net/aspose.cells/writeprotection/password/
---
## WriteProtection.Password property

Sets the protected password to modify the file.

```csharp
public string Password { get; set; }
```

### Examples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WriteProtectionPropertyPasswordDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            
            // Access the first worksheet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Set write protection password
            workbook.Settings.WriteProtection.Password = "owner";
            
            // Save the workbook
            workbook.Save("WriteProtectedWorkbook.xlsx");
            
            Console.WriteLine("Workbook write-protected with password successfully.");
        }
    }
}
```

### See Also

* class [WriteProtection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


