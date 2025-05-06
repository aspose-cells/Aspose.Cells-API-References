---
title: ReferredArea.EndColumn
second_title: Aspose.Cells for .NET API Reference
description: ReferredArea property. The end column of the area
type: docs
url: /net/aspose.cells/referredarea/endcolumn/
---
## ReferredArea.EndColumn property

The end column of the area.

```csharp
public int EndColumn { get; }
```

### Examples

```csharp
// Called: stringBuilder.Append(CellsHelper.CellIndexToName(area.EndRow, area.EndColumn));
[Test]
        public void Property_EndColumn()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;Formula/CellsNet42731.xlsx&quot;);
            ReferredAreaCollection ret = workbook.Worksheets[0].Cells[&quot;E1&quot;].GetPrecedents();
            if (ret != null)
            {
                for (int m = 0; m &lt; ret.Count; m++)
                {
                    ReferredArea area = ret[m];
                    StringBuilder stringBuilder = new StringBuilder();
                    if (area.IsExternalLink)
                    {
                        stringBuilder.Append(&quot;[&quot;);
                        stringBuilder.Append(area.ExternalFileName);
                        stringBuilder.Append(&quot;]&quot;);
                    }
                    stringBuilder.Append(area.SheetName);
                    stringBuilder.Append(&quot;!&quot;);
                    stringBuilder.Append(CellsHelper.CellIndexToName(area.StartRow, area.StartColumn));
                    if (area.IsArea)
                    {
                        stringBuilder.Append(&quot;:&quot;);
                        stringBuilder.Append(CellsHelper.CellIndexToName(area.EndRow, area.EndColumn));
                    }
                    Assert.AreEqual(stringBuilder.ToString(), &quot;Sheet1!A2:C3&quot;);
                }
            }
        }
```

### See Also

* class [ReferredArea](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


