---
title: Worksheet.UnFreezePanes
second_title: Aspose.Cells for .NET API Reference
description: Worksheet method. Unfreezes panes in the worksheet
type: docs
url: /net/aspose.cells/worksheet/unfreezepanes/
---
## Worksheet.UnFreezePanes method

Unfreezes panes in the worksheet.

```csharp
public void UnFreezePanes()
```

### Examples

```csharp
// Called: workbook.Worksheets[0].UnFreezePanes();
private void Method_UnFreezePanes(PaneStateType type)
        {
            Workbook workbook = new Workbook();
            int row, column, rows, columns;
            switch (type)
            {
                case PaneStateType.Frozen:
                    workbook.Worksheets[0].FreezePanes(&quot;C3&quot;, 2, 2);
                    workbook.Worksheets[0].GetFreezedPanes(out row, out column, out rows, out columns);
                    Assert.AreEqual(row, 2);
                    Assert.AreEqual(column, 2);
                    Assert.AreEqual(rows, 2);
                    Assert.AreEqual(columns, 2);
                    break;
                case PaneStateType.FrozenSplit:
                    workbook.Worksheets[0].ActiveCell = &quot;C3&quot;;
                    workbook.Worksheets[0].Split();
                    workbook.Worksheets[0].FreezePanes(&quot;C3&quot;, 2, 2);
                    workbook.Worksheets[0].GetFreezedPanes(out row, out column, out rows, out columns);
                    Assert.AreEqual(row, 2);
                    Assert.AreEqual(column, 2);
                    Assert.AreEqual(rows, 2);
                    Assert.AreEqual(columns, 2);
                    break;
                case PaneStateType.Split:
                    workbook.Worksheets[0].ActiveCell = &quot;C3&quot;;
                    workbook.Worksheets[0].Split();
                    break;
                case PaneStateType.Normal:
                    break;
                default:
                    break;
            }
          
          
         
            Assert.AreEqual(workbook.Worksheets[0].PaneState, type);
            workbook.Save(Constants.destPath + &quot;UnFreezePanes001.xls&quot;);
            workbook = new Workbook(Constants.destPath + &quot;UnFreezePanes001.xls&quot;);
            Assert.AreEqual(workbook.Worksheets[0].PaneState, type);
            workbook.Save(Constants.destPath + &quot;UnFreezePanes001.xlsx&quot;);
            workbook = new Workbook(Constants.destPath + &quot;UnFreezePanes001.xlsx&quot;);
            Assert.AreEqual(workbook.Worksheets[0].PaneState, type);
            workbook.Save(Constants.destPath + &quot;UnFreezePanes001.xlsb&quot;);
            workbook = new Workbook(Constants.destPath + &quot;UnFreezePanes001.xlsb&quot;);
            Assert.AreEqual(workbook.Worksheets[0].PaneState, type);

            //workbook.Save(Constants.destPath + &quot;UnFreezePanes001.ods&quot;);
            //workbook = new Workbook(Constants.destPath + &quot;UnFreezePanes001.ods&quot;);
            //Assert.AreEqual(workbook.Worksheets[0].PaneState, type);
            switch (type)
            {
                case PaneStateType.Frozen:
                    workbook.Worksheets[0].UnFreezePanes();
                    Assert.AreEqual(workbook.Worksheets[0].PaneState, PaneStateType.Normal);
                    break;
                case PaneStateType.FrozenSplit:
                    workbook.Worksheets[0].UnFreezePanes();
                    Assert.AreEqual(workbook.Worksheets[0].PaneState, PaneStateType.Split);
                    break;
            
                case PaneStateType.Split:
                    workbook.Worksheets[0].RemoveSplit();
                    Assert.AreEqual(workbook.Worksheets[0].PaneState, PaneStateType.Normal);
                    break;
            }
        
        }
```

### See Also

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


