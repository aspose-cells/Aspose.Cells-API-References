---
title: Name.RefersTo
second_title: Aspose.Cells for .NET API Reference
description: Name property. Returns or sets the formula that the name is defined to refer to beginning with an equal sign
type: docs
url: /net/aspose.cells/name/refersto/
---
## Name.RefersTo property

Returns or sets the formula that the name is defined to refer to, beginning with an equal sign.

```csharp
public string RefersTo { get; set; }
```

### Examples

```csharp
// Called: n2.RefersTo = &amp;quot;=Sheet1!H10:I15&amp;quot;;
[Test]
        public void Property_RefersTo()
        {
            Workbook wb = new Workbook();
            NameCollection nc = wb.Worksheets.Names;
            Name n1 = nc[nc.Add(&quot;TestName1&quot;)];
            n1.RefersTo = &quot;=Sheet1!F10:G15&quot;;

            Name n2 = nc[nc.Add(&quot;TestName2&quot;)];
            n2.RefersTo = &quot;=Sheet1!H10:I15&quot;;

            Name n3 = nc[nc.Add(&quot;Sheet1!TestName1&quot;)];
            n2.RefersTo = &quot;=Sheet1!F20:G25&quot;;

            Name n4 = nc[nc.Add(&quot;Sheet1!TestName2&quot;)];
            n2.RefersTo = &quot;=Sheet1!H20:I25&quot;;

            wb.Worksheets.Add();
            wb.Worksheets[1].Cells[0, 0].Formula = &quot;=SUM(TestName2)&quot;;
            wb.Worksheets[0].Cells[0, 1].Formula = &quot;=SUM(Sheet1!TestName2)&quot;;
            Assert.IsFalse(n1.IsReferred, &quot;TestName1.IsReferred&quot;);
            Assert.IsFalse(n3.IsReferred, &quot;Sheet1!TestName1.IsReferred&quot;);
            Assert.IsTrue(n2.IsReferred, &quot;TestName2.IsReferred&quot;);
            Assert.IsTrue(n4.IsReferred, &quot;Sheet1!TestName2.IsReferred&quot;);
        }
```

### See Also

* class [Name](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


