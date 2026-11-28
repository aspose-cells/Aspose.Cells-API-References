---
title: "ExportTableOptions.CheckMixedValueType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ExportTableOptions özelliği. False ise Aspose.Cells, performans için DataColumns türünü ilk satırın değer türüne göre ayarlar. True ise Aspose.Cells, DataColumns türünü ayarlamadan önce sütundaki değer türlerinin karışık olup olmadığını kontrol eder ve değer türleri karışık ise DataColumns türü string olur"
type: docs
url: /tr/net/aspose.cells/exporttableoptions/checkmixedvaluetype/
---
## ExportTableOptions.CheckMixedValueType property

False, Aspose.Cells performans için DataColumn'un tipini ilk satırın değer tipine göre ayarlar. True, Aspose.Cells DataColumn'un tipini ayarlamadan önce sütundaki değer tiplerinin karışık olup olmadığını kontrol eder ve değer tipleri karışık ise DataColumn'un tipi string olacaktır.

```csharp
public bool CheckMixedValueType { get; set; }
```

### Örnekler

```csharp
using System;
using System.Data;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ExportTableOptionsPropertyCheckMixedValueTypeDemo
    {
        public static void Run()
        {
            // Örnek veri içeren bir çalışma kitabı oluşturun.
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Başlıkları ekle
            worksheet.Cells["A1"].PutValue("ID");
            worksheet.Cells["B1"].PutValue("Value Date");

            // Karışık tiplerde örnek veri ekle
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["B2"].PutValue(DateTime.Now);
            worksheet.Cells["A3"].PutValue(2.5);
            worksheet.Cells["B3"].PutValue("2023-01-15");
            worksheet.Cells["A4"].PutValue("3");
            worksheet.Cells["B4"].PutValue(DateTime.Now.AddDays(1));

            // CheckMixedValueType etkinleştirilmiş dışa aktarma seçenekleri oluştur
            ExportTableOptions options = new ExportTableOptions
            {
                CheckMixedValueType = true,
                ExportColumnName = true
            };

            // Verileri DataTable'a dışa aktar
            DataTable dataTable = worksheet.Cells.ExportDataTable(0, 0, 4, 2, options);

            // Sonuçları göster
            Console.WriteLine("Columns: " + dataTable.Columns.Count);
            Console.WriteLine("Rows: " + dataTable.Rows.Count);
            Console.WriteLine("ID column type: " + dataTable.Columns["ID"].DataType);
            Console.WriteLine("Value Date column type: " + dataTable.Columns["Value Date"].DataType);
        }
    }
}
```

### Ayrıca Bakınız

* class [ExportTableOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


