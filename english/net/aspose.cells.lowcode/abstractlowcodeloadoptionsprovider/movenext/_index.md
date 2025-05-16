---
title: AbstractLowCodeLoadOptionsProvider.MoveNext
second_title: Aspose.Cells for .NET API Reference
description: AbstractLowCodeLoadOptionsProvider method. Checks whether there is more input
type: docs
url: /net/aspose.cells.lowcode/abstractlowcodeloadoptionsprovider/movenext/
---
## AbstractLowCodeLoadOptionsProvider.MoveNext method

Checks whether there is more input.

```csharp
public abstract bool MoveNext()
```

### Examples

```csharp
namespace AsposeCellsExamples.AbstractLowCodeLoadOptionsProviderMethodMoveNextDemo
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class AbstractLowCodeLoadOptionsProviderMethodMoveNextDemo
    {
        public static void Run()
        {
            // Create a custom provider that implements AbstractLowCodeLoadOptionsProvider
            var provider = new MultiFileProvider();

            // Process multiple files using the provider
            int fileCount = 0;
            while (provider.MoveNext())
            {
                fileCount++;
                Console.WriteLine($"Processing file {fileCount}");

                // Get current load options
                var currentOptions = provider.Current;
                
                // Create a new workbook with current options
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];
                
                // Demonstrate processing
                worksheet.Cells["A1"].Value = $"Processed file {fileCount}";
                worksheet.Cells["A2"].Value = $"Has input file: {currentOptions.InputFile != null}";
                
                // Save each processed file
                workbook.Save($"ProcessedFile_{fileCount}.xlsx");
            }

            Console.WriteLine($"Total files processed: {fileCount}");
        }

        private class MultiFileProvider : AbstractLowCodeLoadOptionsProvider
        {
            private int currentIndex = -1;
            private readonly LowCodeLoadOptions[] fileOptions = new LowCodeLoadOptions[]
            {
                new LowCodeLoadOptions(),
                new LowCodeLoadOptions(),
                new LowCodeLoadOptions()
            };

            public override LowCodeLoadOptions Current => 
                currentIndex >= 0 && currentIndex < fileOptions.Length ? fileOptions[currentIndex] : null;

            public override bool MoveNext()
            {
                currentIndex++;
                return currentIndex < fileOptions.Length;
            }

            public override void Finish(LowCodeLoadOptions part)
            {
                // Cleanup if needed
            }
        }
    }
}
```

### See Also

* class [AbstractLowCodeLoadOptionsProvider](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


