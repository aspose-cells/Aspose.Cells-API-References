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
// Called: Assert.AreEqual(x, part.ID);
[Test]
        public void Property_ID()
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

* class [CustomXmlPart](../)
* namespace [Aspose.Cells.Markup](../../../aspose.cells.markup/)
* assembly [Aspose.Cells](../../../)


