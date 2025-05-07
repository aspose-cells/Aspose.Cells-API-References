---
title: FormatConditionCollection.Item
second_title: Aspose.Cells for .NET API Reference
description: FormatConditionCollection property. Gets the formatting condition by index
type: docs
url: /net/aspose.cells/formatconditioncollection/item/
---
## FormatConditionCollection indexer

Gets the formatting condition by index.

```csharp
public FormatCondition this[int index] { get; }
```

| Parameter | Description |
| --- | --- |
| index | the index of the formatting condition to return. |

### Return Value

the formatting condition

### Examples

```csharp
// Called: Assert.AreEqual("=4", fcs[0].Formula1);
[Test]
        public void Property_Int32_()
        {
            Workbook wb = new Workbook(Constants.sourcePath + "CELLSNET53803.xlsx");
            wb = Util.ReSave(wb, SaveFormat.Xlsb);//.Save(Constants.destPath + "CELLSNET53803.xlsb");
            //wb = new Workbook(Constants.destPath + "CELLSNET53803.xlsb");
            wb = Util.ReSave(wb, SaveFormat.Xlsx);//.Save(Constants.destPath + "CELLSNET53803.xlsx");
            //wb = new Workbook(Constants.destPath + "CELLSNET53803.xlsx");
            FormatConditionCollection fcs =  wb.Worksheets[0].ConditionalFormattings[0];
            Assert.AreEqual(OperatorType.NotBetween, fcs[0].Operator);
            Assert.AreEqual("=4", fcs[0].Formula1);
        }
```

### See Also

* class [FormatCondition](../../formatcondition/)
* class [FormatConditionCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


