---
title: ExternalLink.IsVisible
second_title: Aspose.Cells for .NET API Reference
description: ExternalLink property. Indicates whether this external link is visible in MS Excel
type: docs
url: /net/aspose.cells/externallink/isvisible/
---
## ExternalLink.IsVisible property

Indicates whether this external link is visible in MS Excel.

```csharp
public bool IsVisible { get; }
```

### Examples

```csharp
// Called: Assert.IsTrue(workbook.Worksheets.ExternalLinks[4].IsVisible);
[Test]
        public void Property_IsVisible()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;CELLSNET47157.xls&quot;);

            Assert.IsTrue(workbook.Worksheets.ExternalLinks[4].IsVisible);
            Assert.IsFalse(workbook.Worksheets.ExternalLinks[3].IsVisible);
             workbook = new Workbook(Constants.sourcePath + &quot;CELLSNET47157.xlsx&quot;);
            int c = 0;
            for (int i = 0; i &lt; workbook.Worksheets.ExternalLinks.Count; i++)
            {
                if (!workbook.Worksheets.ExternalLinks[i].IsVisible)
                {
                    continue;
                }

                c++;
            }
            Assert.AreEqual(3, c);

        }
```

### See Also

* class [ExternalLink](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


