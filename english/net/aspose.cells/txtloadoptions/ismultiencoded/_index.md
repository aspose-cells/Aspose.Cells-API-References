---
title: TxtLoadOptions.IsMultiEncoded
second_title: Aspose.Cells for .NET API Reference
description: TxtLoadOptions property. True means that the file contains several encoding
type: docs
url: /net/aspose.cells/txtloadoptions/ismultiencoded/
---
## TxtLoadOptions.IsMultiEncoded property

True means that the file contains several encoding.

```csharp
public bool IsMultiEncoded { get; set; }
```

### Examples

```csharp
// Called: options.IsMultiEncoded = true;
[Test]
        public void Property_IsMultiEncoded()
        {
            TxtLoadOptions options = new TxtLoadOptions();
            options.IsMultiEncoded = true;
            Workbook workbook1 = new Workbook(Constants.sourcePath +  "CELLSNET-42197.csv", options);
            Assert.AreEqual(workbook1.Worksheets[0].Cells["A2"].StringValue, "NBYPN-E");
            Assert.AreEqual(workbook1.Worksheets[0].Cells["A3"].StringValue, "NBYPN-E");
        }
```

### See Also

* class [TxtLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


