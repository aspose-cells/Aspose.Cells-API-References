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
// Called: Encoding = Encoding.ASCII,
public void TxtSaveOptions_Property_Encoding()
{
    Assert.AreEqual(",,v_2_2,v_2_3,v_2_4\r\n,,v_3_2,v_3_3,v_3_4\r\n,,v_4_2,v_4_3,v_4_4\r\n",
        CSVTest.SaveAsCsv(new Workbook(), new TxtSaveOptions()
        {
            Encoding = Encoding.ASCII,
            LightCellsDataProvider = new LightCellsDataProviderJ43341(),
        }));
}
```

### See Also

* class [TxtSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


