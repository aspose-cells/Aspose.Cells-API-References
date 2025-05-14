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
public static void SaveOptions_Property_MergeAreas()
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


