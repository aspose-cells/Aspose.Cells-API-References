---
title: SpreadsheetConverter.Process
second_title: Aspose.Cells for .NET API Reference
description: SpreadsheetConverter method. Converts given template file between spreadsheet file formats
type: docs
url: /net/aspose.cells.lowcode/spreadsheetconverter/process/
---
## Process(string, string) {#process_1}

Converts given template file between spreadsheet file formats.

```csharp
public static void Process(string templateFile, string resultFile)
```

| Parameter | Type | Description |
| --- | --- | --- |
| templateFile | String | The template file to be converted |
| resultFile | String | The resultant file |

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class SpreadsheetConverterMethodProcessWithStringStringDemo
    {
        public static void Run()
        {
            // Create template workbook and save to file
            Workbook templateWorkbook = new Workbook();
            templateWorkbook.Worksheets[0].Cells["A1"].PutValue("Sample Data");
            templateWorkbook.Save("template.xlsx", SaveFormat.Xlsx);

            try
            {
                // Convert template.xlsx to result.xlsb
                SpreadsheetConverter.Process("template.xlsx", "result.xlsb");
                
                Console.WriteLine("Process method completed successfully. File converted to XLSB format.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error during conversion: {ex.Message}");
            }
        }
    }
}
```

### See Also

* class [SpreadsheetConverter](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)

---

## Process(LowCodeLoadOptions, LowCodeSaveOptions) {#process}

Converts between different spreadsheet file formats.

```csharp
public static void Process(LowCodeLoadOptions loadOptions, LowCodeSaveOptions saveOptions)
```

| Parameter | Type | Description |
| --- | --- | --- |
| loadOptions | LowCodeLoadOptions | Options for input and loading |
| saveOptions | LowCodeSaveOptions | Options for output and saving |

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class SpreadsheetConverterMethodProcessWithLowCodeLoadOptionsLowCodeSaveODemo
    {
        public static void Run()
        {
            // Create a sample input file
            using (Workbook workbook = new Workbook())
            {
                workbook.Worksheets[0].Cells["A1"].PutValue("Process Method Demo");
                workbook.Save("LowCodeInput.xlsx");
            }

            try
            {
                // Create load options with input file
                LowCodeLoadOptions loadOptions = new LowCodeLoadOptions();
                typeof(LowCodeLoadOptions).GetProperty("FileName").SetValue(loadOptions, "LowCodeInput.xlsx");

                // Create save options with output file
                LowCodeSaveOptions saveOptions = new LowCodeSaveOptions();
                typeof(LowCodeSaveOptions).GetProperty("FileName").SetValue(saveOptions, "LowCodeOutput.xlsb");

                // Execute conversion
                SpreadsheetConverter.Process(loadOptions, saveOptions);

                Console.WriteLine("Process method executed. Output saved to LowCodeOutput.xlsb");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Process method: {ex.Message}");
            }
        }
    }
}
```

### See Also

* class [LowCodeLoadOptions](../../lowcodeloadoptions/)
* class [LowCodeSaveOptions](../../lowcodesaveoptions/)
* class [SpreadsheetConverter](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


