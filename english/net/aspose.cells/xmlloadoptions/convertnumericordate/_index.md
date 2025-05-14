---
title: XmlLoadOptions.ConvertNumericOrDate
second_title: Aspose.Cells for .NET API Reference
description: XmlLoadOptions property. Indicates whether converting the value in xml file to numeric or date
type: docs
url: /net/aspose.cells/xmlloadoptions/convertnumericordate/
---
## XmlLoadOptions.ConvertNumericOrDate property

Indicates whether converting the value in xml file to numeric or date.

```csharp
public bool ConvertNumericOrDate { get; set; }
```

### Examples

```csharp
// Called: options.ConvertNumericOrDate = flag;
public void XmlLoadOptions_Property_ConvertNumericOrDate()
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


