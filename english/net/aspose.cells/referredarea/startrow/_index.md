---
title: ReferredArea.StartRow
second_title: Aspose.Cells for .NET API Reference
description: ReferredArea property. The start row of the area
type: docs
url: /net/aspose.cells/referredarea/startrow/
---
## ReferredArea.StartRow property

The start row of the area.

```csharp
public int StartRow { get; }
```

### Examples

```csharp
// Called: stringBuilder.Append(CellsHelper.CellIndexToName(area.StartRow, area.StartColumn));
[Test]
        public void Property_StartRow()
        {
             Workbook workbook = new Workbook();
             Cells cells = workbook.Worksheets[0].Cells;
             cells[&quot;A1&quot;].Formula = &quot;= B1 + SUM(B1:B10) + [Book1.xls]Sheet1!A1&quot;;
              ReferredAreaCollection areas = cells[&quot;A1&quot;].GetPrecedents();
             for (int i = 0; i &lt; areas.Count; i++)
             {
                 ReferredArea area = areas[i];
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
                    switch (i)
                    {
                        case 0:
                            Assert.AreEqual(stringBuilder.ToString(), &quot;Sheet1!B1&quot;);
                            break;
                        case 1:
                            Assert.AreEqual(stringBuilder.ToString(), &quot;Sheet1!B1:B10&quot;);
                            break;
                        case 2:
                            Assert.AreEqual(stringBuilder.ToString().ToUpper(), &quot;[Book1.xls]Sheet1!A1&quot;.ToUpper());
                            break;
                    }
                   
                 }
                 workbook.Save(Constants.destPath + &quot;Test217025.xls&quot;);
        }
```

### See Also

* class [ReferredArea](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


