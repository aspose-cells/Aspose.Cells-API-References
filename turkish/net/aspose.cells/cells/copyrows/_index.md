---
title: "Cells.CopyRows"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Cells yöntemi. Bazı tam satırların veri ve biçimlerini kopyalar"
type: docs
url: /tr/net/aspose.cells/cells/copyrows/
---
## CopyRows(Cells, int, int, int) {#copyrows}

Bazı bütün satırların veri ve biçimlerini kopyalar.

```csharp
public void CopyRows(Cells sourceCells, int sourceRowIndex, int destinationRowIndex, int rowNumber)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| sourceCells | Hücreler | Kaynak Cells nesnesi, kopyalanacak veri ve biçimleri içerir. |
| sourceRowIndex | Int32 | Kaynak satır indeksi. |
| destinationRowIndex | Int32 | Hedef satır indeksi. |
| rowNumber | Int32 | Kopyalanan satır numarası. |

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodCopyRowsWithCellsInt32Int32Int32Demo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook destinationWorkbook = new Workbook();
            Workbook sourceWorkbook = new Workbook();

            // Kaynak çalışma kitabına bazı örnek veriler ekleyin
            Worksheet sourceSheet = sourceWorkbook.Worksheets[0];
            sourceSheet.Cells["A1"].PutValue("Source Data 1");
            sourceSheet.Cells["A2"].PutValue("Source Data 2");
            sourceSheet.Cells["A3"].PutValue("Source Data 3");

            // Her iki çalışma kitabından da hücreleri alın
            Cells destinationCells = destinationWorkbook.Worksheets[0].Cells;
            Cells sourceCells = sourceSheet.Cells;

            // Kaynaktan hedefe tüm satırları, hedefte satır 0'dan başlayarak kopyalayın
            destinationCells.CopyRows(sourceCells, 0, 0, sourceCells.MaxDisplayRange.RowCount);

            // Sonucu kaydet
            destinationWorkbook.Save("output.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## CopyRows(Cells, int, int, int, CopyOptions) {#copyrows_1}

Bazı bütün satırların veri ve biçimlerini kopyalar.

```csharp
public void CopyRows(Cells sourceCells, int sourceRowIndex, int destinationRowIndex, int rowNumber, 
    CopyOptions copyOptions)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| sourceCells | Hücreler | Kaynak Cells nesnesi, kopyalanacak veri ve biçimleri içerir. |
| sourceRowIndex | Int32 | Kaynak satır indeksi. |
| destinationRowIndex | Int32 | Hedef satır indeksi. |
| rowNumber | Int32 | Kopyalanan satır numarası. |
| copyOptions | CopyOptions | Kopyalama seçenekleri. |

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodCopyRowsWithCellsInt32Int32Int32CopyOptionDemo2
    {
        public static void Run()
        {
            // Örnek veri içeren bir çalışma kitabı oluşturun.
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Bazı örnek veriler ve köprüler ekleyin
            worksheet.Cells["A1"].PutValue("Source Data");
            worksheet.Cells["A4"].PutValue("Row 4 Data");
            worksheet.Hyperlinks.Add("A4", 1, 1, "https://www.example.com");

            // Satır 5'te boş bir satır ekleyin
            worksheet.Cells.InsertRows(5, 1);

            // Satır 4'ü Satır 5'e CopyOptions olmadan kopyala
            worksheet.Cells.CopyRows(worksheet.Cells, 4, 5, 1);
            Console.WriteLine("Hyperlinks count after copy without options: " + worksheet.Hyperlinks.Count);

            // Çalışma sayfasını sıfırla
            worksheet.Cells.ClearContents(0, 0, worksheet.Cells.MaxRow + 1, worksheet.Cells.MaxColumn + 1);
            worksheet.Hyperlinks.Clear();
            worksheet.Cells["A4"].PutValue("Row 4 Data");
            worksheet.Hyperlinks.Add("A4", 1, 1, "https://www.example.com");

            // Satır 5'te tekrar boş bir satır ekle
            worksheet.Cells.InsertRows(5, 1);

            // Satır 4'ü Satır 5'e CopyOptions ile kopyala
            CopyOptions options = new CopyOptions();
            options.ExtendToAdjacentRange = true;
            worksheet.Cells.CopyRows(worksheet.Cells, 4, 5, 1, options);
            Console.WriteLine("Hyperlinks count after copy with options: " + worksheet.Hyperlinks.Count);
        }
    }
}
```

### Ayrıca Bakınız

* class [CopyOptions](../../copyoptions/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## CopyRows(Cells, int, int, int, CopyOptions, PasteOptions) {#copyrows_2}

Bazı bütün satırların veri ve biçimlerini kopyalar.

```csharp
public void CopyRows(Cells sourceCells0, int sourceRowIndex, int destinationRowIndex, 
    int rowNumber, CopyOptions copyOptions, PasteOptions pasteOptions)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| sourceCells0 | Hücreler | Kaynak Cells nesnesi, kopyalanacak veri ve biçimleri içerir. |
| sourceRowIndex | Int32 | Kaynak satır indeksi. |
| destinationRowIndex | Int32 | Hedef satır indeksi. |
| rowNumber | Int32 | Kopyalanan satır numarası. |
| copyOptions | CopyOptions | Kopyalama seçenekleri. |
| pasteOptions | PasteOptions | yapıştırma seçenekleri. |

### Ayrıca Bakınız

* class [CopyOptions](../../copyoptions/)
* class [PasteOptions](../../pasteoptions/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


