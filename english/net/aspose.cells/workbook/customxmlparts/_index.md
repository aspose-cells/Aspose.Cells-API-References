---
title: Workbook.CustomXmlParts
second_title: Aspose.Cells for .NET API Reference
description: Workbook property. Represents a Custom XML Data Storage Part custom XML data within a package
type: docs
url: /net/aspose.cells/workbook/customxmlparts/
---
## Workbook.CustomXmlParts property

Represents a Custom XML Data Storage Part (custom XML data within a package).

```csharp
public CustomXmlPartCollection CustomXmlParts { get; }
```

### Examples

```csharp
// Called: Assert.AreEqual(1, wb.CustomXmlParts.Count);
        public void Workbook_Property_CustomXmlParts()
        {
            Workbook wb = new Workbook();
            string data = "<MyXmlData1 xmlns=\"http://my.namespace.com\"/>";
            string schema = "<?xml version=\"1.0\" encoding=\"UTF-8\" standalone=\"no\"?>"
+ "<ds:datastoreItem ds:itemID=\"{1D3CF2F4-9155-40AE-99F6-33298D217F89}\" xmlns:ds=\"http://schemas.openxmlformats.org/officeDocument/2006/customXml\">"
    + "<ds:schemaRefs>"
        + "<ds:schemaRef ds:uri=\"http://my.namespace.com\"/>"
    + "</ds:schemaRefs>"
+ "</ds:datastoreItem>";
            wb.CustomXmlParts.Add(Encoding.UTF8.GetBytes(data), Encoding.UTF8.GetBytes(schema));
            wb.Save(Constants.destPath + "example.xlsx");
            wb = new Workbook(Constants.destPath + "example.xlsx");
            Assert.AreEqual(1, wb.CustomXmlParts.Count);
        }
```

### See Also

* class [CustomXmlPartCollection](../../../aspose.cells.markup/customxmlpartcollection/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


