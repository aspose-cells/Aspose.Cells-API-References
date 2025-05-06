---
title: Range.PutValue
second_title: Aspose.Cells for .NET API Reference
description: Range method. Puts a value into the range if appropriate the value will be converted to other data type and cells number format will be reset
type: docs
url: /net/aspose.cells/range/putvalue/
---
## Range.PutValue method

Puts a value into the range, if appropriate the value will be converted to other data type and cell's number format will be reset.

```csharp
public void PutValue(string stringValue, bool isConverted, bool setStyle)
```

| Parameter | Type | Description |
| --- | --- | --- |
| stringValue | String | Input value |
| isConverted | Boolean | True: converted to other data type if appropriate. |
| setStyle | Boolean | True: set the number format to cell's style when converting to other data type |

### Examples

```csharp
// Called: range.PutValue(&amp;quot;right orange&amp;quot;, false, false);
[Test]
        public void Method_Boolean_()
        {
            var workbook = new Workbook();
            workbook.Settings.UpdateAdjacentCellsBorder = true;
            var worksheet = workbook.Worksheets[0];

            var range = worksheet.Cells.CreateRange(1, 1, 6, 6);
            var style = worksheet.Workbook.CreateStyle();
            var flag = new StyleFlag();

            ApplyColorBorder(style, BorderType.BottomBorder, &quot;blue&quot;);
            ApplyStyleBorder(style, BorderType.BottomBorder, CellBorderType.Thick);
            flag.BottomBorder = true;

            ApplyColorBorder(style, BorderType.LeftBorder, &quot;blue&quot;);
            ApplyStyleBorder(style, BorderType.LeftBorder, CellBorderType.Thick);
            flag.LeftBorder = true;

            ApplyColorBorder(style, BorderType.RightBorder, &quot;blue&quot;);
            ApplyStyleBorder(style, BorderType.RightBorder, CellBorderType.Thick);
            flag.RightBorder = true;

            ApplyColorBorder(style, BorderType.TopBorder, &quot;blue&quot;);
            ApplyStyleBorder(style, BorderType.TopBorder, CellBorderType.Thick);
            flag.TopBorder = true;
            range.ApplyStyle(style, flag);
            //everything should be blue at this moment

            //set left border DOESNT WORK
            range = worksheet.Cells.CreateRange(2, 2, 1, 1);
            range.PutValue(&quot;left border&quot;, false, false);
            style = worksheet.Workbook.CreateStyle();
            flag = new StyleFlag();
            ApplyColorBorder(style, BorderType.LeftBorder, &quot;green&quot;);
            ApplyStyleBorder(style, BorderType.LeftBorder, CellBorderType.Thick);
            flag.LeftBorder = true;
            range.ApplyStyle(style, flag);
           AssertHelper.AreEqual(worksheet.Cells[2,2].GetStyle().Borders[BorderType.LeftBorder].Color, Color.Green);

            //set right border DOESNT WORK
            range = worksheet.Cells.CreateRange(2, 3, 1, 1);
            range.PutValue(&quot;right orange&quot;, false, false);
            style = worksheet.Workbook.CreateStyle();
            flag = new StyleFlag();
            ApplyColorBorder(style, BorderType.RightBorder, &quot;orange&quot;);
            ApplyStyleBorder(style, BorderType.RightBorder, CellBorderType.Thick);
            flag.RightBorder = true;
            range.ApplyStyle(style, flag);
           AssertHelper.AreEqual(worksheet.Cells[2, 3].GetStyle().Borders[BorderType.RightBorder].Color, Color.Orange);


            //set top border DOESNT WORK
            range = worksheet.Cells.CreateRange(3, 2, 1, 1);
            range.PutValue(&quot;top pink &quot;, false, false);
            style = worksheet.Workbook.CreateStyle();
            flag = new StyleFlag();
            ApplyColorBorder(style, BorderType.TopBorder, &quot;pink&quot;);
            ApplyStyleBorder(style, BorderType.TopBorder, CellBorderType.Thick);
            flag.TopBorder = true;
            range.ApplyStyle(style, flag);
           AssertHelper.AreEqual(worksheet.Cells[3, 2].GetStyle().Borders[BorderType.TopBorder].Color, Color.Pink);


            //set left border DOESNT WORK
            range = worksheet.Cells.CreateRange(3, 3, 1, 1);
            range.PutValue(&quot;bottom brown&quot;, false, false);
            style = worksheet.Workbook.CreateStyle();
            flag = new StyleFlag();
            ApplyColorBorder(style, BorderType.BottomBorder, &quot;brown&quot;);
            ApplyStyleBorder(style, BorderType.BottomBorder, CellBorderType.Thick);
            flag.BottomBorder = true;
            range.ApplyStyle(style, flag);
           AssertHelper.AreEqual(worksheet.Cells[3, 3].GetStyle().Borders[BorderType.BottomBorder].Color, Color.Brown);


            //set left border WORKS only when it&apos;s on the last row
            range = worksheet.Cells.CreateRange(6, 1, 1, 1);
            range.PutValue(&quot;left border&quot;, false, false);
            style = worksheet.Workbook.CreateStyle();
            flag = new StyleFlag();
            ApplyColorBorder(style, BorderType.LeftBorder, &quot;green&quot;);
            ApplyStyleBorder(style, BorderType.LeftBorder, CellBorderType.Thick);
            flag.LeftBorder = true;
            range.ApplyStyle(style, flag);
           AssertHelper.AreEqual(worksheet.Cells[6, 1].GetStyle().Borders[BorderType.LeftBorder].Color, Color.Green);


            //set right border DOESNT WORK
            range = worksheet.Cells.CreateRange(6, 2, 1, 1);
            range.PutValue(&quot;right orange&quot;, false, false);
            style = worksheet.Workbook.CreateStyle();
            flag = new StyleFlag();
            ApplyColorBorder(style, BorderType.RightBorder, &quot;orange&quot;);
            ApplyStyleBorder(style, BorderType.RightBorder, CellBorderType.Thick);
            flag.RightBorder = true;
            range.ApplyStyle(style, flag);
           AssertHelper.AreEqual(worksheet.Cells[6, 2].GetStyle().Borders[BorderType.RightBorder].Color, Color.Orange);


            //set top border DOESNT WORK
            range = worksheet.Cells.CreateRange(6, 3, 1, 1);
            range.PutValue(&quot;top pink &quot;, false, false);
            style = worksheet.Workbook.CreateStyle();
            flag = new StyleFlag();
            ApplyColorBorder(style, BorderType.TopBorder, &quot;pink&quot;);
            ApplyStyleBorder(style, BorderType.TopBorder, CellBorderType.Thick);
            flag.TopBorder = true;
            range.ApplyStyle(style, flag);
           AssertHelper.AreEqual(worksheet.Cells[6, 3].GetStyle().Borders[BorderType.TopBorder].Color, Color.Pink);


            //set bottom border WORK only when it&apos;s on the last row
            range = worksheet.Cells.CreateRange(6, 4, 1, 1);
            range.PutValue(&quot;bottom brown&quot;, false, false);
            style = worksheet.Workbook.CreateStyle();
            flag = new StyleFlag();
            ApplyColorBorder(style, BorderType.BottomBorder, &quot;brown&quot;);
            ApplyStyleBorder(style, BorderType.BottomBorder, CellBorderType.Thick);
            flag.BottomBorder = true;
            range.ApplyStyle(style, flag);
           AssertHelper.AreEqual(worksheet.Cells[6, 4].GetStyle().Borders[BorderType.BottomBorder].Color, Color.Brown);


            worksheet.AutoFitColumns(1, 1, 6, 6);
            workbook.Save(Constants.destPath + &quot;CellsNet45416.xlsx&quot;);
        }
```

### See Also

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


