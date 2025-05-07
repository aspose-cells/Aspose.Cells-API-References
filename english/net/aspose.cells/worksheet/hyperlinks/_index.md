---
title: Worksheet.Hyperlinks
second_title: Aspose.Cells for .NET API Reference
description: Worksheet property. Gets the HyperlinkCollection collection
type: docs
url: /net/aspose.cells/worksheet/hyperlinks/
---
## Worksheet.Hyperlinks property

Gets the [`HyperlinkCollection`](../../hyperlinkcollection/) collection.

```csharp
public HyperlinkCollection Hyperlinks { get; }
```

### Examples

```csharp
// Called: worksheet.Hyperlinks.Add("A1", 1, 1, "https://www.aspose.com");
public static void Property_Hyperlinks()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add some data to the worksheet
            worksheet.Cells["A1"].PutValue("Click here to visit Aspose");
            worksheet.Hyperlinks.Add("A1", 1, 1, "https://www.aspose.com");

            // Create HtmlSaveOptions and set the LinkTargetType
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            saveOptions.LinkTargetType = HtmlLinkTargetType.Blank; // Opens the link in a new window or tab

            // Save the workbook to HTML format
            workbook.Save("HtmlLinkTargetTypeExample.html", saveOptions);

            Console.WriteLine("HTML file saved with link target type set to '_blank'.");
        }
```

### See Also

* class [HyperlinkCollection](../../hyperlinkcollection/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


