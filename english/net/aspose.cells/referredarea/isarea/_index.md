---
title: ReferredArea.IsArea
second_title: Aspose.Cells for .NET API Reference
description: ReferredArea property. Indicates whether this is an area
type: docs
url: /net/aspose.cells/referredarea/isarea/
---
## ReferredArea.IsArea property

Indicates whether this is an area.

```csharp
public bool IsArea { get; }
```

### Remarks

If this is not an area, only StartRow and StartColumn effect.

### Examples

```csharp
// Called: if (area.IsArea)
[Test]
        public void Property_IsArea()
        {
             Workbook workbook = new Workbook();
             Cells cells = workbook.Worksheets[0].Cells;
             cells["A1"].Formula = "= B1 + SUM(B1:B10) + [Book1.xls]Sheet1!A1";
              ReferredAreaCollection areas = cells["A1"].GetPrecedents();
             for (int i = 0; i < areas.Count; i++)
             {
                 ReferredArea area = areas[i];
                  StringBuilder stringBuilder = new StringBuilder();
                  if (area.IsExternalLink)
                  {
                      stringBuilder.Append("[");
                       stringBuilder.Append(area.ExternalFileName);
                       stringBuilder.Append("]");
                   }
                   stringBuilder.Append(area.SheetName);
                   stringBuilder.Append("!");
                   stringBuilder.Append(CellsHelper.CellIndexToName(area.StartRow, area.StartColumn));
                   if (area.IsArea)
                    {
                        stringBuilder.Append(":");
                        stringBuilder.Append(CellsHelper.CellIndexToName(area.EndRow, area.EndColumn));
                    }
                    switch (i)
                    {
                        case 0:
                            Assert.AreEqual(stringBuilder.ToString(), "Sheet1!B1");
                            break;
                        case 1:
                            Assert.AreEqual(stringBuilder.ToString(), "Sheet1!B1:B10");
                            break;
                        case 2:
                            Assert.AreEqual(stringBuilder.ToString().ToUpper(), "[Book1.xls]Sheet1!A1".ToUpper());
                            break;
                    }
                   
                 }
                 workbook.Save(Constants.destPath + "Test217025.xls");
        }
```

### See Also

* class [ReferredArea](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


