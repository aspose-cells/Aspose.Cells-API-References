---
title: CustomXmlPartCollection.SelectByID
second_title: Aspose.Cells for .NET API Reference
description: CustomXmlPartCollection method. Gets an item by id
type: docs
url: /net/aspose.cells.markup/customxmlpartcollection/selectbyid/
---
## CustomXmlPartCollection.SelectByID method

Gets an item by id.

```csharp
public CustomXmlPart SelectByID(string id)
```

| Parameter | Type | Description |
| --- | --- | --- |
| id | String | Contains the GUID for the custom XML part. |

### Examples

```csharp
// Called: CustomXmlPart part = workbook.CustomXmlParts.SelectByID("2F087CB2-7CA8-43DA-B048-2E2F61F4936F");
[Test]
        public void Method_String_()
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

* class [CustomXmlPart](../../customxmlpart/)
* class [CustomXmlPartCollection](../)
* namespace [Aspose.Cells.Markup](../../../aspose.cells.markup/)
* assembly [Aspose.Cells](../../../)


