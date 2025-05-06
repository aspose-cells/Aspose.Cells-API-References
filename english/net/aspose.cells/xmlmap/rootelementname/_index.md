---
title: XmlMap.RootElementName
second_title: Aspose.Cells for .NET API Reference
description: XmlMap property. Gets root element name
type: docs
url: /net/aspose.cells/xmlmap/rootelementname/
---
## XmlMap.RootElementName property

Gets root element name.

```csharp
public string RootElementName { get; }
```

### Examples

```csharp
// Called: string rootElementName = wb.Worksheets.XmlMaps[0].RootElementName;
[Test]
        public void Property_RootElementName()
        {
            Workbook wb = new Workbook(Constants.sourcePath + &quot;CELLSNET-45747.xlsm&quot;);
            string rootElementName = wb.Worksheets.XmlMaps[0].RootElementName;
            Assert.AreEqual(&quot;root&quot;, rootElementName);
        }
```

### See Also

* class [XmlMap](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


