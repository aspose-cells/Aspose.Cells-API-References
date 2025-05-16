---
title: StreamProviderOptions.StreamProviderOptions
second_title: Aspose.Cells for .NET API Reference
description: StreamProviderOptions constructor. Initializes a new instance of the StreamProviderOptions class
type: docs
url: /net/aspose.cells/streamprovideroptions/streamprovideroptions/
---
## StreamProviderOptions(ResourceLoadingType, string) {#constructor_1}

Initializes a new instance of the [`StreamProviderOptions`](../) class.

```csharp
public StreamProviderOptions(ResourceLoadingType loadingType, string defaultPath)
```

| Parameter | Type | Description |
| --- | --- | --- |
| loadingType | ResourceLoadingType | The type to load the linked resource. |
| defaultPath | String | The default path. |

### Examples

```csharp
namespace AsposeCellsExamples.StreamProviderOptionsMethodCtorWithResourceLoadingTypeStringDemo
{
    using Aspose.Cells;
    using System;

    public class StreamProviderOptionsMethodCtorWithResourceLoadingTypeStringDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Call the #ctor method with ResourceLoadingType.Default and a default path
                StreamProviderOptions options = new StreamProviderOptions(ResourceLoadingType.Default, "output_files/");

                // Display the properties set by the constructor
                Console.WriteLine($"ResourceLoadingType: {options.ResourceLoadingType}");
                Console.WriteLine($"DefaultPath: {options.DefaultPath}");

                // Set additional properties
                options.CustomPath = "custom_output/";
                options.Stream = null; // Can be set to a specific stream if needed

                // Use the options when saving (example with HTML save options)
                HtmlSaveOptions saveOptions = new HtmlSaveOptions();
                saveOptions.StreamProvider = (IStreamProvider)options;

                // Save the workbook to demonstrate the effect
                workbook.Save("StreamProviderOptionsDemo.html", saveOptions);

                Console.WriteLine("Workbook saved with StreamProviderOptions settings.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing #ctor method: {ex.Message}");
            }
        }
    }
}
```

### See Also

* enum [ResourceLoadingType](../../resourceloadingtype/)
* class [StreamProviderOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## StreamProviderOptions() {#constructor}

Initializes a new instance of the [`StreamProviderOptions`](../) class.

```csharp
public StreamProviderOptions()
```

### Examples

```csharp
namespace AsposeCellsExamples.StreamProviderOptionsMethodCtorDemo
{
    using Aspose.Cells;
    using System;
    using System.IO;

    public class StreamProviderOptionsMethodCtorDemo
    {
        public static void Run()
        {
            try
            {
                // Demonstrate parameterless constructor
                StreamProviderOptions options1 = new StreamProviderOptions();
                Console.WriteLine("Parameterless constructor:");
                Console.WriteLine($"ResourceLoadingType: {options1.ResourceLoadingType}");
                Console.WriteLine($"DefaultPath: {options1.DefaultPath}");

                // Demonstrate constructor with parameters
                StreamProviderOptions options2 = new StreamProviderOptions(
                    ResourceLoadingType.Default, 
                    "output_files/");
                
                Console.WriteLine("\nConstructor with parameters:");
                Console.WriteLine($"ResourceLoadingType: {options2.ResourceLoadingType}");
                Console.WriteLine($"DefaultPath: {options2.DefaultPath}");

                // Set additional properties
                options2.CustomPath = "custom_path/";
                options2.Stream = new MemoryStream();

                // Create a workbook and save with stream options
                Workbook workbook = new Workbook();
                workbook.Worksheets[0].Cells["A1"].PutValue("StreamProviderOptions Demo");
                
                HtmlSaveOptions saveOptions = new HtmlSaveOptions();
                saveOptions.StreamProvider = (IStreamProvider)options2;
                
                workbook.Save("StreamProviderOptionsDemo.html", saveOptions);
                Console.WriteLine("\nWorkbook saved with custom stream options");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing StreamProviderOptions constructor demo: {ex.Message}");
            }
        }
    }
}
```

### See Also

* class [StreamProviderOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


