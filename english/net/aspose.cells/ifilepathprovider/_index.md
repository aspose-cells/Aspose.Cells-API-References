---
title: Interface IFilePathProvider
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.IFilePathProvider interface. Represents the exported file path provider
type: docs
url: /net/aspose.cells/ifilepathprovider/
---
## IFilePathProvider interface

Represents the exported file path provider.

```csharp
public interface IFilePathProvider
```

## Methods

| Name | Description |
| --- | --- |
| [GetFullName](../../aspose.cells/ifilepathprovider/getfullname/)(string) | Gets the full path of the file by Worksheet name when exporting Worksheet to HTML separately. So the references among the Worksheets can be exported correctly. |

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class IFilePathProviderDemo : IFilePathProvider
    {
        // Implementing the GetFullName method from the IFilePathProvider interface
        public string GetFullName(string sheetName)
        {
            // For demonstration, return a simple file path based on the sheet name
            return $"{sheetName}.html";
        }

        public static void IFilePathProviderExample()
        {
            // Create a new workbook and add some data
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Hello");
            worksheet.Cells["A2"].PutValue("World");

            // Create HtmlSaveOptions and set the FilePathProvider
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            saveOptions.FilePathProvider = new IFilePathProviderDemo();

            // Save the workbook to HTML format
            workbook.Save("IFilePathProviderExample.html", saveOptions);

            Console.WriteLine("Workbook saved to HTML with custom file paths.");
        }
    }


}
```

### See Also

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


