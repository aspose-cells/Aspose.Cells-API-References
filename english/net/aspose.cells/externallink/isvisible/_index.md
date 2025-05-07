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
// Called: if (workbook.Worksheets.ExternalLinks[i].IsVisible)
[Test]
        public void Property_IsVisible()
        {
            //test.UnFreezePanes001();
            Workbook workbook = new Workbook(Constants.sourcePath + "CELLSNET47566.xlsx");
            int count = 0;
            for (int i = 0; i < workbook.Worksheets.ExternalLinks.Count; i++)
            {
                if (workbook.Worksheets.ExternalLinks[i].IsVisible)
                {
                    count++;
                }
            }
            Assert.AreEqual(8, count);
        }
```

### See Also

* class [ExternalLink](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


