---
title: Workbook.ImportXml
second_title: Aspose.Cells for .NET API Reference
description: Workbook method. Imports/Updates an XML data file into the workbook
type: docs
url: /net/aspose.cells/workbook/importxml/
---
## ImportXml(string, string, int, int) {#importxml_1}

Imports/Updates an XML data file into the workbook.

```csharp
public void ImportXml(string url, string sheetName, int row, int col)
```

| Parameter | Type | Description |
| --- | --- | --- |
| url | String | the url/path of the xml file. |
| sheetName | String | the destination sheet name. |
| row | Int32 | the destination row |
| col | Int32 | the destination column |

### Examples

The following code imports xml data into worksheet 'Sheet 1' at Cell A1.

```csharp
Workbook wb = new Workbook("Book1.xlsx");

wb.ImportXml("xml.xml", "Sheet1", 0, 0);

wb.Save("output.xlsx");
```

### See Also

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## ImportXml(Stream, string, int, int) {#importxml}

Imports/Updates an XML data file into the workbook.

```csharp
public void ImportXml(Stream stream, string sheetName, int row, int col)
```

| Parameter | Type | Description |
| --- | --- | --- |
| stream | Stream | the xml file stream. |
| sheetName | String | the destination sheet name. |
| row | Int32 | the destination row. |
| col | Int32 | the destination column. |

### Examples

```csharp
// Called: workbook.ImportXml(stream, name, 1, 1);
[Test]
        public void Method_Int32_()
        {
            string sourcePath = Constants.sourcePath + "CELLSNET-47105/";
            Workbook workbook = new Workbook(sourcePath + "Unmapped.xlsx");

            System.Xml.XmlDocument document = new System.Xml.XmlDocument();
            document.Load(sourcePath + "Unmapped.xml");
            System.IO.Stream stream = new System.IO.MemoryStream();
            document.Save(stream);
            stream.Position = 0;
            string name = workbook.Worksheets[0].Name.ToString();

            workbook.ImportXml(stream, name, 1, 1);

            Cells cells = workbook.Worksheets[0].Cells;
            Assert.AreEqual("Test1", cells["B4"].StringValue);
            Assert.AreEqual("Test2", cells["C4"].StringValue);
            Assert.AreEqual("Test3", cells["D4"].StringValue);
            Assert.AreEqual("Test4", cells["B5"].StringValue);
            Assert.AreEqual("Test5", cells["C5"].StringValue);
            Assert.AreEqual("Test6", cells["D5"].StringValue);
        }
```

### See Also

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


