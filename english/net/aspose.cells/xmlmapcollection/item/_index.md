---
title: XmlMapCollection.Item
second_title: Aspose.Cells for .NET API Reference
description: XmlMapCollection property. Gets the xml map by the specific index
type: docs
url: /net/aspose.cells/xmlmapcollection/item/
---
## XmlMapCollection indexer

Gets the xml map by the specific index.

```csharp
public XmlMap this[int index] { get; }
```

| Parameter | Description |
| --- | --- |
| index | The index. |

### Return Value

The xml map

### Examples

```csharp
// Called: wb.ExportXml(xmlMaps[0].Name, ms);
[Test]
        public void Property_Int32_()
        {
            Workbook wb = new Workbook(Constants.sourcePath + &quot;CELLSNET-51120.xlsm&quot;);

            XmlMapCollection xmlMaps = wb.Worksheets.XmlMaps;

            using (MemoryStream ms = new MemoryStream())
            {
                wb.ExportXml(xmlMaps[0].Name, ms);

                using (StreamReader sr = new StreamReader(ms, Encoding.UTF8))
                {
                    string line;
                    while ((line = sr.ReadLine()) != null)
                    {
                        line = line.Trim();
                        if (!string.IsNullOrEmpty(line))
                        {
                            if (line.StartsWith(&quot;&lt;?&quot;))
                            {
                                continue;
                            }

                            Assert.IsTrue(line.IndexOf(&quot;ns1:MaterialDisciplines&quot;) &gt; -1);
                            Assert.IsTrue(line.IndexOf(&quot;xmlns:ns1=\&quot;http://tempuri.org/XMLSchema.xsd\&quot;&quot;) &gt; -1);

                            break;
                        }
                    }
                }
            }
        }
```

### See Also

* class [XmlMap](../../xmlmap/)
* class [XmlMapCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


