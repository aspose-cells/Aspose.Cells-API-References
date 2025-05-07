---
title: Font.Charset
second_title: Aspose.Cells for .NET API Reference
description: Font property. Represent the character set
type: docs
url: /net/aspose.cells/font/charset/
---
## Font.Charset property

Represent the character set.

```csharp
public int Charset { get; set; }
```

### Examples

```csharp
// Called: Assert.AreEqual(0x80, workbook.DefaultStyle.Font.Charset);
[Test]
        public void Property_Charset()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + "CellsJava45084.xls");

           // Assert.AreEqual("游ゴシック", workbook.DefaultStyle.Font.Name);
            Assert.AreEqual(0x80, workbook.DefaultStyle.Font.Charset);
            workbook.Save(Constants.destPath + "CellsJava45084.xls");
            workbook = new Workbook(Constants.destPath + "CellsJava45084.xls");

            //Assert.AreEqual("游ゴシック", workbook.DefaultStyle.Font.Name);
            Assert.AreEqual(0x80, workbook.DefaultStyle.Font.Charset);
        }
```

### See Also

* class [Font](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


