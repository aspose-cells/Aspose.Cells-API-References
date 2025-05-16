---
title: TxtLoadOptions.TxtLoadOptions
second_title: Aspose.Cells for .NET API Reference
description: TxtLoadOptions constructor. Creates the options for loading text file
type: docs
url: /net/aspose.cells/txtloadoptions/txtloadoptions/
---
## TxtLoadOptions() {#constructor}

Creates the options for loading text file.

```csharp
public TxtLoadOptions()
```

### Remarks

The default load file type is CSV .

### Examples

```csharp
// Called: TxtLoadOptions loadOptions = new TxtLoadOptions();
[Test, Category("Bug")]
        public void TxtLoadOptions_Constructor()
        {
            Workbook workbook = new Workbook();
            //workbook.Open(Constants.sourcePath + "example.csv", ',');           
            TxtLoadOptions loadOptions = new TxtLoadOptions();
            loadOptions.Separator = ',';
            workbook = new Workbook(Constants.sourcePath + "example.csv", loadOptions);
            Assert.IsTrue(workbook.Worksheets[0].Cells["A5"].GetStyle().IsDateTime);
            // Assert.AreEqual(workbook.Worksheets[0].Cells[0, 2].GetStyle().Custom, "YYYY-M-D".ToLower());
        }
```

### See Also

* class [TxtLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## TxtLoadOptions(LoadFormat) {#constructor_1}

Creates the options for loading text file.

```csharp
public TxtLoadOptions(LoadFormat loadFormat)
```

| Parameter | Type | Description |
| --- | --- | --- |
| loadFormat | LoadFormat | The loading format |

### Examples

```csharp
namespace AsposeCellsExamples.TxtLoadOptionsMethodCtorWithLoadFormatDemo
{
    using Aspose.Cells;
    using System;
    using System.IO;

    public class TxtLoadOptionsMethodCtorWithLoadFormatDemo
    {
        public static void Run()
        {
            // Create sample CSV content and temporary file
            string csvData = "Column1,Column2,Column3\nData1,Data2,Data3";
            string tempFile = Path.GetTempFileName();
            File.WriteAllText(tempFile, csvData);

            try
            {
                // Create TxtLoadOptions with LoadFormat.Csv
                TxtLoadOptions loadOptions = new TxtLoadOptions(LoadFormat.Csv);
                loadOptions.Separator = ',';
                loadOptions.HasTextQualifier = true;

                // Load CSV using the configured options
                Workbook workbook = new Workbook(tempFile, loadOptions);
                Worksheet worksheet = workbook.Worksheets[0];

                // Demonstrate loaded data
                Console.WriteLine($"A1 Cell Value: {worksheet.Cells["A1"].StringValue}");
                Console.WriteLine($"B2 Cell Value: {worksheet.Cells["B2"].StringValue}");

                // Save processed workbook
                workbook.Save("TxtLoadOptionsCtorDemoOutput.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing constructor: {ex.Message}");
            }
            finally
            {
                // Cleanup temporary file
                if (File.Exists(tempFile))
                {
                    File.Delete(tempFile);
                }
            }
        }
    }
}
```

### See Also

* enum [LoadFormat](../../loadformat/)
* class [TxtLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


