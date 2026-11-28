---
title: "Sınıf ExportTableOptions"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.ExportTableOptions sınıfı. Tüm dışa aktarma tablo seçeneklerini temsil eder"
type: docs
url: /tr/net/aspose.cells/exporttableoptions/
---
## ExportTableOptions class

Tüm dışa aktarma tablo seçeneklerini temsil eder.

```csharp
public class ExportTableOptions
```

## Yapıcılar

| Ad | Açıklama |
| --- | --- |
| [ExportTableOptions](exporttableoptions/)() | Varsayılan yapıcı. |

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [AllowDBNull](../../aspose.cells/exporttableoptions/allowdbnull/) { get; set; } | Bu değer, bu tabloda DBNull'ların izin verilip verilmediğini gösterir. |
| [CheckMixedValueType](../../aspose.cells/exporttableoptions/checkmixedvaluetype/) { get; set; } | False, Aspose.Cells performans için DataColumn'un tipini ilk satırın değer tipine göre ayarlar. True, Aspose.Cells DataColumn'un tipini ayarlamadan önce sütundaki değer tiplerinin karışık olup olmadığını kontrol eder ve değer tipleri karışık ise DataColumn'un tipi string olacaktır. |
| [DataTable](../../aspose.cells/exporttableoptions/datatable/) { get; set; } | Sütunların veri tipi atanan DataTable'ı alır ve ayarlar. |
| [ExportAsHtmlString](../../aspose.cells/exporttableoptions/exportashtmlstring/) { get; set; } | Hücrelerin HTML dize değerini DataTable'a dışa aktarır. |
| [ExportAsString](../../aspose.cells/exporttableoptions/exportasstring/) { get; set; } | Hücrelerin dize değerini DataTable'a dışa aktarır. |
| [ExportColumnName](../../aspose.cells/exporttableoptions/exportcolumnname/) { get; set; } | İlk satırdaki verilerin DataTable'ın sütun adı olarak dışa aktarılıp aktarılmayacağını gösterir. Varsayılan değer false'tur. |
| [FormatStrategy](../../aspose.cells/exporttableoptions/formatstrategy/) { get; set; } | Değeri dize olarak dışa aktarırken kullanılan biçim stratejisini alır ve ayarlar. |
| [Indexes](../../aspose.cells/exporttableoptions/indexes/) { get; set; } | Dışa aktarılması gereken sütunların/satırların indeksleri. |
| [IsVertical](../../aspose.cells/exporttableoptions/isvertical/) { get; set; } | Workbook dosyasındaki bir satır DataTable'da bir satırı temsil ediyorsa true. Workbook dosyasındaki bir sütun DataTable'da bir satırı temsil ediyorsa false. |
| [PlotVisibleCells](../../aspose.cells/exporttableoptions/plotvisiblecells/) { get; set; } | Yalnızca görünen hücreleri dışa aktarır. |
| [PlotVisibleColumns](../../aspose.cells/exporttableoptions/plotvisiblecolumns/) { get; set; } | Yalnızca görünen sütunları dışa aktarır. |
| [PlotVisibleRows](../../aspose.cells/exporttableoptions/plotvisiblerows/) { get; set; } | Yalnızca görünen satırları dışa aktarır. |
| [RenameStrategy](../../aspose.cells/exporttableoptions/renamestrategy/) { get; set; } | Sütunların yinelenen adları için strateji. |
| [SkipErrorValue](../../aspose.cells/exporttableoptions/skiperrorvalue/) { get; set; } | Sütun için geçersiz değerin atlanıp atlanmayacağını gösterir. Örneğin, sütun tipi decimal ise ve değer decimal.MaxValue'dan büyükse ve bu özellik true ise, tekrar istisna fırlatmayacağız. Varsayılan değer false'tur. |

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| virtual [PreprocessExportedValue](../../aspose.cells/exporttableoptions/preprocessexportedvalue/)(int, int, CellValue) | Dışa aktarılacak mevcut hücrenin değerini ön işleme tabi tut. |

### Açıklamalar

Dışa aktarma ile ilgili hata değerlerini yok sayma gibi özel gereksinimler varsa, kullanıcı bu sınıfı genişleterek ilgili API'leri geçersiz kılarak hedefe ulaşabilir.

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Data;

    public class ExportTableOptionsDemo
    {
        public static void ExportTableOptionsExample()
        {
            // Yeni bir çalışma kitabı oluşturun ve ilk çalışma sayfasını alın.
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Çalışma sayfasına bazı örnek veriler ekleyin
            worksheet.Cells[0, 0].PutValue("Name");
            worksheet.Cells[0, 1].PutValue("Age");
            worksheet.Cells[1, 0].PutValue("John");
            worksheet.Cells[1, 1].PutValue(30);
            worksheet.Cells[2, 0].PutValue("Jane");
            worksheet.Cells[2, 1].PutValue(25);

            // ExportTableOptions bir örnek oluşturun
            ExportTableOptions exportOptions = new ExportTableOptions
            {
                ExportColumnName = true,
                SkipErrorValue = true,
                PlotVisibleCells = true,
                PlotVisibleRows = true,
                PlotVisibleColumns = true,
                ExportAsString = false,
                ExportAsHtmlString = false,
                FormatStrategy = CellValueFormatStrategy.DisplayStyle,
                CheckMixedValueType = true,
                AllowDBNull = true,
                IsVertical = true,
                RenameStrategy = RenameStrategy.Digit
            };

            // Çalışma sayfasındaki verileri bir DataTable'a dışa aktar
            DataTable dataTable = worksheet.Cells.ExportDataTable(0, 0, 3, 2, exportOptions);

            // Dışa aktarılan verileri görüntüle
            foreach (DataRow row in dataTable.Rows)
            {
                foreach (var item in row.ItemArray)
                {
                    Console.Write(item + "\t");
                }
                Console.WriteLine();
            }

            // Çalışma kitabını kaydedin
            workbook.Save("ExportTableOptionsExample.xlsx");
            workbook.Save("ExportTableOptionsExample.pdf");
        }
    }

}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


