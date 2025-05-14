---
title: XmlLoadOptions.XmlLoadOptions
second_title: Aspose.Cells for .NET API Reference
description: XmlLoadOptions constructor. Represents the options of loading xml file
type: docs
url: /net/aspose.cells/xmlloadoptions/xmlloadoptions/
---
## XmlLoadOptions() {#constructor}

Represents the options of loading xml file.

```csharp
public XmlLoadOptions()
```

### Examples

```csharp
// Called: XmlLoadOptions options = new XmlLoadOptions();
public void XmlLoadOptions_Constructor()
{
    bool[] flags = {true, false};
    foreach(bool flag in flags)
    {
        XmlLoadOptions options = new XmlLoadOptions();
        options.ConvertNumericOrDate = flag;
        Workbook wb = new Workbook(Constants.sourcePath + "example.xml", options);
        // wb.Worksheets.RefreshAll();
        Cell cell = wb.Worksheets[0].Cells["E4"];
       Assert.IsTrue( (cell.Type == CellValueType.IsString) != flag);
        wb.Save(Constants.destPath + "example.xlsx");
    }
            
}
```

### See Also

* class [XmlLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## XmlLoadOptions(LoadFormat) {#constructor_1}

Represents the options of loading xml file.

```csharp
public XmlLoadOptions(LoadFormat type)
```

| Parameter | Type | Description |
| --- | --- | --- |
| type | LoadFormat | The load format type. |

### See Also

* enum [LoadFormat](../../loadformat/)
* class [XmlLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


