---
title: ConditionalFormattingValueCollection.Item
second_title: Aspose.Cells for .NET API Reference
description: ConditionalFormattingValueCollection property. Get the CFValueObject element at the specified index
type: docs
url: /net/aspose.cells/conditionalformattingvaluecollection/item/
---
## ConditionalFormattingValueCollection indexer

Get the CFValueObject element at the specified index.

```csharp
public ConditionalFormattingValue this[int index] { get; }
```

| Parameter | Description |
| --- | --- |
| index | The zero based index of the element. |

### Return Value

The element at the specified index.

### Examples

```csharp
// Called: Assert.AreEqual(0, (int)icons[0].Value);
[Test]
        public void Property_Int32_()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;CellsNet51961.ods&quot;);
            workbook.Save(Constants.destPath + &quot;CellsNet51961.ods&quot;);
            workbook = new Workbook(Constants.destPath + &quot;CellsNet51961.ods&quot;);
            ConditionalFormattingValueCollection icons = workbook.Worksheets[0].ConditionalFormattings[0][0].IconSet.Cfvos;
            Assert.AreEqual(0, (int)icons[0].Value);
            Assert.AreEqual(&quot;abc&quot;, (string)icons[2].Value);

        }
```

### See Also

* class [ConditionalFormattingValue](../../conditionalformattingvalue/)
* class [ConditionalFormattingValueCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


