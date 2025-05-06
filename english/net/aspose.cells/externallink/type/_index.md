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
// Called: Console.WriteLine(&amp;quot;External Link Type: &amp;quot; + externalLink.Type);
public static void Property_Type()
        {
            // Open a file with external links
            Workbook workbook = new Workbook(&quot;UpdatedExternalLinkExample_original.xlsx&quot;);

            // Get External Link 
            ExternalLink externalLink = workbook.Worksheets.ExternalLinks[0];

            // Display properties of the external link
            Console.WriteLine(&quot;External Link Type: &quot; + externalLink.Type);
            Console.WriteLine(&quot;Path Type: &quot; + externalLink.PathType);
            Console.WriteLine(&quot;Original Data Source: &quot; + externalLink.OriginalDataSource);
            Console.WriteLine(&quot;Data Source: &quot; + externalLink.DataSource);
            Console.WriteLine(&quot;Is Referred: &quot; + externalLink.IsReferred);
            Console.WriteLine(&quot;Is Visible: &quot; + externalLink.IsVisible);

            // Change External Link&apos;s Data Source
            externalLink.DataSource = &quot;d:\\linktest.xls&quot;;

            // Add an external name to the external link
            externalLink.AddExternalName(&quot;ExternalName&quot;, &quot;Sheet1!A1&quot;);

            // Save the workbook
            workbook.Save(&quot;UpdatedExternalLinkExample.xlsx&quot;);

            return;
        }
```

### See Also

* enum [ExternalLinkType](../../externallinktype/)
* class [ExternalLink](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


