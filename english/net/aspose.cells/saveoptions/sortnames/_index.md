---
title: SaveOptions.SortNames
second_title: Aspose.Cells for .NET API Reference
description: SaveOptions property. Indicates whether sorting defined names before saving file
type: docs
url: /net/aspose.cells/saveoptions/sortnames/
---
## SaveOptions.SortNames property

Indicates whether sorting defined names before saving file.

```csharp
public bool SortNames { get; set; }
```

### Examples

```csharp
// Called: saveOptions.SortNames = true;
public static void Property_SortNames()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fill some data into the worksheet
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue("Jane");
            worksheet.Cells["B3"].PutValue(25);

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
            workbook.Save("XlsSaveOptionsExample.xlsx", saveOptions);

            return;
        }
```

### See Also

* class [SaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


