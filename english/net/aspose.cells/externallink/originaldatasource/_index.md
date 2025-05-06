---
title: ExternalLink.OriginalDataSource
second_title: Aspose.Cells for .NET API Reference
description: ExternalLink property. Represents stored data source of the external link
type: docs
url: /net/aspose.cells/externallink/originaldatasource/
---
## ExternalLink.OriginalDataSource property

Represents stored data source of the external link.

```csharp
public string OriginalDataSource { get; set; }
```

### Examples

```csharp
// Called: Console.WriteLine(&amp;quot;Original Data Source:&amp;quot; + workbook.Worksheets.ExternalLinks[i].OriginalDataSource);
[Test]
        public void Property_OriginalDataSource()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;CELLSNET45470.xlsx&quot;);
            //for (int i = 0; i &lt; workbook.Worksheets.ExternalLinks.Count; i++)
            int i = 1;
            {
                Console.WriteLine((i + 1).ToString() + &quot;. &quot; + workbook.Worksheets.ExternalLinks[i].DataSource);
#if !LINUX_TEST
                Assert.IsTrue(workbook.Worksheets.ExternalLinks[i].DataSource.StartsWith(&quot;S:&quot;));
                Console.WriteLine(&quot;Original Data Source:&quot; + workbook.Worksheets.ExternalLinks[i].OriginalDataSource);
                //Console.WriteLine(&quot;ToString:&quot; + workbook.Worksheets.ExternalLinks[i].ToString());
#endif
            }
        }
```

### See Also

* class [ExternalLink](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


