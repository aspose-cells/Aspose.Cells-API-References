---
title: Class CustomXmlPart
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.Markup.CustomXmlPart class. Represents a Custom XML Data Storage Part custom XML data within a package
type: docs
url: /net/aspose.cells.markup/customxmlpart/
---
## CustomXmlPart class

Represents a Custom XML Data Storage Part (custom XML data within a package).

```csharp
public class CustomXmlPart
```

## Properties

| Name | Description |
| --- | --- |
| [Data](../../aspose.cells.markup/customxmlpart/data/) { get; set; } | Gets or sets the XML content of this Custom XML Data Storage Part. |
| [ID](../../aspose.cells.markup/customxmlpart/id/) { get; set; } | Gets and sets the id of the custom xml part. |
| [SchemaData](../../aspose.cells.markup/customxmlpart/schemadata/) { get; set; } | Gets or sets the XML content of this Custom XML Schema Data Storage Part. |

### Examples

```csharp
// Called: CustomXmlPart part = workbook.CustomXmlParts.SelectByID("2F087CB2-7CA8-43DA-B048-2E2F61F4936F");
[Test]
        public void Type_CustomXmlPart()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + "CellsNet46130.xlsx");
            //for (int i = 0; i < workbook.CustomXmlParts.Count; i++)
            //{
            //    Console.WriteLine(workbook.CustomXmlParts[i].ID);
            //}
            CustomXmlPart part = workbook.CustomXmlParts.SelectByID("2F087CB2-7CA8-43DA-B048-2E2F61F4936F");
            Assert.AreEqual("2F087CB2-7CA8-43DA-B048-2E2F61F4936F",part.ID);
            string x = "2F087CB2-7CA8-43DA-B048-2E2F61F0000F";
            part.ID = x;
            workbook.Save(Constants.destPath + "CellsNet46130.xlsx");
            workbook = new Workbook(Constants.destPath + "CellsNet46130.xlsx");
            part = workbook.CustomXmlParts.SelectByID(x);
            Assert.AreEqual(x, part.ID);

        }
```

### See Also

* namespace [Aspose.Cells.Markup](../../aspose.cells.markup/)
* assembly [Aspose.Cells](../../)


