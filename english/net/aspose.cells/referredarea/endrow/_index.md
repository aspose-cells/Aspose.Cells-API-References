---
title: ReferredArea.EndRow
second_title: Aspose.Cells for .NET API Reference
description: ReferredArea property. The end row of the area
type: docs
url: /net/aspose.cells/referredarea/endrow/
---
## ReferredArea.EndRow property

The end row of the area.

```csharp
public int EndRow { get; }
```

### Examples

```csharp
// Called: stringBuilder.Append(CellsHelper.CellIndexToName(area.EndRow, area.EndColumn));
public void ReferredArea_Property_EndRow()
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
         workbook.Save(Constants.destPath + "example.xls");
}
```

### See Also

* class [ReferredArea](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


