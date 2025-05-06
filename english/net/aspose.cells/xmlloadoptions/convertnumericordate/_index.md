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
[Test]
        public void Property_ConvertNumericOrDate()
        {
            bool[] flags = {true, false};
            foreach(bool flag in flags)
            {
                XmlLoadOptions options = new XmlLoadOptions();
                options.ConvertNumericOrDate = flag;
                Workbook wb = new Workbook(Constants.sourcePath + &quot;CELLSPYTHONNET218.xml&quot;, options);
                // wb.Worksheets.RefreshAll();
                Cell cell = wb.Worksheets[0].Cells[&quot;E4&quot;];
               Assert.IsTrue( (cell.Type == CellValueType.IsString) != flag);
                wb.Save(Constants.destPath + &quot;CELLSPYTHONNET218.xlsx&quot;);
            }
            
        }
```

### See Also

* class [XmlLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


