---
title: XmlMapCollection.Add
second_title: Aspose.Cells for .NET API Reference
description: XmlMapCollection method. Add a XmlMap by the url/path of a xml/xsd file
type: docs
url: /net/aspose.cells/xmlmapcollection/add/
---
## XmlMapCollection.Add method

Add a [`XmlMap`](../../xmlmap/) by the url/path of a xml/xsd file.

```csharp
public int Add(string url)
```

| Parameter | Type | Description |
| --- | --- | --- |
| url | String | url/path of a xml/xsd file. |

### Return Value

[`XmlMap`](../../xmlmap/) object index.

### Examples

The following code adds two XmlMaps by a xsd file and a xml file.

```csharp
Workbook wb = new Workbook();

XmlMapCollection xmlMapCollection = wb.Worksheets.XmlMaps;

//Add a XmlMap by a xsd file.
xmlMapCollection.Add("schema.xsd");

//Add a XmlMap by a xml file.
xmlMapCollection.Add("xml.xml");

wb.Save("twoXmlMaps.xlsx");
```

### See Also

* class [XmlMapCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


