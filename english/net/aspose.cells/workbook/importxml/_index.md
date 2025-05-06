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
// Called: lWorkBook.ImportXml(stream, &amp;quot;Sheet1&amp;quot;, 0, 0);
[Test]
       public void Method_Int32_()
        {
            string aFilePath = Constants.sourcePath + &quot;CellsNet52662.xlsx&quot;;
            string aXmlPath = Constants.sourcePath + &quot;CellsNet52662.xml&quot;;
            string destPath = Constants.destPath + &quot;CellsNet52662.xlsx&quot;;
            using (Workbook lWorkBook = new Workbook(aFilePath))
            {
                var lWorksheet = lWorkBook.Worksheets[0];
                System.Xml.XmlDocument document = new System.Xml.XmlDocument();
                document.Load(aXmlPath);
                System.IO.Stream stream = new System.IO.MemoryStream();
                document.Save(stream);
                stream.Position = 0;

                lWorkBook.ImportXml(stream, &quot;Sheet1&quot;, 0, 0);
                Cell k2 = lWorksheet.Cells[&quot;k2&quot;];
                Assert.AreEqual(&quot;=[@[ns1:TRN_AMOUNT]]*-1&quot;,k2.Formula);
                Assert.IsTrue(Util.CompareColor(Color.Yellow, k2.GetStyle().ForegroundColor));
                lWorkBook.Save(destPath);

            }

        }
```

### See Also

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


