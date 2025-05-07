---
title: ConditionalFormattingIconCollection.Item
second_title: Aspose.Cells for .NET API Reference
description: ConditionalFormattingIconCollection property. Gets the ConditionalFormattingIcon element at the specified index
type: docs
url: /net/aspose.cells/conditionalformattingiconcollection/item/
---
## ConditionalFormattingIconCollection indexer

Gets the ConditionalFormattingIcon element at the specified index.

```csharp
public ConditionalFormattingIcon this[int index] { get; }
```

| Parameter | Description |
| --- | --- |
| index | The zero based index of the element. |

### Return Value

The element at the specified index.

### Examples

```csharp
// Called: Assert.AreEqual(2, iconCollection[2].Index);
[Test]
        public void Property_Int32_()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + "ConditionalFormattings/TestConditionalIcon1.xlsx");
            Worksheet sheet1 = workbook.Worksheets[0];
            ConditionalFormattingResult r = sheet1.Cells["C2"].GetConditionalFormattingResult();
            Assert.AreEqual(r.ConditionalFormattingIcon.Index, 2);
            r = sheet1.Cells["D2"].GetConditionalFormattingResult();
            Assert.AreEqual(r.ConditionalFormattingIcon.Index, 1);
            r = sheet1.Cells["E2"].GetConditionalFormattingResult();
            Assert.AreEqual(r.ConditionalFormattingIcon.Index, 0);
            FormatConditionCollection conditionCollection = sheet1.ConditionalFormattings[0];
            FormatCondition condition = conditionCollection[0];
        
            ConditionalFormattingIconCollection iconCollection = condition.IconSet.CfIcons;
            Assert.AreEqual(0, iconCollection[0].Index);
            Assert.AreEqual(1, iconCollection[1].Index);
            Assert.AreEqual(2, iconCollection[2].Index);

        }
```

### See Also

* class [ConditionalFormattingIcon](../../conditionalformattingicon/)
* class [ConditionalFormattingIconCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


