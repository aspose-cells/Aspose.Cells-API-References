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

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodImportXmlWithStringStringInt32Int32Demo
    {
        public static void Run()
        {
            // Create a workbook object
            Workbook wb = new Workbook();
            
            // Import XML data into the first worksheet starting at cell A1
            wb.ImportXml("data.xml", "Sheet1", 0, 0);
            
            // Save the workbook
            wb.Save("output.xlsx");
        }
    }
}
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
using System;
using System.IO;
using System.Xml;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodImportXmlWithStreamStringInt32Int32Demo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            
            // Create sample XML data
            string xmlData = @"<?xml version='1.0' encoding='UTF-8'?>
                <Root>
                    <Row>
                        <Name>John</Name>
                        <Age>30</Age>
                    </Row>
                    <Row>
                        <Name>Mary</Name>
                        <Age>25</Age>
                    </Row>
                </Root>";

            // Convert XML string to stream
            MemoryStream stream = new MemoryStream();
            XmlDocument xmlDoc = new XmlDocument();
            xmlDoc.LoadXml(xmlData);
            xmlDoc.Save(stream);
            stream.Position = 0;

            // Import XML data into worksheet
            workbook.ImportXml(stream, "Sheet1", 0, 0);

            // Save the workbook
            workbook.Save("output.xlsx");
        }
    }
}
```

### See Also

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


