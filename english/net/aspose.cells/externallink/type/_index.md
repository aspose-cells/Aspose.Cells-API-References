---
title: ExternalLink.Type
second_title: Aspose.Cells for .NET API Reference
description: ExternalLink property. Gets the type of external link
type: docs
url: /net/aspose.cells/externallink/type/
---
## ExternalLink.Type property

Gets the type of external link.

```csharp
public ExternalLinkType Type { get; }
```

### Examples

```csharp
// Called: Console.WriteLine("External Link Type: " + externalLink.Type);
public static void ExternalLink_Property_Type()
        {
            // Open a file with external links
            Workbook workbook = new Workbook("ExternalLinkTypeExample_original.xlsx");

            // Get External Link 
            ExternalLink externalLink = workbook.Worksheets.ExternalLinks[0];

            // Display the type of external link
            Console.WriteLine("External Link Type: " + externalLink.Type);

            // Change External Link's Data Source
            externalLink.DataSource = "d:\\link.xls";

            // Save the workbook
            workbook.Save("ExternalLinkTypeExample.xlsx");
        }
```

### See Also

* enum [ExternalLinkType](../../externallinktype/)
* class [ExternalLink](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


