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
            Workbook workbook1 = new Workbook(Constants.sourcePath +  &quot;CELLSNET-42197.csv&quot;, options);
            Assert.AreEqual(workbook1.Worksheets[0].Cells[&quot;A2&quot;].StringValue, &quot;NBYPN-E&quot;);
            Assert.AreEqual(workbook1.Worksheets[0].Cells[&quot;A3&quot;].StringValue, &quot;NBYPN-E&quot;);
        }
```

### See Also

* class [TxtLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


