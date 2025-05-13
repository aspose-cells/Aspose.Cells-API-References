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
private void Worksheet_Method_UnFreezePanes(PaneStateType type)
        {
            Workbook workbook = new Workbook();
            int row, column, rows, columns;
            switch (type)
            {
                case PaneStateType.Frozen:
                    workbook.Worksheets[0].FreezePanes("C3", 2, 2);
                    workbook.Worksheets[0].GetFreezedPanes(out row, out column, out rows, out columns);
                    Assert.AreEqual(row, 2);
                    Assert.AreEqual(column, 2);
                    Assert.AreEqual(rows, 2);
                    Assert.AreEqual(columns, 2);
                    break;
                case PaneStateType.FrozenSplit:
                    workbook.Worksheets[0].ActiveCell = "C3";
                    workbook.Worksheets[0].Split();
                    workbook.Worksheets[0].FreezePanes("C3", 2, 2);
                    workbook.Worksheets[0].GetFreezedPanes(out row, out column, out rows, out columns);
                    Assert.AreEqual(row, 2);
                    Assert.AreEqual(column, 2);
                    Assert.AreEqual(rows, 2);
                    Assert.AreEqual(columns, 2);
                    break;
                case PaneStateType.Split:
                    workbook.Worksheets[0].ActiveCell = "C3";
                    workbook.Worksheets[0].Split();
                    break;
                case PaneStateType.Normal:
                    break;
                default:
                    break;
            }
          
          
         
            Assert.AreEqual(workbook.Worksheets[0].PaneState, type);
            workbook.Save(Constants.destPath + "example.xls");
            workbook = new Workbook(Constants.destPath + "example.xls");
            Assert.AreEqual(workbook.Worksheets[0].PaneState, type);
            workbook.Save(Constants.destPath + "example.xlsx");
            workbook = new Workbook(Constants.destPath + "example.xlsx");
            Assert.AreEqual(workbook.Worksheets[0].PaneState, type);
            workbook.Save(Constants.destPath + "example.xlsb");
            workbook = new Workbook(Constants.destPath + "example.xlsb");
            Assert.AreEqual(workbook.Worksheets[0].PaneState, type);

            //workbook.Save(Constants.destPath + "example.ods");
            //workbook = new Workbook(Constants.destPath + "example.ods");
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


