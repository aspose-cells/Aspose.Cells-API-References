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
// Called: saveOptions.EnableZip64 = true;
[Test]
        public void Property_EnableZip64()
        {
            Workbook workbook = new Workbook();
            workbook.Worksheets[0].Cells[&quot;A10&quot;].PutValue(&quot;sdfsfd&quot;);
            OoxmlSaveOptions saveOptions = new OoxmlSaveOptions();
            saveOptions.UpdateZoom = true;
            saveOptions.EnableZip64 = true;
            workbook.Save(Constants.destPath + &quot;SaveOptions01.xlsx&quot;, saveOptions);
        }
```

### See Also

* class [OoxmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


