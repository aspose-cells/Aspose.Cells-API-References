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
// Called: Assert.AreEqual(1, reloadedWb.Worksheets.XmlMaps.Count);
[Test]
        public void Property_XmlMaps()
        {
            Workbook wb = new Workbook();
            XmlMapCollection maps = wb.Worksheets.XmlMaps;
            maps.Add(Constants.sourcePath+&quot;CELLSNET-47951/Sample.xsd&quot;);

            MemoryStream ms = new MemoryStream();
            wb.Save(ms, SaveFormat.Xlsx);
            ms.Position = 0;

            Workbook reloadedWb = new Workbook(ms);
            Assert.AreEqual(1, reloadedWb.Worksheets.XmlMaps.Count);
        }
```

### See Also

* class [XmlMapCollection](../../xmlmapcollection/)
* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


