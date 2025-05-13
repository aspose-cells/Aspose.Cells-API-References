---
title: ExternalLink.PathType
second_title: Aspose.Cells for .NET API Reference
description: ExternalLink property. Get the path type of this external link
type: docs
url: /net/aspose.cells/externallink/pathtype/
---
## ExternalLink.PathType property

Get the path type of this external link

```csharp
public string PathType { get; }
```

### Examples

```csharp
// Called: Console.WriteLine("Path Type: " + externalLink.PathType);
public static void ExternalLink_Property_PathType()
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

* class [ExternalLink](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


