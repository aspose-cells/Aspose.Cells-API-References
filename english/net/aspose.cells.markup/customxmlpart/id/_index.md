---
title: CustomXmlPart.ID
second_title: Aspose.Cells for .NET API Reference
description: CustomXmlPart property. Gets and sets the id of the custom xml part
type: docs
url: /net/aspose.cells.markup/customxmlpart/id/
---
## CustomXmlPart.ID property

Gets and sets the id of the custom xml part.

```csharp
public string ID { get; set; }
```

### Examples

```csharp
// Called: Assert.AreEqual("2F087CB2-7CA8-43DA-B048-2E2F61F4936F",part.ID);
public void CustomXmlPart_Property_ID()
{
    Workbook workbook = new Workbook(Constants.sourcePath + "example.xlsx");
    //for (int i = 0; i < workbook.CustomXmlParts.Count; i++)
    //{
    //    Console.WriteLine(workbook.CustomXmlParts[i].ID);
    //}
    CustomXmlPart part = workbook.CustomXmlParts.SelectByID("2F087CB2-7CA8-43DA-B048-2E2F61F4936F");
    Assert.AreEqual("2F087CB2-7CA8-43DA-B048-2E2F61F4936F",part.ID);
    string x = "2F087CB2-7CA8-43DA-B048-2E2F61F0000F";
    part.ID = x;
    workbook.Save(Constants.destPath + "example.xlsx");
    workbook = new Workbook(Constants.destPath + "example.xlsx");
    part = workbook.CustomXmlParts.SelectByID(x);
    Assert.AreEqual(x, part.ID);

}
```

### See Also

* class [CustomXmlPart](../)
* namespace [Aspose.Cells.Markup](../../../aspose.cells.markup/)
* assembly [Aspose.Cells](../../../)


