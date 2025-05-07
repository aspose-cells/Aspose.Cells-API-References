---
title: WriteProtection.Author
second_title: Aspose.Cells for .NET API Reference
description: WriteProtection property. Gets and sets the author
type: docs
url: /net/aspose.cells/writeprotection/author/
---
## WriteProtection.Author property

Gets and sets the author.

```csharp
public string Author { get; set; }
```

### Examples

```csharp
// Called: workbook.Settings.WriteProtection.Author = "abc";
[Test]
        public void Property_Author()
        {

            Workbook workbook = new Workbook();

            workbook.Settings.WriteProtection.Password = "test";
            workbook.Settings.WriteProtection.Author = "abc";
            workbook.Save(Constants.destPath + "WriteProtection1.xlsx");
            workbook = new Workbook(Constants.destPath + "WriteProtection1.xlsx");
            Assert.AreEqual("abc", workbook.Settings.WriteProtection.Author);

        }
```

### See Also

* class [WriteProtection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


