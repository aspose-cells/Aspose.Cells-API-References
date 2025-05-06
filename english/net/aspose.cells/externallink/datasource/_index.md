---
title: ExternalLink.DataSource
second_title: Aspose.Cells for .NET API Reference
description: ExternalLink property. Represents data source of the external link
type: docs
url: /net/aspose.cells/externallink/datasource/
---
## ExternalLink.DataSource property

Represents data source of the external link.

```csharp
public string DataSource { get; set; }
```

### Examples

```csharp
// Called: Console.WriteLine(&amp;quot;External Link &amp;quot; + i + &amp;quot; Data Source: &amp;quot; + link.DataSource);
public static void Property_DataSource()
        {
            // Open a file with external links
            Workbook workbook = new Workbook(&quot;ExternalLinkCollectionExample_original.xlsx&quot;);

            // Get the external links collection
            ExternalLinkCollection externalLinks = workbook.Worksheets.ExternalLinks;

            // Display the count of external links
            Console.WriteLine(&quot;Number of external links: &quot; + externalLinks.Count);

            // Iterate through the external links and display their data sources
            for (int i = 0; i &lt; externalLinks.Count; i++)
            {
                ExternalLink link = externalLinks[i];
                Console.WriteLine(&quot;External Link &quot; + i + &quot; Data Source: &quot; + link.DataSource);
            }

            // Add a new external link
            int newLinkIndex = externalLinks.Add(&quot;newLink.xls&quot;, new[] { &quot;Sheet1&quot; });
            Console.WriteLine(&quot;Added new external link at index: &quot; + newLinkIndex);

            // Change the data source of the first external link
            if (externalLinks.Count &gt; 0)
            {
                externalLinks[0].DataSource = &quot;d:\\link.xlsx&quot;;
                Console.WriteLine(&quot;Updated data source of the first external link.&quot;);
            }

            // Save the workbook
            workbook.Save(&quot;ExternalLinkCollectionExample.xlsx&quot;);

            // Clear all external links
            externalLinks.Clear();
            Console.WriteLine(&quot;Cleared all external links.&quot;);

            // Save the workbook after clearing external links
            workbook.Save(&quot;ExternalLinkCollectionExample2.xlsx&quot;);
        }
```

### See Also

* class [ExternalLink](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


