---
title: LowCodeSplitOptions.LoadOptions
second_title: Aspose.Cells for .NET API Reference
description: LowCodeSplitOptions property. Load options for loading the spreadsheet that will be split
type: docs
url: /net/aspose.cells.lowcode/lowcodesplitoptions/loadoptions/
---
## LowCodeSplitOptions.LoadOptions property

Load options for loading the spreadsheet that will be split.

```csharp
public LowCodeLoadOptions LoadOptions { get; set; }
```

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells.LowCode;
    using System;

    public class LowCodeSplitOptionsPropertyLoadOptionsDemo
    {
        public static void Run()
        {
            // Create split options instance
            LowCodeSplitOptions splitOptions = new LowCodeSplitOptions();

            // Initialize load options
            splitOptions.LoadOptions = new LowCodeLoadOptions();

            // Create new load options with different settings (using available properties)
            splitOptions.LoadOptions = new LowCodeLoadOptions();
            
            // Demonstrate final configuration
            Console.WriteLine("LoadOptions configured with InputFile: " + splitOptions.LoadOptions.InputFile);
        }
    }
}
```

### See Also

* class [LowCodeLoadOptions](../../lowcodeloadoptions/)
* class [LowCodeSplitOptions](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


