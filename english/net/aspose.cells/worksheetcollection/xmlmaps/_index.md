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
[Test]
        //Exception
        public void Property_XmlMaps()
        {
            // Load sample Excel file having XML Map
            Workbook wb = new Workbook(Constants.sourcePath + "CELLSNET-49497.xlsx");
            XmlMap map = wb.Worksheets.XmlMaps[0];
            wb.ExportXml(map.Name, Constants.destPath + "CELLSNET-49497.xml");
        }
```

### See Also

* class [XmlMapCollection](../../xmlmapcollection/)
* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


