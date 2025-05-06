---
title: ExternalLinkCollection.Count
second_title: Aspose.Cells for .NET API Reference
description: ExternalLinkCollection property. Gets the number of elements actually contained in the collection
type: docs
url: /net/aspose.cells/externallinkcollection/count/
---
## ExternalLinkCollection.Count property

Gets the number of elements actually contained in the collection.

```csharp
public int Count { get; }
```

### Examples

```csharp
// Called: Assert.IsTrue(externalLinks[externalLinks.Count-1].DataSource.StartsWith(&amp;quot;http&amp;quot;));
[Test]
        public void Property_Count()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;Forecast_CY11_-_Corporate_Summary.xls&quot;);
            ExternalLinkCollection externalLinks = workbook.Worksheets.ExternalLinks;
            Assert.IsTrue(externalLinks[externalLinks.Count-1].DataSource.StartsWith(&quot;http&quot;));
        }
```

### See Also

* class [ExternalLinkCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


