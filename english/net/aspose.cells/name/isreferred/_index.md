---
title: Name.IsReferred
second_title: Aspose.Cells for .NET API Reference
description: Name property. Indicates whether this name is referred by other formulas
type: docs
url: /net/aspose.cells/name/isreferred/
---
## Name.IsReferred property

Indicates whether this name is referred by other formulas.

```csharp
public bool IsReferred { get; }
```

### Examples

```csharp
// Called: Assert.IsTrue(n2.IsReferred, "TestName2.IsReferred");
public void Name_Property_IsReferred()
{
    Workbook wb = new Workbook();
    NameCollection nc = wb.Worksheets.Names;
    Name n1 = nc[nc.Add("TestName1")];
    n1.RefersTo = "=Sheet1!F10:G15";

    Name n2 = nc[nc.Add("TestName2")];
    n2.RefersTo = "=Sheet1!H10:I15";

    Name n3 = nc[nc.Add("Sheet1!TestName1")];
    n2.RefersTo = "=Sheet1!F20:G25";

    Name n4 = nc[nc.Add("Sheet1!TestName2")];
    n2.RefersTo = "=Sheet1!H20:I25";

    wb.Worksheets.Add();
    wb.Worksheets[1].Cells[0, 0].Formula = "=SUM(TestName2)";
    wb.Worksheets[0].Cells[0, 1].Formula = "=SUM(Sheet1!TestName2)";
    Assert.IsFalse(n1.IsReferred, "TestName1.IsReferred");
    Assert.IsFalse(n3.IsReferred, "Sheet1!TestName1.IsReferred");
    Assert.IsTrue(n2.IsReferred, "TestName2.IsReferred");
    Assert.IsTrue(n4.IsReferred, "Sheet1!TestName2.IsReferred");
}
```

### See Also

* class [Name](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


