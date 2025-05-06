---
title: WorkbookSettings.Compliance
second_title: Aspose.Cells for .NET API Reference
description: WorkbookSettings property. Specifies the OOXML version for the output document. The default value is Ecma376_2006
type: docs
url: /net/aspose.cells/workbooksettings/compliance/
---
## WorkbookSettings.Compliance property

Specifies the OOXML version for the output document. The default value is Ecma376_2006.

```csharp
public OoxmlCompliance Compliance { get; set; }
```

### Remarks

Only for .xlsx files.

### Examples

```csharp
// Called: settings.Compliance = OoxmlCompliance.Iso29500_2008_Strict;
public static void Property_Compliance()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();

            // Access workbook settings
            WorkbookSettings settings = workbook.Settings;

            // Set the OOXML compliance level to ISO/IEC 29500:2008 Strict
            settings.Compliance = OoxmlCompliance.Iso29500_2008_Strict;

            // Add some data to the worksheet
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells[0, 0].PutValue(&quot;Hello, World!&quot;);

            // Save the workbook with the specified OOXML compliance level
            workbook.Save(&quot;OoxmlComplianceExample.xlsx&quot;);

            return;
        }
```

### See Also

* enum [OoxmlCompliance](../../ooxmlcompliance/)
* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


