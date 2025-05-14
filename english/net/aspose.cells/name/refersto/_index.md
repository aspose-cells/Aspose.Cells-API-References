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
// Called: Assert.AreEqual("=工作表1!$C:$D", book.Worksheets.Names[1].RefersTo);
public void Name_Property_RefersTo()
{
    Workbook book = new Workbook(Constants.sourcePath + "example.ods");
    Assert.AreEqual("=工作表1!$6:$8", book.Worksheets.Names[0].RefersTo);
    Assert.AreEqual("=工作表1!$C:$D", book.Worksheets.Names[1].RefersTo);
}
```

### See Also

* class [Name](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


