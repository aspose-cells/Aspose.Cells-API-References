---
title: Name.Text
second_title: Aspose.Cells for .NET API Reference
description: Name property. Gets the name text of the object
type: docs
url: /net/aspose.cells/name/text/
---
## Name.Text property

Gets the name text of the object.

```csharp
public string Text { get; set; }
```

### Examples

```csharp
// Called: Assert.AreEqual("list2", names[0].Text);
public void Name_Property_Text()
{
    Workbook workbook = new Workbook(Constants.sourcePath + "example.ods");
    NameCollection names = workbook.Worksheets.Names;
    Assert.AreEqual(3, names.Count);
    Assert.AreEqual(1, names[0].SheetIndex);
    Assert.AreEqual("list2", names[0].Text);
    workbook.Save(Constants.destPath + "example.ods");
    workbook = new Workbook(Constants.sourcePath + "example.ods");
    names = workbook.Worksheets.Names;
    Assert.AreEqual(3, names.Count);
    Assert.AreEqual(1, names[0].SheetIndex);
    Assert.AreEqual("list2", names[0].Text);
}
```

### See Also

* class [Name](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


