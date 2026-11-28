---
title: "Workbook.ExportXml"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Workbook yöntemi. Belirtilen XML haritası tarafından bağlanan XML verilerini dışa aktar"
type: docs
url: /tr/net/aspose.cells/workbook/exportxml/
---
## ExportXml(string, string) {#exportxml_1}

Belirtilen XML haritası ile bağlanmış XML verisini dışa aktar.

```csharp
public void ExportXml(string mapName, string path)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| mapName | String | Dışa aktarılması gereken XML haritasının adı |
| yol | String | dışa aktarma yolu |

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodExportXmlWithStringStringDemo
    {
        public static void Run()
        {
            // Bir çalışma kitabı oluştur ve Excel dosyasını yükle
            Workbook wb = new Workbook("Book1.xlsx");
            
            // Çalışma kitabından ilk XmlMap'i al
            if (wb.Worksheets.XmlMaps.Count > 0)
            {
                XmlMap xmlMap = wb.Worksheets.XmlMaps[0];
                
                // XmlMap'in adı ve çıktı dosya yolu kullanılarak XML verilerini dışa aktar
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

### Ayrıca Bakınız

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## ExportXml(string, Stream) {#exportxml}

XML verisini dışa aktar.

```csharp
public void ExportXml(string mapName, Stream stream)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| mapName | String | Dışa aktarılması gereken XML haritasının adı |
| akış | Stream | dışa aktarma akışı |

### Örnekler

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
            // Yeni bir çalışma kitabı oluştur ve bazı veriler ekle
            using (Workbook workbook = new Workbook())
            {
                Worksheet sheet = workbook.Worksheets[0];
                sheet.Cells["A1"].PutValue("Id");
                sheet.Cells["B1"].PutValue("Name");
                sheet.Cells["A2"].PutValue(1);
                sheet.Cells["B2"].PutValue("Alice");
                sheet.Cells["A3"].PutValue(2);
                sheet.Cells["B3"].PutValue("Bob");

                // Dışa aktarılacak XML haritasının adı – demo amaçları için bir yer tutucu ad kullanıyoruz
                string mapName = "SampleMap";

                try
                {
                    // XML haritasını bir dosyaya FileStream (String, Stream aşırı yüklemesi) kullanarak dışa aktar
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

### Ayrıca Bakınız

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


