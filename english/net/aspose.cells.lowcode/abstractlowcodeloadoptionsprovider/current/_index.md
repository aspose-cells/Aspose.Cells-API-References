---
title: AbstractLowCodeLoadOptionsProvider.Current
second_title: Aspose.Cells for .NET API Reference
description: AbstractLowCodeLoadOptionsProvider property. Gets the load options from which to load data of currently processed part
type: docs
url: /net/aspose.cells.lowcode/abstractlowcodeloadoptionsprovider/current/
---
## AbstractLowCodeLoadOptionsProvider.Current property

Gets the load options from which to load data of currently processed part.

```csharp
public abstract LowCodeLoadOptions Current { get; }
```

### Examples

```csharp
namespace AsposeCellsExamples.AbstractLowCodeLoadOptionsProviderPropertyCurrentDemo
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class AbstractLowCodeLoadOptionsProviderPropertyCurrentDemo
    {
        public static void Run()
        {
            // Create load options with different configurations
            LowCodeLoadOptions options1 = new LowCodeLoadOptions();
            LowCodeLoadOptions options2 = new LowCodeLoadOptions();

            // Initialize custom provider with our load options
            using (CustomProvider provider = new CustomProvider(new[] { options1, options2 }))
            {
                int counter = 1;
                while (provider.MoveNext())
                {
                    // Access Current property to get active load options
                    Console.WriteLine($"Processing set {counter}");
                    
                    // Create workbook using current load options' input file/stream
                    Workbook workbook;
                    if (provider.Current.InputFile != null)
                    {
                        workbook = new Workbook(provider.Current.InputFile);
                    }
                    else if (provider.Current.InputStream != null)
                    {
                        workbook = new Workbook(provider.Current.InputStream);
                    }
                    else
                    {
                        workbook = new Workbook();
                    }

                    Worksheet worksheet = workbook.Worksheets[0];

                    // Demonstrate option impact removed due to missing property
                    worksheet.Cells["A1"].Value = "Sample Value";

                    // Save result
                    workbook.Save($"CurrentDemo_{counter}.xlsx");
                    counter++;
                }
            }
        }
    }

    // Custom provider implementation with IDisposable
    public class CustomProvider : AbstractLowCodeLoadOptionsProvider, IDisposable
    {
        private readonly LowCodeLoadOptions[] _options;
        private int _index = -1;

        public CustomProvider(LowCodeLoadOptions[] options)
        {
            _options = options;
        }

        public override bool MoveNext()
        {
            _index++;
            return _index < _options.Length;
        }

        public override LowCodeLoadOptions Current => 
            _index >= 0 && _index < _options.Length ? _options[_index] : null;

        public override void Finish(LowCodeLoadOptions part)
        {
            // Optional cleanup logic
        }

        public void Dispose()
        {
            // Implement IDisposable if needed
        }
    }
}
```

### See Also

* class [LowCodeLoadOptions](../../lowcodeloadoptions/)
* class [AbstractLowCodeLoadOptionsProvider](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


