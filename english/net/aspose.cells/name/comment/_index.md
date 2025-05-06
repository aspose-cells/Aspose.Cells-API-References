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
// Called: Assert.AreEqual(name.Comment, &amp;quot;abc&amp;quot;);
[Test]
        public void Property_Comment()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;NameComment.xlsx&quot;);
            Name name = workbook.Worksheets.Names[0];
            Assert.AreEqual(name.Comment, &quot;abc&quot;);
            workbook.Save(Constants.destPath + &quot;Test_203493.xls&quot;);
            workbook = new Workbook(Constants.destPath + &quot;Test_203493.xls&quot;);
            name = workbook.Worksheets.Names[0];
            Assert.AreEqual(name.Comment, &quot;abc&quot;);
        }
```

### See Also

* class [Name](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


