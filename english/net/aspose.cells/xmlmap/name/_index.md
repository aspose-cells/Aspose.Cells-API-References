---
title: XmlMap.Name
second_title: Aspose.Cells for .NET API Reference
description: XmlMap property. Returns or sets the name of the object
type: docs
url: /net/aspose.cells/xmlmap/name/
---
## XmlMap.Name property

Returns or sets the name of the object.

```csharp
public string Name { get; set; }
```

### Examples

```csharp
// Called: wb.ExportXml(map.Name, Constants.destPath + &amp;quot;CELLSNET-49497.xml&amp;quot;);
[Test]
        //Exception
        public void Property_Name()
        {
            // Load sample Excel file having XML Map
            Workbook wb = new Workbook(Constants.sourcePath + &quot;CELLSNET-49497.xlsx&quot;);
            XmlMap map = wb.Worksheets.XmlMaps[0];
            wb.ExportXml(map.Name, Constants.destPath + &quot;CELLSNET-49497.xml&quot;);
        }
```

### See Also

* class [XmlMap](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


