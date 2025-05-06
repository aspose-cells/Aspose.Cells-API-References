---
title: ValidationCollection.Item
second_title: Aspose.Cells for .NET API Reference
description: ValidationCollection property. Gets the Validation element at the specified index
type: docs
url: /net/aspose.cells/validationcollection/item/
---
## ValidationCollection indexer

Gets the [`Validation`](../../validation/) element at the specified index.

```csharp
public Validation this[int index] { get; }
```

| Parameter | Description |
| --- | --- |
| index | The zero based index of the element. |

### Return Value

The element at the specified index.

### Examples

```csharp
// Called: Assert.AreEqual(&amp;quot;A,B,C&amp;quot;, workbook.Worksheets[0].Validations[0].Formula1);
[Test]
        public void Property_Int32_()
        {

            Workbook workbook = new Workbook(Constants.sourcePath + &quot;CELLSNET49077.xlsx&quot;);
            Assert.AreEqual(&quot;A,B,C&quot;, workbook.Worksheets[0].Validations[0].Formula1);
            Assert.AreEqual(&quot;=A5&quot;, workbook.Worksheets[0].Validations[1].Formula1);
            workbook.Save(Constants.destPath + &quot;CELLSNET49077.ods&quot;);
            workbook = new Workbook(Constants.destPath + &quot;CELLSNET49077.ods&quot;);
            Assert.AreEqual(&quot;A,B,C&quot;, workbook.Worksheets[0].Validations[0].Formula1);
            Assert.AreEqual(&quot;=A5&quot;, workbook.Worksheets[0].Validations[1].Formula1);
            Assert.IsTrue(ManualFileUtil.ManualCheckStringInZip(Constants.destPath + &quot;CELLSNET49077.ods&quot;, &quot;content.xml&quot;, new string[] { &quot;of:is-true-formula([.A5])&quot;, &quot;of:cell-content-is-in-list(&amp;quot;A&amp;quot;;&amp;quot;B&amp;quot;;&amp;quot;C&amp;quot;)&quot; }, true));
           

        }
```

### See Also

* class [Validation](../../validation/)
* class [ValidationCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


