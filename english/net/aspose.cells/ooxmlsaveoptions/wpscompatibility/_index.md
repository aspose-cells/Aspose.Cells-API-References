---
title: OoxmlSaveOptions.WpsCompatibility
second_title: Aspose.Cells for .NET API Reference
description: OoxmlSaveOptions property. Indicates whether to make the xls more compatible with WPS
type: docs
url: /net/aspose.cells/ooxmlsaveoptions/wpscompatibility/
---
## OoxmlSaveOptions.WpsCompatibility property

Indicates whether to make the xls more compatible with WPS.

```csharp
[Obsolete("Use WorkbookSetting.WpsCompatibility property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool WpsCompatibility { get; set; }
```

### Remarks

NOTE: This member is now obsolete. Instead, please use WorkbookSetting.WpsCompatibility property. This method will be removed 12 months later since December 2025. Aspose apologizes for any inconvenience you may have experienced.

### Examples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class OoxmlSaveOptionsPropertyWpsCompatibilityDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            
            // Access first worksheet and add sample data
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Test WPS Compatibility");
            
            // Create OOXML save options and enable WPS compatibility
            OoxmlSaveOptions options = new OoxmlSaveOptions();
            options.WpsCompatibility = true;
            
            // Save the workbook with WPS compatibility
            workbook.Save("output_with_wps_compatibility.xlsx", options);
            
            Console.WriteLine("Workbook saved with WPS compatibility enabled.");
        }
    }
}
```

### See Also

* class [OoxmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


