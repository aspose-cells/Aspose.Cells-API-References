---
title: Workbook.ExportXml
second_title: Aspose.Cells for .NET API Reference
description: Workbook method. Export XML data linked by the specified XML map
type: docs
url: /net/aspose.cells/workbook/exportxml/
---
## ExportXml(string, string) {#exportxml_1}

Export XML data linked by the specified XML map.

```csharp
public void ExportXml(string mapName, string path)
```

| Parameter | Type | Description |
| --- | --- | --- |
| mapName | String | name of the XML map that need to be exported |
| path | String | the export path |

### Examples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodExportXmlWithStringStringDemo
    {
        public static void Run()
        {
            // Create a workbook and load the Excel file
            Workbook wb = new Workbook("Book1.xlsx");
            
            // Get the first XmlMap from the workbook
            if (wb.Worksheets.XmlMaps.Count > 0)
            {
                XmlMap xmlMap = wb.Worksheets.XmlMaps[0];
                
                // Export XML data using the XmlMap's name and output file path
                wb.ExportXml(xmlMap.Name, "output.xml");
                Console.WriteLine("XML exported successfully to output.xml");
            }
            else
            {
                Console.WriteLine("No XmlMap found in the workbook");
            }
        }
    }
}
```

### See Also

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## ExportXml(string, Stream) {#exportxml}

Export XML data.

```csharp
public void ExportXml(string mapName, Stream stream)
```

| Parameter | Type | Description |
| --- | --- | --- |
| mapName | String | name of the XML map that need to be exported |
| stream | Stream | the export stream |

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.IO;

    public class WorkbookMethodExportXmlWithStringStreamDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add sample data to worksheet
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("Item1");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["A3"].PutValue("Item2");
            worksheet.Cells["B3"].PutValue(200);

            // Create a memory stream to hold the XML data
            using (MemoryStream xmlStream = new MemoryStream())
            {
                try
                {
                    // Call ExportXml with mapName and stream parameters
                    workbook.ExportXml("SampleMap", xmlStream);

                    // Reset stream position to read the content
                    xmlStream.Position = 0;

                    // Read the XML content from the stream
                    using (StreamReader reader = new StreamReader(xmlStream))
                    {
                        string xmlContent = reader.ReadToEnd();
                        Console.WriteLine("Exported XML content:");
                        Console.WriteLine(xmlContent);
                    }

                    Console.WriteLine("ExportXml method executed successfully with parameters (String, Stream)");
                }
                catch (Exception ex)
                {
                    Console.WriteLine($"Error executing ExportXml method: {ex.Message}");
                }
            }

            // Save the workbook
            workbook.Save("WorkbookMethodExportXmlWithStringStreamDemo.xlsx");
        }
    }
}
```

### See Also

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


