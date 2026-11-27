---
title: "Workbook.ImportXml"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Workbook-metod. Importerar/Uppdaterar en XML-datafil i arbetsboken"
type: docs
url: /sv/net/aspose.cells/workbook/importxml/
---
## ImportXml(string, string, int, int) {#importxml_1}

Importerar/Uppdaterar en XML‑datafil i arbetsboken.

```csharp
public void ImportXml(string url, string sheetName, int row, int col)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| url | String | url/vägen till xml-filen. |
| sheetName | String | namnet på destinationsarket. |
| row | Int32 | destinationsraden |
| kol | Int32 | destinationskolumnen |

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodImportXmlWithStringStringInt32Int32Demo
    {
        public static void Run()
        {
            // Skapa ett arbetsbok-objekt
            Workbook wb = new Workbook();
            
            // Importera XML-data till det första kalkylbladet med start i cell A1
            wb.ImportXml("data.xml", "Sheet1", 0, 0);
            
            // Spara arbetsboken
            wb.Save("output.xlsx");
        }
    }
}
```

### Se även

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## ImportXml(Stream, string, int, int) {#importxml}

Importerar/Uppdaterar en XML‑datafil i arbetsboken.

```csharp
public void ImportXml(Stream stream, string sheetName, int row, int col)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| ström | Ström | XML-filströmmen. |
| sheetName | String | namnet på destinationsarket. |
| row | Int32 | destinationsraden. |
| kol | Int32 | destinationskolumnen. |

### Exempel

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
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();

            // Skapa exempel på XML-data
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

            // Konvertera XML-sträng till en MemoryStream
            MemoryStream xmlStream = new MemoryStream();
            StreamWriter writer = new StreamWriter(xmlStream);
            writer.Write(xmlData);
            writer.Flush();
            xmlStream.Position = 0;

            try
            {
                // Importera XML-data till arbetsboken med start i cell A1 på det första kalkylbladet
                workbook.ImportXml(xmlStream, "Sheet1", 0, 0);

                // Spara arbetsboken
                workbook.Save("ImportXmlDemo.xlsx");
                Console.WriteLine("XML data imported successfully to ImportXmlDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error importing XML: {ex.Message}");
            }
            finally
            {
                // Rensa resurser
                xmlStream.Dispose();
            }
        }
    }
}
```

### Se även

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


