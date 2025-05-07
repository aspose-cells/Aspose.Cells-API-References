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
// Called: part = workbook.CustomXmlParts.SelectByID(x);
[Test]
        public void Property_CustomXmlParts()
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

* class [CustomXmlPartCollection](../../../aspose.cells.markup/customxmlpartcollection/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


