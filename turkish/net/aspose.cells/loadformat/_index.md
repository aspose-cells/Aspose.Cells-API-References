---
title: "Enum LoadFormat"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.LoadFormat enum. Yükleme dosya formatını temsil eder"
type: docs
url: /tr/net/aspose.cells/loadformat/
---
## LoadFormat enumeration

Yükleme dosya biçimini temsil eder.

```csharp
public enum LoadFormat
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| Auto | `0` | Formatı otomatik olarak tanımayı temsil eder. |
| Csv | `1` | Virgülle Ayrılmış Değerler (CSV) metin dosyası. |
| CSV | `1` | Virgülle Ayrılmış Değerler (CSV) metin dosyası. NOT: Bu üye artık kullanımdan kaldırıldı. Bunun yerine lütfen Csv özelliğini kullanın. Bu özellik Nisan 2021'den itibaren 6 ay sonra kaldırılacak. Aspose, yaşadığınız herhangi bir rahatsızlıktan dolayı özür diler. |
| Xlsx | `6` | Office Open XML spreadsheetML çalışma kitabını veya şablonunu, makrolu ya da makrosuz, temsil eder. |
| Tsv | `11` | Sekme ile Ayrılmış Değerler (TSV) metin dosyası. |
| TSV | `11` | Sekme ile Ayrılmış Değerler (TSV) metin dosyası. NOT: Bu üye artık kullanımdan kaldırıldı. Bunun yerine lütfen Tsv özelliğini kullanın. Bu özellik Nisan 2021'den itibaren 6 ay sonra kaldırılacak. Aspose, yaşadığınız herhangi bir rahatsızlıktan dolayı özür diler. |
| TabDelimited | `11` | Sekme sınırlı bir metin dosyasını temsil eder, Tsv ile aynı. |
| Html | `12` | Bir html dosyasını temsil eder. |
| MHtml | `13` | Bir mhtml dosyasını temsil eder. |
| Ods | `14` | Open Document Sheet (ODS) dosyası. |
| ODS | `14` | Open Document Sheet (ODS) dosyası. NOT: Bu üye artık kullanımdan kaldırıldı. Bunun yerine lütfen Ods özelliğini kullanın. Bu özellik Nisan 2021'den itibaren 6 ay sonra kaldırılacak. Aspose, yaşadığınız herhangi bir rahatsızlıktan dolayı özür diler. |
| Excel97To2003 | `5` | Excel97-2003 xls dosyasını temsil eder. |
| SpreadsheetML | `15` | Excel 2003 xml dosyasını temsil eder. |
| Xlsb | `16` | xlsb dosyasını temsil eder. |
| Ots | `31` | Open Document Template Sheet (OTS) dosyası. |
| Numbers | `56` | Numbers dosyasını temsil eder. |
| Fods | `59` | OpenDocument Flat XML Spreadsheet (.fods) dosya formatını temsil eder. |
| FODS | `59` | OpenDocument Flat XML Spreadsheet (.fods) dosya formatını temsil eder. NOT: Bu üye artık kullanımdan kaldırıldı. Bunun yerine lütfen Fods özelliğini kullanın. Bu özellik Nisan 2021'den itibaren 6 ay sonra kaldırılacak. Aspose, yaşadığınız herhangi bir rahatsızlıktan dolayı özür diler. |
| Sxc | `60` | StarOffice Calc Spreadsheet (.sxc) dosya formatını temsil eder. |
| SXC | `60` | StarOffice Calc Spreadsheet (.sxc) dosya formatını temsil eder. NOT: Bu üye artık kullanımdan kaldırıldı. Bunun yerine lütfen Sxc özelliğini kullanın. Bu özellik Nisan 2021'den itibaren 6 ay sonra kaldırılacak. Aspose, yaşadığınız herhangi bir rahatsızlıktan dolayı özür diler. |
| Xml | `51` | Basit bir xml dosyasını temsil eder. |
| Epub | `52` | Bir EPUB dosyasını temsil eder. |
| Azw3 | `53` | AZW3 dosyasını temsil eder. |
| Chm | `54` | CHM dosyasını temsil eder. |
| Markdown | `55` | Markdown dosyasını temsil eder. |
| Unknown | `255` | Tanımlanamayan formatı temsil eder, yüklenemez. |
| Image | `254` | Görüntü |
| Json | `513` | Json |
| Dif | `30` | Veri Değişim Formatı. |
| Dbf | `515` | Xbase Veri dosyası |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class LoadFormatDemo
    {
        public static void LoadFormatExample()
        {
            // Aspose.Cells kullanarak farklı formatlarda bir Excel dosyası yükle
            string[] filePaths = {
                "LoadFormatDemo_original.xlsx",
                "LoadFormatDemo_original.xls",
                "LoadFormatDemo_original.csv",
                "LoadFormatDemo_original.json"
            };

            foreach (var filePath in filePaths)
            {
                // Dosya uzantısına göre yükleme formatını belirle
                LoadFormat loadFormat = GetLoadFormat(filePath);

                // Belirlenen LoadFormat ile LoadOptions oluştur
                LoadOptions loadOptions = new LoadOptions(loadFormat);

                // Belirtilen yükleme seçenekleriyle çalışma kitabını yükle
                Workbook workbook = new Workbook(filePath, loadOptions);

                // Çalışma kitabı üzerinde bazı işlemler gerçekleştir
                Console.WriteLine($"Loaded file: {filePath}");
                Console.WriteLine($"Number of sheets: {workbook.Worksheets.Count}");

                // Çalışma kitabını yeni bir dosyaya kaydet
                string outputFilePath = $"output_{System.IO.Path.GetFileName(filePath)}";
                workbook.Save(outputFilePath);
                Console.WriteLine($"Saved file as: {outputFilePath}");
            }
        }

        private static LoadFormat GetLoadFormat(string filePath)
        {
            string extension = System.IO.Path.GetExtension(filePath).ToLower();
            switch (extension)
            {
                case ".xlsx":
                    return LoadFormat.Xlsx;
                case ".xls":
                    return LoadFormat.Excel97To2003;
                case ".csv":
                    return LoadFormat.Csv;
                case ".json":
                    return LoadFormat.Json;
                default:
                    return LoadFormat.Auto;
            }
        }
    }

}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


