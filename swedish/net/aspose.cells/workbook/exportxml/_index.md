---
title: "Workbook.ExportXml"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Workbook-metod. Exportera XML-data som är länkad via den angivna XML-kartan"
type: docs
url: /sv/net/aspose.cells/workbook/exportxml/
---
## ExportXml(string, string) {#exportxml_1}

Exportera XML-data länkad av den specificerade XML-kartan.

```csharp
public void ExportXml(string mapName, string path)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| mapName | String | namn på XML-kartan som ska exporteras |
| sökväg | String | export-sökvägen |

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodExportXmlWithStringStringDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok och läs in Excel-filen
            Workbook wb = new Workbook("Book1.xlsx");
            
            // Hämta den första XmlMap från arbetsboken
            if (wb.Worksheets.XmlMaps.Count > 0)
            {
                XmlMap xmlMap = wb.Worksheets.XmlMaps[0];
                
                // Exportera XML-data med XmlMap:s namn och utdatafilens sökväg
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

### Se även

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## ExportXml(string, Stream) {#exportxml}

Exportera XML-data.

```csharp
public void ExportXml(string mapName, Stream stream)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| mapName | String | namn på XML-kartan som ska exporteras |
| ström | Ström | exportströmmen |

### Exempel

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodExportXmlWithStringStreamDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok och lägg till lite data
            using (Workbook workbook = new Workbook())
            {
                Worksheet sheet = workbook.Worksheets[0];
                sheet.Cells["A1"].PutValue("Id");
                sheet.Cells["B1"].PutValue("Name");
                sheet.Cells["A2"].PutValue(1);
                sheet.Cells["B2"].PutValue("Alice");
                sheet.Cells["A3"].PutValue(2);
                sheet.Cells["B3"].PutValue("Bob");

                // Namn på XML-kartan som ska exporteras – för demonstrationsändamål använder vi ett platshållarnamn
                string mapName = "SampleMap";

                try
                {
                    // Exportera XML-kartan till en fil med en FileStream (String, Stream-överladdning)
                    string outputPath = "ExportedSample.xml";
                    using (FileStream fs = new FileStream(outputPath, FileMode.Create, FileAccess.Write))
                    {
                        workbook.ExportXml(mapName, fs);
                    }

                    Console.WriteLine($"ExportXml completed successfully. Output saved to '{outputPath}'.");
                }
                catch (Exception ex)
                {
                    Console.WriteLine($"Error during ExportXml: {ex.Message}");
                }
            }
        }
    }
}
```

### Se även

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


