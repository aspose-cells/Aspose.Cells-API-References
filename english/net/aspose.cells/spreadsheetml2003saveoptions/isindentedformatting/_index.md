---
title: SpreadsheetML2003SaveOptions.IsIndentedFormatting
second_title: Aspose.Cells for .NET API Reference
description: SpreadsheetML2003SaveOptions property. Causes child elements to be indented
type: docs
url: /net/aspose.cells/spreadsheetml2003saveoptions/isindentedformatting/
---
## SpreadsheetML2003SaveOptions.IsIndentedFormatting property

Causes child elements to be indented.

```csharp
public bool IsIndentedFormatting { get; set; }
```

### Remarks

The default value is true. If the value is false, it will reduce the size of the xml file

### Examples

```csharp
// Called: saveOptions.IsIndentedFormatting = true;
public static void SpreadsheetML2003SaveOptions_Property_IsIndentedFormatting()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fill some data into the worksheet
            worksheet.Cells["A1"].PutValue("Hello");
            worksheet.Cells["B1"].PutValue("World");
            worksheet.Cells["A2"].PutValue(123);
            worksheet.Cells["B2"].PutValue(456);

            // Create an instance of SpreadsheetML2003SaveOptions
            SpreadsheetML2003SaveOptions saveOptions = new SpreadsheetML2003SaveOptions();

            // Set properties
            saveOptions.IsIndentedFormatting = true;
            saveOptions.LimitAsXls = false;
            saveOptions.ExportColumnIndexOfCell = true;
            saveOptions.ClearData = false;
            saveOptions.CachedFileFolder = @"C:\Temp";
            saveOptions.ValidateMergedAreas = true;
            saveOptions.MergeAreas = true;
            saveOptions.SortNames = true;
            saveOptions.SortExternalNames = true;
            saveOptions.RefreshChartCache = true;
            saveOptions.UpdateSmartArt = false;

            // Save the workbook with the specified save options
            workbook.Save("example.xml", saveOptions);

            return;
        }
```

### See Also

* class [SpreadsheetML2003SaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


