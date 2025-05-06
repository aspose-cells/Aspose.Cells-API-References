---
title: SaveOptions.MergeAreas
second_title: Aspose.Cells for .NET API Reference
description: SaveOptions property. Indicates whether merge the areas of conditional formatting and validation before saving the file
type: docs
url: /net/aspose.cells/saveoptions/mergeareas/
---
## SaveOptions.MergeAreas property

Indicates whether merge the areas of conditional formatting and validation before saving the file.

```csharp
public bool MergeAreas { get; set; }
```

### Remarks

The default value is false.

### Examples

```csharp
// Called: saveOptions.MergeAreas = true;
public static void Property_MergeAreas()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fill some data into the worksheet
            worksheet.Cells[&quot;A1&quot;].PutValue(&quot;Name&quot;);
            worksheet.Cells[&quot;B1&quot;].PutValue(&quot;Age&quot;);
            worksheet.Cells[&quot;A2&quot;].PutValue(&quot;John&quot;);
            worksheet.Cells[&quot;B2&quot;].PutValue(30);
            worksheet.Cells[&quot;A3&quot;].PutValue(&quot;Jane&quot;);
            worksheet.Cells[&quot;B3&quot;].PutValue(25);

            // Create an instance of XlsSaveOptions
            XlsSaveOptions saveOptions = new XlsSaveOptions();

            // Setting properties
            saveOptions.MatchColor = true;
            saveOptions.ClearData = false;
            saveOptions.ValidateMergedAreas = true;
            saveOptions.MergeAreas = true;
            saveOptions.SortNames = true;
            saveOptions.SortExternalNames = false;
            saveOptions.RefreshChartCache = true;
            saveOptions.UpdateSmartArt = false;

            // Save the workbook with the specified save options
            workbook.Save(&quot;XlsSaveOptionsExample.xlsx&quot;, saveOptions);

            return;
        }
```

### See Also

* class [SaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


