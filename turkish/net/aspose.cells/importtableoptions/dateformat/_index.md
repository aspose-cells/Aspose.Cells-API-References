---
title: "ImportTableOptions.DateFormat"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ImportTableOptions özelliği. İçe aktarılmış tarih‑zaman değerlerine sahip hücreler için tarih biçimi dizesini alır veya ayarlar"
type: docs
url: /tr/net/aspose.cells/importtableoptions/dateformat/
---
## ImportTableOptions.DateFormat property

İçe aktarılan tarih‑zaman değerlerine sahip hücreler için tarih biçimi dizesini alır veya ayarlar.

```csharp
public string DateFormat { get; set; }
```

### Örnekler

```csharp
using System;
using System.Data;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ImportTableOptionsPropertyDateFormatDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Tarih değerleri içeren örnek bir DataTable oluşturun
            DataTable dataTable = new DataTable();
            dataTable.Columns.Add("DateColumn", typeof(DateTime));
            dataTable.Rows.Add(new DateTime(2023, 1, 15));
            dataTable.Rows.Add(new DateTime(2023, 2, 20));
            dataTable.Rows.Add(new DateTime(2023, 3, 25));

            // İçe aktarma aralığını tanımlayın
            Aspose.Cells.Range range = worksheet.Cells.CreateRange(0, 0, 10, 1);

            // Özel tarih biçimiyle verileri içe aktar
            worksheet.Cells.ImportData(dataTable, 0, 0, new ImportTableOptions()
            {
                IsFieldNameShown = true,
                DateFormat = "YYYY-MM-DD"
            });

            // Sonucu göstermek için çalışma kitabını kaydet
            workbook.Save("DateFormatDemoOutput.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [ImportTableOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


