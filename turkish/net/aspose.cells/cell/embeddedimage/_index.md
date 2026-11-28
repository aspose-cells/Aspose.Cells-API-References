---
title: "Cell.EmbeddedImage"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Cell özelliği. Hücredeki gömülü resmi alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells/cell/embeddedimage/
---
## Cell.EmbeddedImage property

Hücredeki gömülü resmi alır ve ayarlar.

```csharp
public byte[] EmbeddedImage { get; set; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.IO;

    public class CellPropertyEmbeddedImageDemo
    {
        public static void Run()
        {
            try
            {
                // Yeni bir çalışma kitabı oluşturun ve ilk çalışma sayfasını alın.
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];

                // Gömülü resmi depolamak için bir hücre seç
                Cell cell = worksheet.Cells["B2"];

                // 1x1 piksel şeffaf PNG (Base64 kodlu)
                const string pngBase64 =
                    "iVBORw0KGgoAAAANSUhEUgAAAAEAAAABCAQAAAC1HAwCAAAAC0lEQVR42mP8/x8AAwMCAO2b4ZcAAAAASUVORK5CYII=";

                // Base64 dizesini bayt dizisine dönüştür
                byte[] imageBytes = Convert.FromBase64String(pngBase64);

                // Gömülü resmi hücreye ayarla
                cell.EmbeddedImage = imageBytes;

                // Gömülü resmi hücreden geri al
                byte[] retrievedBytes = cell.EmbeddedImage;

                // Alınan resmi bir dosyaya yazarak doğru şekilde depolandığını doğrula
                string outputImagePath = "EmbeddedImage_Output.png";
                File.WriteAllBytes(outputImagePath, retrievedBytes);

                Console.WriteLine($"Embedded image byte length: {retrievedBytes.Length}");
                Console.WriteLine($"Embedded image saved to: {Path.GetFullPath(outputImagePath)}");

                // Çalışma kitabını kaydet (gömülü resim .xlsx içinde depolanır)
                string workbookPath = "EmbeddedImageDemo.xlsx";
                workbook.Save(workbookPath);
                Console.WriteLine($"Workbook saved to: {Path.GetFullPath(workbookPath)}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


