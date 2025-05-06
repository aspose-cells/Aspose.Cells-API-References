---
title: Worksheet.SetVisible
second_title: Aspose.Cells for .NET API Reference
description: Worksheet method. Sets the visible options
type: docs
url: /net/aspose.cells/worksheet/setvisible/
---
## Worksheet.SetVisible method

Sets the visible options.

```csharp
public void SetVisible(bool isVisible, bool ignoreError)
```

| Parameter | Type | Description |
| --- | --- | --- |
| isVisible | Boolean | Whether the worksheet is visible |
| ignoreError | Boolean | Whether to ignore error if this option is not valid. |

### Examples

```csharp
// Called: aWkAsp.Worksheets[2].SetVisible(false, true);
[Test]
        public void Method_Boolean_()
        {
            Aspose.Cells.Workbook aWkAsp = new Aspose.Cells.Workbook(Constants.sourcePath + &quot;CELLSNET45175.xls&quot;);

            aWkAsp.Worksheets[1].SetVisible(false, true);
            aWkAsp.Worksheets[2].SetVisible(false, true);

            Cells cells = aWkAsp.Worksheets[0].Cells;
            int maxCol = cells.MaxColumn;
            for (int iRow = cells.MaxRow; iRow &gt; 1; iRow--)
            {
                Cell cell = cells.CheckCell(iRow, 0);
                if (cell != null &amp;&amp; cell.Value != null &amp;&amp; cell.Value.ToString().ToUpper() == &quot;S&quot;)
                {
                    cells.DeleteRange(iRow, 0, iRow, maxCol, ShiftType.Up);
                }
            }
            string printArea = aWkAsp.Worksheets[0].PageSetup.PrintArea;
            Assert.IsTrue(string.IsNullOrEmpty(printArea));
            Util.ReSave(aWkAsp, SaveFormat.Excel97To2003);
            Util.SaveAsBuffer(aWkAsp, SaveFormat.Pdf);
            //aWkAsp.Save(Constants.destPath + &quot;CELLSNET45175.xls&quot;);
            //aWkAsp.Save(Constants.destPath + &quot;CELLSNET45175.pdf&quot;, Aspose.Cells.SaveFormat.Pdf);
        }
```

### See Also

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


