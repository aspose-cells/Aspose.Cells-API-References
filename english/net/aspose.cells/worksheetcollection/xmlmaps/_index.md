---
title: WorksheetCollection.XmlMaps
second_title: Aspose.Cells for .NET API Reference
description: WorksheetCollection property. Gets and sets the XML maps in the workbook
type: docs
url: /net/aspose.cells/worksheetcollection/xmlmaps/
---
## WorksheetCollection.XmlMaps property

Gets and sets the XML maps in the workbook.

```csharp
public XmlMapCollection XmlMaps { get; set; }
```

### Examples

```csharp
// Called: XmlMap map = wb.Worksheets.XmlMaps[0];
//Exception
public void WorksheetCollection_Property_XmlMaps()
{
    // Load sample Excel file having XML Map
    Workbook wb = new Workbook(Constants.sourcePath + "example.xlsx");
    XmlMap map = wb.Worksheets.XmlMaps[0];
    wb.ExportXml(map.Name, Constants.destPath + "example.xml");
}
```

### See Also

* class [XmlMapCollection](../../xmlmapcollection/)
* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


