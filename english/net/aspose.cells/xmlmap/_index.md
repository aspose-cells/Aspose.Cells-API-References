---
title: Class XmlMap
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.XmlMap class. Represents Xml map information
type: docs
url: /net/aspose.cells/xmlmap/
---
## XmlMap class

Represents Xml map information.

```csharp
public class XmlMap
```

## Properties

| Name | Description |
| --- | --- |
| [DataBinding](../../aspose.cells/xmlmap/databinding/) { get; } | Gets an [`XmlDataBinding`](../xmldatabinding/) of this map. |
| [Name](../../aspose.cells/xmlmap/name/) { get; set; } | Returns or sets the name of the object. |
| [RootElementName](../../aspose.cells/xmlmap/rootelementname/) { get; } | Gets root element name. |

### Examples

```csharp
// Called: XmlMap map = wb.Worksheets.XmlMaps[0];
//Exception
public void Cells_Type_XmlMap()
{
    // Load sample Excel file having XML Map
    Workbook wb = new Workbook(Constants.sourcePath + "example.xlsx");
    XmlMap map = wb.Worksheets.XmlMaps[0];
    wb.ExportXml(map.Name, Constants.destPath + "example.xml");
}
```

### See Also

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


