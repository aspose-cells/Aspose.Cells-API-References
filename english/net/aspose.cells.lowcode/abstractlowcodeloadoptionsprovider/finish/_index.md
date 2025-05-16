---
title: AbstractLowCodeLoadOptionsProvider.Finish
second_title: Aspose.Cells for .NET API Reference
description: AbstractLowCodeLoadOptionsProvider method. Releases resources after processing currently part of input
type: docs
url: /net/aspose.cells.lowcode/abstractlowcodeloadoptionsprovider/finish/
---
## AbstractLowCodeLoadOptionsProvider.Finish method

Releases resources after processing currently part of input.

```csharp
public virtual void Finish(LowCodeLoadOptions part)
```

| Parameter | Type | Description |
| --- | --- | --- |
| part | LowCodeLoadOptions | the load options used for currently split part. |

### Remarks

By default this method just closes the stream specified by the [`InputStream`](../../lowcodeloadoptions/inputstream/) directly(if the load options specified a Stream as source). User may overwrite this method to control how to release resources according to their requirement and the implementation of [`Current`](../current/).

### Examples

```csharp
namespace AsposeCellsExamples.AbstractLowCodeLoadOptionsProviderMethodFinishWithLowCodeLoadOptionsDemo
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class AbstractLowCodeLoadOptionsProviderMethodFinishWithLowCodeLoadOptionsDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            LowCodeLoadOptions loadOptions = new LowCodeLoadOptions();
            CustomLoadOptionsProvider provider = new CustomLoadOptionsProvider();

            try
            {
                provider.Finish(loadOptions);
                worksheet.Cells["A1"].Value = "Finish method called successfully";
                Console.WriteLine("Finish method executed with LowCodeLoadOptions parameter");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
                worksheet.Cells["A1"].Value = "Error occurred during Finish call";
            }

            workbook.Save("FinishMethodDemo.xlsx");
        }
    }

    public class CustomLoadOptionsProvider : AbstractLowCodeLoadOptionsProvider
    {
        private LowCodeLoadOptions current;

        public override LowCodeLoadOptions Current => current;

        public override bool MoveNext()
        {
            current = new LowCodeLoadOptions();
            return false;
        }
    }
}
```

### See Also

* class [LowCodeLoadOptions](../../lowcodeloadoptions/)
* class [AbstractLowCodeLoadOptionsProvider](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


