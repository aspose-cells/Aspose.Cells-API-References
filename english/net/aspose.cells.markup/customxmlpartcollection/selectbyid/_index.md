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
// Called: part = workbook.CustomXmlParts.SelectByID(x);
[Test]
        public void Method_String_()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;CellsNet46130.xlsx&quot;);
            //for (int i = 0; i &lt; workbook.CustomXmlParts.Count; i++)
            //{
            //    Console.WriteLine(workbook.CustomXmlParts[i].ID);
            //}
            CustomXmlPart part = workbook.CustomXmlParts.SelectByID(&quot;2F087CB2-7CA8-43DA-B048-2E2F61F4936F&quot;);
            Assert.AreEqual(&quot;2F087CB2-7CA8-43DA-B048-2E2F61F4936F&quot;,part.ID);
            string x = &quot;2F087CB2-7CA8-43DA-B048-2E2F61F0000F&quot;;
            part.ID = x;
            workbook.Save(Constants.destPath + &quot;CellsNet46130.xlsx&quot;);
            workbook = new Workbook(Constants.destPath + &quot;CellsNet46130.xlsx&quot;);
            part = workbook.CustomXmlParts.SelectByID(x);
            Assert.AreEqual(x, part.ID);

        }
```

### See Also

* class [CustomXmlPart](../../customxmlpart/)
* class [CustomXmlPartCollection](../)
* namespace [Aspose.Cells.Markup](../../../aspose.cells.markup/)
* assembly [Aspose.Cells](../../../)


