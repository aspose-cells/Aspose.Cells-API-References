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
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.IO;

    public class WorkbookMethodImportXmlWithStreamStringInt32Int32Demo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();

            // Create sample XML data
            string xmlData = @"<Products>
                <Product>
                    <Name>Laptop</Name>
                    <Price>999.99</Price>
                </Product>
                <Product>
                    <Name>Phone</Name>
                    <Price>699.99</Price>
                </Product>
            </Products>";

            // Convert XML string to a MemoryStream
            MemoryStream xmlStream = new MemoryStream();
            StreamWriter writer = new StreamWriter(xmlStream);
            writer.Write(xmlData);
            writer.Flush();
            xmlStream.Position = 0;

            try
            {
                // Import XML data into the workbook starting at cell A1 of the first worksheet
                workbook.ImportXml(xmlStream, "Sheet1", 0, 0);

                // Save the workbook
                workbook.Save("ImportXmlDemo.xlsx");
                Console.WriteLine("XML data imported successfully to ImportXmlDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error importing XML: {ex.Message}");
            }
            finally
            {
                // Clean up resources
                xmlStream.Dispose();
            }
        }
    }
}
```

### See Also

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


