---
title: AbstractLowCodeSaveOptionsProvider.GetSaveOptions
second_title: Aspose.Cells for .NET API Reference
description: AbstractLowCodeSaveOptionsProvider method. Gets the save options from which to get the output settings for currently split part. Returning null denotes to skip given part
type: docs
url: /net/aspose.cells.lowcode/abstractlowcodesaveoptionsprovider/getsaveoptions/
---
## AbstractLowCodeSaveOptionsProvider.GetSaveOptions method

Gets the save options from which to get the output settings for currently split part. Returning null denotes to skip given part.

```csharp
public abstract LowCodeSaveOptions GetSaveOptions(SplitPartInfo part)
```

### Examples

```csharp
namespace AsposeCellsExamples.AbstractLowCodeSaveOptionsProviderMethodGetSaveOptionsWithSplitPartInfoDemo
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class AbstractLowCodeSaveOptionsProviderMethodGetSaveOptionsWithSplitPartInfoDemo
    {
        public static void Run()
        {
            // Create a custom provider by extending AbstractLowCodeSaveOptionsProvider
            var provider = new CustomSaveOptionsProvider();

            // Create a workbook with sample data
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Sample Data");

            // Create a SplitPartInfo instance (simulated since constructor isn't public)
            var splitPartInfo = (SplitPartInfo)Activator.CreateInstance(typeof(SplitPartInfo), nonPublic: true);
            typeof(SplitPartInfo).GetProperty("PartIndex").SetValue(splitPartInfo, 0);
            typeof(SplitPartInfo).GetProperty("SheetIndex").SetValue(splitPartInfo, 0);
            typeof(SplitPartInfo).GetProperty("SheetName").SetValue(splitPartInfo, "Sheet1");

            try
            {
                // Call GetSaveOptions with SplitPartInfo parameter
                LowCodeSaveOptions saveOptions = provider.GetSaveOptions(splitPartInfo);

                // Configure save options
                saveOptions.SaveFormat = SaveFormat.Xlsx;
                saveOptions.OutputFile = "OutputWithSplitPartInfo.xlsx";

                Console.WriteLine($"Save options created for part {splitPartInfo.PartIndex} of sheet {splitPartInfo.SheetName}");

                // Demonstrate finishing the process
                provider.Finish(saveOptions);
                Console.WriteLine("Process completed successfully");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetSaveOptions: {ex.Message}");
            }
        }
    }

    // Custom implementation of AbstractLowCodeSaveOptionsProvider
    public class CustomSaveOptionsProvider : AbstractLowCodeSaveOptionsProvider
    {
        public override LowCodeSaveOptions GetSaveOptions(SplitPartInfo partInfo)
        {
            if (partInfo == null)
            {
                throw new ArgumentNullException(nameof(partInfo));
            }

            // Create custom save options based on part info
            return new LowCodeSaveOptions
            {
                SaveFormat = SaveFormat.Xlsx,
                OutputFile = $"Part_{partInfo.PartIndex}_Sheet_{partInfo.SheetName}.xlsx"
            };
        }
    }
}
```

### See Also

* class [LowCodeSaveOptions](../../lowcodesaveoptions/)
* class [SplitPartInfo](../../splitpartinfo/)
* class [AbstractLowCodeSaveOptionsProvider](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


