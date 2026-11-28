---
title: "Enum DirectoryType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.DirectoryType enum. Dosya adının dizin tipini temsil eder"
type: docs
url: /tr/net/aspose.cells/directorytype/
---
## DirectoryType enumeration

Dosya adının dizin türünü temsil eder.

```csharp
public enum DirectoryType
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| Volume | `0` | MS-DOS sürücü harfini temsil eder. Sürücü harfi izlenir. Veya \\server\share\myfile.xls gibi UNC dosya adları. |
| SameVolume | `1` | Kaynak çalışma kitabının bağımlı çalışma kitabıyla aynı sürücüde olduğunu gösterir (sürücü harfi atlanır). |
| DownDirectory | `2` | Kaynak çalışma kitabının geçerli dizinin bir alt dizininde olduğunu gösterir. |
| UpDirectory | `3` | Kaynak çalışma kitabının geçerli dizinin üst dizininde olduğunu gösterir. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class DirectoryTypeDemo
    {
        public static void DirectoryTypeExample()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();

            // Çalışma kitabına yeni bir çalışma sayfası ekle
            Worksheet worksheet = workbook.Worksheets[0];

            // Çalışma sayfasına örnek veri ekle
            worksheet.Cells["A1"].PutValue("Data");
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(200);
            worksheet.Cells["A4"].PutValue(300);

            // Çalışma kitabına harici bir bağlantı ekle
            string externalFileName = "externalWorkbook.xlsx";
            string[] sheetNames = { "Sheet1" };

            // DirectoryType.Volume ile harici bağlantı ekle
            int linkIndex = workbook.Worksheets.ExternalLinks.Add(DirectoryType.Volume, externalFileName, sheetNames);

            // Eklenen harici bağlantıyı al
            ExternalLink externalLink = workbook.Worksheets.ExternalLinks[linkIndex];

            // Harici bağlantının ayrıntılarını çıktı olarak ver
            Console.WriteLine("External Link Details:");
            Console.WriteLine("File Name: " + externalLink.DataSource);

            // Çalışma kitabını kaydedin
            workbook.Save("DirectoryTypeExample.xlsx");
            workbook.Save("DirectoryTypeExample.pdf");
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


