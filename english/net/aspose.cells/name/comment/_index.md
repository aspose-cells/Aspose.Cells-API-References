---
title: Name.Comment
second_title: Aspose.Cells for .NET API Reference
description: Name property. Gets and sets the comment of the name. Only applies for Excel 2007 or higher versions
type: docs
url: /net/aspose.cells/name/comment/
---
## Name.Comment property

Gets and sets the comment of the name. Only applies for Excel 2007 or higher versions.

```csharp
public string Comment { get; set; }
```

### Examples

```csharp
// Called: Assert.AreEqual(name.Comment, "abc");
public void Name_Property_Comment()
{
    Workbook workbook = new Workbook(Constants.sourcePath + "NameComment.xlsx");
    Name name = workbook.Worksheets.Names[0];
    Assert.AreEqual(name.Comment, "abc");
    workbook.Save(Constants.destPath + "example.xls");
    workbook = new Workbook(Constants.destPath + "example.xls");
    name = workbook.Worksheets.Names[0];
    Assert.AreEqual(name.Comment, "abc");
}
```

### See Also

* class [Name](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


