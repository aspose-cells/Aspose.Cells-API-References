---
title: "Workbook.ImportXml"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Workbook yöntemi. XML veri dosyasını çalışma kitabına içe aktarır/günceller"
type: docs
url: /tr/net/aspose.cells/workbook/importxml/
---
## ImportXml(string, string, int, int) {#importxml_1}

Bir XML veri dosyasını çalışma kitabına içe aktarır/günceller.

```csharp
public void ImportXml(string url, string sheetName, int row, int col)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| url | String | xml dosyasının url/yolu. |
| sheetName | String | hedef sayfa adı. |
| satır | Int32 | hedef satır |
| col | Int32 | hedef sütun |

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodImportXmlWithStringStringInt32Int32Demo
    {
        public static void Run()
        {
            // Bir çalışma kitabı nesnesi oluştur
            Workbook wb = new Workbook();
            
            // XML verisini A1 hücresinden başlayarak ilk çalışma sayfasına içe aktar
            wb.ImportXml("data.xml", "Sheet1", 0, 0);
            
            // Çalışma kitabını kaydedin
            wb.Save("output.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## ImportXml(Stream, string, int, int) {#importxml}

Bir XML veri dosyasını çalışma kitabına içe aktarır/günceller.

```csharp
public void ImportXml(Stream stream, string sheetName, int row, int col)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| akış | Stream | xml dosya akışı. |
| sheetName | String | hedef sayfa adı. |
| satır | Int32 | hedef satır. |
| col | Int32 | hedef sütun. |

### Örnekler

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
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();

            // Örnek XML verisi oluştur
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

            // XML dizesini MemoryStream'e dönüştür
            MemoryStream xmlStream = new MemoryStream();
            StreamWriter writer = new StreamWriter(xmlStream);
            writer.Write(xmlData);
            writer.Flush();
            xmlStream.Position = 0;

            try
            {
                // XML verisini ilk çalışma sayfasının A1 hücresinden başlayarak çalışma kitabına içe aktar
                workbook.ImportXml(xmlStream, "Sheet1", 0, 0);

                // Çalışma kitabını kaydedin
                workbook.Save("ImportXmlDemo.xlsx");
                Console.WriteLine("XML data imported successfully to ImportXmlDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error importing XML: {ex.Message}");
            }
            finally
            {
                // Kaynakları temizle
                xmlStream.Dispose();
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


