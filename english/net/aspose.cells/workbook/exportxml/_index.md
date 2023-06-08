---
title: Workbook.ExportXml
second_title: Aspose.Cells for .NET API Reference
description: Workbook method. Export XML data linked by the specified XML map
type: docs
url: /net/aspose.cells/workbook/exportxml/
---
## ExportXml(string, string) {#exportxml_1}

Export XML data linked by the specified XML map.

```csharp
public void ExportXml(string mapName, string path)
```

| Parameter | Type | Description |
| --- | --- | --- |
| mapName | String | name of the XML map that need to be exported |
| path | String | the export path |

### Examples

The following code exported the data linked by the first XmlMap.

```csharp
Workbook wb = new Workbook("Book1.xlsx");

//Make sure that the source xlsx file contains a XmlMap.
XmlMap xmlMap = wb.Worksheets.XmlMaps[0];

wb.ExportXml(xmlMap.Name, "output.xml");
```

### See Also

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## ExportXml(string, Stream) {#exportxml}

Export XML data.

```csharp
public void ExportXml(string mapName, Stream stream)
```

| Parameter | Type | Description |
| --- | --- | --- |
| mapName | String | name of the XML map that need to be exported |
| stream | Stream | the export stream |

### See Also

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


