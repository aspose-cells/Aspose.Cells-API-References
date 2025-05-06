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
[Test]
        public void Type_XmlMap()
        {
            string sourcePath = Constants.sourcePath + &quot;CELLSNET-49759/&quot;;
            Workbook wb = new Workbook(sourcePath + &quot;Excel.xlsx&quot;);

            if (wb.Worksheets.XmlMaps.Count &gt;= 1)
            {
                XmlMap map = wb.Worksheets.XmlMaps[0];

                string savePath = Constants.destPath + &quot;CELLSNET-49759.xml&quot;;
                wb.ExportXml(map.Name, savePath);

                string content = File.ReadAllText(savePath);
                Assert.IsTrue(content.IndexOf(&quot;ShareClassSEDOLCode&quot;) == -1);
            }
        }
```

### See Also

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


