---
title: TxtSaveOptions.Encoding
second_title: Aspose.Cells for .NET API Reference
description: TxtSaveOptions property. Gets and sets the default encoding
type: docs
url: /net/aspose.cells/txtsaveoptions/encoding/
---
## TxtSaveOptions.Encoding property

Gets and sets the default encoding.

```csharp
public Encoding Encoding { get; set; }
```

### Examples

```csharp
// Called: wb.Save(ms, new TxtSaveOptions() { Encoding = Encoding.UTF8, });
[Test]
        public void Property_Encoding()
        {
            MemoryStream ms = new MemoryStream();
            byte[] data = Encoding.ASCII.GetBytes("abc,123");
            ms.Write(data, 0, data.Length);
            ms.Seek(0, SeekOrigin.Begin);
            Workbook wb = new Workbook(ms, new TxtLoadOptions() { Encoding = Encoding.ASCII, });
            Cells cells = wb.Worksheets[0].Cells;
            Assert.AreEqual("abc", cells[0, 0].Value, "A1.Value from CSV");
            Assert.AreEqual(123, cells[0, 1].IntValue, "A2.Value from CSV");
            cells[0, 3].PutValue("هل تتردد إلى هذه الصفحة كثيرًا؟ اجعل");
            ms = new MemoryStream();
            wb.Save(ms, new TxtSaveOptions() { Encoding = Encoding.UTF8, });
            Assert.AreEqual("EF-BB-BF", BitConverter.ToString(ms.GetBuffer(), 0, 3), "FileHeader of saved file");
        }
```

### See Also

* class [TxtSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


