---
title: ListObject.UpdateColumnName
second_title: Aspose.Cells for .NET API Reference
description: ListObject method. Updates all list columns name from the worksheet
type: docs
url: /net/aspose.cells.tables/listobject/updatecolumnname/
---
## ListObject.UpdateColumnName method

Updates all list columns' name from the worksheet.

```csharp
public void UpdateColumnName()
```

### Remarks

The value of the cells in the header row of the table must be same as the name of the ListColumn; Cell.PutValue do not auto modify the name of the ListColumn for performance.

### Examples

```csharp
// Called: innerRange.UpdateColumnName();
[Test]
        public void Method_UpdateColumnName()
        {
            Workbook wb = new Workbook();
            Worksheet ws = wb.Worksheets[0];

            var outerRange = ws.Cells.CreateRange(0, 0, 10, 10);
            outerRange.SetOutlineBorder(Aspose.Cells.BorderType.TopBorder, CellBorderType.Thick, Color.Blue);
            outerRange.SetOutlineBorder(Aspose.Cells.BorderType.BottomBorder, CellBorderType.Thick, Color.Blue);
            outerRange.SetOutlineBorder(Aspose.Cells.BorderType.LeftBorder, CellBorderType.Thick, Color.Blue);
            outerRange.SetOutlineBorder(Aspose.Cells.BorderType.RightBorder, CellBorderType.Thick, Color.Blue);

            var innerRange = ws.ListObjects[ws.ListObjects.Add(3, 3, 6, 6, true)];
            for (int r = 0; r &lt; 3; r++)
            {
                for (int c = 0; c &lt; 3; c++)
                {
                    if (c &gt; 0)
                        ws.Cells[innerRange.StartRow + r, innerRange.StartColumn + c].PutValue(r + c);
                    else
                        ws.Cells[innerRange.StartRow + r, innerRange.StartColumn + c].PutValue(string.Empty);
                }
            }
            innerRange.TableStyleType = TableStyleType.TableStyleDark4;
            innerRange.UpdateColumnName();
            var myDir = @&quot;MyDirHere&quot;;
            wb.Save(Constants.destPath + &quot;CELLSNET46128.xlsx&quot;);
            wb = new Workbook(Constants.destPath + &quot;CELLSNET46128.xlsx&quot;);
            Assert.AreEqual(&quot;Column1&quot;,wb.Worksheets[0].Cells[&quot;D4&quot;].StringValue);
        }
```

### See Also

* class [ListObject](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


