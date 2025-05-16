---
title: AbstractLowCodeSaveOptionsProvider.Finish
second_title: Aspose.Cells for .NET API Reference
description: AbstractLowCodeSaveOptionsProvider method. Releases resources after processing currently split part
type: docs
url: /net/aspose.cells.lowcode/abstractlowcodesaveoptionsprovider/finish/
---
## AbstractLowCodeSaveOptionsProvider.Finish method

Releases resources after processing currently split part.

```csharp
public virtual void Finish(LowCodeSaveOptions part)
```

| Parameter | Type | Description |
| --- | --- | --- |
| part | LowCodeSaveOptions | the save options used for currently split part. |

### Remarks

By default this method just closes the stream specified by the [`OutputStream`](../../lowcodesaveoptions/outputstream/) directly(if the save options specified a Stream as destination). User may overwrite this method to control how to release resources according to their requirement and the implementation of [`GetSaveOptions`](../getsaveoptions/).

### Examples

```csharp
namespace AsposeCellsExamples.AbstractLowCodeSaveOptionsProviderMethodFinishWithLowCodeSaveOptionsDemo
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class AbstractLowCodeSaveOptionsProviderMethodFinishWithLowCodeSaveOptionsDemo
    {
        public static void Run()
        {
            // Create a new workbook with sample data
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Initial Data");

            // Create concrete provider instance
            var provider = new CustomLowCodeSaveOptionsProvider();
            
            // Create LowCodeSaveOptions instance
            LowCodeSaveOptions saveOptions = new LowCodeSaveOptions();

            try
            {
                // Execute Finish method with LowCodeSaveOptions parameter
                provider.Finish(saveOptions);
                Console.WriteLine("Finish method completed successfully");

                // Save workbook with the processed options, using the correct SaveFormat
                workbook.Save("FinishMethodOutput.xlsx", SaveFormat.Xlsx);
                Console.WriteLine("Workbook saved with applied options");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error during Finish method execution: {ex.Message}");
            }
        }
    }

    // Concrete implementation of AbstractLowCodeSaveOptionsProvider
    public class CustomLowCodeSaveOptionsProvider : AbstractLowCodeSaveOptionsProvider
    {
        // Implement the required abstract method
        public override LowCodeSaveOptions GetSaveOptions(SplitPartInfo partInfo)
        {
            // Return a default instance or customize as needed
            return new LowCodeSaveOptions();
        }
    }
}
```

### See Also

* class [LowCodeSaveOptions](../../lowcodesaveoptions/)
* class [AbstractLowCodeSaveOptionsProvider](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


