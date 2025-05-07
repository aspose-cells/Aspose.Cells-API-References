---
title: OoxmlSaveOptions.EnableZip64
second_title: Aspose.Cells for .NET API Reference
description: OoxmlSaveOptions property. Always use ZIP64 extensions when writing zip archives even when unnecessary
type: docs
url: /net/aspose.cells/ooxmlsaveoptions/enablezip64/
---
## OoxmlSaveOptions.EnableZip64 property

Always use ZIP64 extensions when writing zip archives, even when unnecessary.

```csharp
public bool EnableZip64 { get; set; }
```

### Examples

```csharp
// Called: workBook.Save(outStream, new OoxmlSaveOptions(SaveFormat.Xlsx) { EnableZip64 = true });
[Test]
        public void Property_EnableZip64()
        {
            var workBook = new Workbook();
            var outStream = new AppendOnlyMemStream();
            //  outStream.AllowReadSeek = true;
            using (outStream)
            {
                workBook.Save(outStream, new OoxmlSaveOptions(SaveFormat.Xlsx) { EnableZip64 = true });
                // Note to Aspose Engrs, the below works just fine
                // workBook.Save(outStream, SaveFormat.Xlsx);
            }
            outStream.AllowReadSeek = true;
            outStream.Seek(0, SeekOrigin.Begin);
            using (var fileStream = File.Create(Constants.destPath + "CellsNet47315.xlsx"))
            {
                outStream.AllowReadSeek = true;
                outStream.Seek(0, SeekOrigin.Begin);
                outStream.CopyTo(fileStream);
            }
        }
```

### See Also

* class [OoxmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


