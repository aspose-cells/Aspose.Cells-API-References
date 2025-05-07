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
public static void Property_Type()
        {
            // Open a file with external links
            Workbook workbook = new Workbook("UpdatedExternalLinkExample_original.xlsx");

            // Get External Link 
            ExternalLink externalLink = workbook.Worksheets.ExternalLinks[0];

            // Display properties of the external link
            Console.WriteLine("External Link Type: " + externalLink.Type);
            Console.WriteLine("Path Type: " + externalLink.PathType);
            Console.WriteLine("Original Data Source: " + externalLink.OriginalDataSource);
            Console.WriteLine("Data Source: " + externalLink.DataSource);
            Console.WriteLine("Is Referred: " + externalLink.IsReferred);
            Console.WriteLine("Is Visible: " + externalLink.IsVisible);

            // Change External Link's Data Source
            externalLink.DataSource = "d:\\linktest.xls";

            // Add an external name to the external link
            externalLink.AddExternalName("ExternalName", "Sheet1!A1");

            // Save the workbook
            workbook.Save("UpdatedExternalLinkExample.xlsx");

            return;
        }
```

### See Also

* enum [ExternalLinkType](../../externallinktype/)
* class [ExternalLink](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


