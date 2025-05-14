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
// Called: wb.ExportXml(map.Name, savePath);
public void XmlMap_Property_Name()
{
    string sourcePath = Constants.sourcePath + "CELLSNET-49759/";
    Workbook wb = new Workbook(sourcePath + "Excel.xlsx");

    if (wb.Worksheets.XmlMaps.Count >= 1)
    {
        XmlMap map = wb.Worksheets.XmlMaps[0];

        string savePath = Constants.destPath + "example.xml";
        wb.ExportXml(map.Name, savePath);

        string content = File.ReadAllText(savePath);
        Assert.IsTrue(content.IndexOf("ShareClassSEDOLCode") == -1);
    }
}
```

### See Also

* class [XmlMap](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


