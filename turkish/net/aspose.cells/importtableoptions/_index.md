---
title: "Sınıf ImportTableOptions"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.ImportTableOptions sınıfı. Hücrelere veri içe aktarma seçeneklerini temsil eder"
type: docs
url: /tr/net/aspose.cells/importtableoptions/
---
## ImportTableOptions class

Verilerin hücrelere içe aktarılması seçeneklerini temsil eder.

```csharp
public class ImportTableOptions
```

## Yapıcılar

| Ad | Açıklama |
| --- | --- |
| [ImportTableOptions](importtableoptions/)() | Varsayılan içe aktarma seçeneklerini oluşturur. |

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [CheckMergedCells](../../aspose.cells/importtableoptions/checkmergedcells/) { get; set; } | Birleştirilmiş hücrelerin kontrol edilip edilmediğini belirtir. |
| [ColumnIndexes](../../aspose.cells/importtableoptions/columnindexes/) { get; set; } | Veri kaynağından içe aktarılacak sütunları (0 tabanlı) alır veya ayarlar. null, tüm sütunların içe aktarılması gerektiği anlamına gelir. |
| [ConvertGridStyle](../../aspose.cells/importtableoptions/convertgridstyle/) { get; set; } | Izgara görünümünün stilinin hücrelere uygulanıp uygulanmayacağını belirtir. |
| [ConvertNumericData](../../aspose.cells/importtableoptions/convertnumericdata/) { get; set; } | Dize değerinin sayısal veya tarih değerine dönüştürülüp dönüştürülmeyeceğini gösteren bir değeri alır veya ayarlar. |
| [DateFormat](../../aspose.cells/importtableoptions/dateformat/) { get; set; } | İçe aktarılan tarih‑zaman değerlerine sahip hücreler için tarih biçimi dizesini alır veya ayarlar. |
| [DefaultValues](../../aspose.cells/importtableoptions/defaultvalues/) { get; set; } | Tablodaki değer için varsayılan değer null'dur. |
| [ExportCaptionAsFieldName](../../aspose.cells/importtableoptions/exportcaptionasfieldname/) { get; set; } | Başlığın alan adı olarak dışa aktarılıp aktarılmayacağını gösterir. |
| [InsertRows](../../aspose.cells/importtableoptions/insertrows/) { get; set; } | Veri kayıtlarını içe aktarmak için yeni satırların eklenip eklenmeyeceğini gösterir. |
| [IsFieldNameShown](../../aspose.cells/importtableoptions/isfieldnameshown/) { get; set; } | Alan adının içe aktarılıp aktarılmayacağını gösterir. |
| [IsFormulas](../../aspose.cells/importtableoptions/isformulas/) { get; set; } | Verilerin formül olup olmadığını gösterir. |
| [IsHtmlString](../../aspose.cells/importtableoptions/ishtmlstring/) { get; set; } | Değerin html etiketleri içerip içermediğini gösterir. |
| [NumberFormats](../../aspose.cells/importtableoptions/numberformats/) { get; set; } | Sayı biçimlerini alır veya ayarlar |
| [ShiftFirstRowDown](../../aspose.cells/importtableoptions/shiftfirstrowdown/) { get; set; } | Satır eklerken ilk satırın aşağı kaydırılıp kaydırılmayacağını gösterir. |
| [Styles](../../aspose.cells/importtableoptions/styles/) { get; set; } | Tablonun her sütunu için stilleri alır ve ayarlar. |
| [TotalColumns](../../aspose.cells/importtableoptions/totalcolumns/) { get; set; } | Veri kaynağından içe aktarılacak toplam sütun sayısını alır veya ayarlar. -1, verilen veri kaynağının tüm satırları anlamına gelir. |
| [TotalRows](../../aspose.cells/importtableoptions/totalrows/) { get; set; } | Veri kaynağından içe aktarılacak toplam satır sayısını alır veya ayarlar. -1, verilen veri kaynağının tüm satırları anlamına gelir. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Data;

    public class ImportTableOptionsDemo
    {
        public static void ImportTableOptionsExample()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // İçe aktarılacak bir DataTable oluştur
            DataTable dataTable = new DataTable("SampleData");
            dataTable.Columns.Add("ID", typeof(int));
            dataTable.Columns.Add("Name", typeof(string));
            dataTable.Columns.Add("Date", typeof(DateTime));
            dataTable.Rows.Add(1, "John Doe", DateTime.Now);
            dataTable.Rows.Add(2, "Jane Smith", DateTime.Now.AddDays(1));

            // ImportTableOptions örneği oluştur
            ImportTableOptions importOptions = new ImportTableOptions
            {
                ConvertGridStyle = true,
                ConvertNumericData = true,
                InsertRows = true,
                ShiftFirstRowDown = false,
                IsFieldNameShown = true,
                ExportCaptionAsFieldName = false,
                DateFormat = "yyyy-MM-dd",
                TotalRows = -1, // Import all rows
                TotalColumns = -1, // Import all columns
                IsHtmlString = false,
                CheckMergedCells = false
            };

            // DataTable'ı çalışma sayfasına aktar
            worksheet.Cells.ImportData(dataTable, 0, 0, importOptions);

            // Çalışma kitabını kaydedin
            workbook.Save("ImportTableOptionsExample.xlsx");
            workbook.Save("ImportTableOptionsExample.pdf");
            return;
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


