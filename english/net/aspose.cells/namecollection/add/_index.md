---
title: NameCollection.Add
second_title: Aspose.Cells for .NET API Reference
description: NameCollection method. Defines a new name
type: docs
url: /net/aspose.cells/namecollection/add/
---
## NameCollection.Add method

Defines a new name.

```csharp
public int Add(string text)
```

| Parameter | Type | Description |
| --- | --- | --- |
| text | String | The text to use as the name. |

### Return Value

[`Name`](../../name/) object index.

### Remarks

Name cannot include spaces and cannot look like cell references.

### Examples

```csharp
// Called: Name n2 = nc[nc.Add(&amp;quot;TestName2&amp;quot;)];
[Test]
        public void Method_String_()
        {
            Workbook wb = new Workbook();
            Cells cells = wb.Worksheets.Add(&quot;Sheet2&quot;).Cells;
            NameCollection nc = wb.Worksheets.Names;
            Name n1 = nc[nc.Add(&quot;TestName1&quot;)];
            n1.RefersTo = &quot;=Sheet1!F10&quot;;

            Name n2 = nc[nc.Add(&quot;TestName2&quot;)];
            n2.RefersTo = &quot;=Sheet2!F10&quot;;
            cells[&quot;F10&quot;].PutValue(1);
            Cell cell = cells[0, 0];
            cell.Formula = &quot;=TestName2&quot;;
            wb.CalculateFormula(false);
            Assert.AreEqual(1, cell.IntValue, &quot;Before delete sheet, =TestName2&quot;);
            wb.Worksheets.RemoveAt(0);
            wb.CalculateFormula(false);
            Assert.AreEqual(1, cell.IntValue, &quot;Before delete sheet, =TestName2&quot;);
        }
```

### See Also

* class [NameCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


