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
// Called: wb.ExportXml(map.Name, Constants.destPath + "CELLSNET-49595.xml");
[Test]
        //Exception
        public void Property_Name()
        {
            // Load sample Excel file having XML Map
            Workbook wb = new Workbook(Constants.sourcePath + "CELLSNET-49595.xlsx");
            XmlMap map = wb.Worksheets.XmlMaps[0];
            wb.ExportXml(map.Name, Constants.destPath + "CELLSNET-49595.xml");
        }
```

### See Also

* class [XmlMap](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


