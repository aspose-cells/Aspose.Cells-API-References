---
title: "Cells.CopyColumns"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Cells yöntemi. Bir bütün sütunun veri ve biçimlerini kopyalar"
type: docs
url: /tr/net/aspose.cells/cells/copycolumns/
---
## CopyColumns(Cells, int, int, int, PasteOptions) {#copycolumns_1}

Bir bütün sütunun veri ve biçimlerini kopyalar.

```csharp
public void CopyColumns(Cells sourceCells, int sourceColumnIndex, int destinationColumnIndex, 
    int columnNumber, PasteOptions pasteOptions)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| sourceCells | Hücreler | Kaynak Cells nesnesi, kopyalanacak veri ve biçimleri içerir. |
| sourceColumnIndex | Int32 | Kaynak sütun indeksi. |
| destinationColumnIndex | Int32 | Hedef sütun indeksi. |
| columnNumber | Int32 | Kopyalanan sütun numarası. |
| pasteOptions | PasteOptions | yapıştırma seçenekleri. |

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodCopyColumnsWithCellsInt32Int32Int32PasteOptioDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Çalışma sayfasına örnek veri ekle
            worksheet.Cells["A1"].PutValue("Header1");
            worksheet.Cells["B1"].PutValue("Header2");
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["B2"].PutValue(200);

            // Başka bir çalışma kitabını hedef olarak oluştur
            Workbook destWorkbook = new Workbook();
            Worksheet destWorksheet = destWorkbook.Worksheets[0];

            // Sütunları yalnızca biçimlendirme ile kopyala
            try
            {
                destWorksheet.Cells.CopyColumns(
                    worksheet.Cells, 
                    0, // source column index
                    0, // destination column index
                    2, // column count (copy 2 columns)
                    new PasteOptions() { PasteType = PasteType.Formats });
                
                Console.WriteLine("Columns copied successfully with formatting only.");
            }
            catch (Exception ex)
            {
                Console.WriteLine("Error copying columns: " + ex.Message);
            }

            // Çalışma kitabını kaydedin
            workbook.Save("CopyColumnsDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [PasteOptions](../../pasteoptions/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## CopyColumns(Cells, int, int, int) {#copycolumns}

Bütün sütunların veri ve biçimlerini kopyalar.

```csharp
public void CopyColumns(Cells sourceCells, int sourceColumnIndex, int destinationColumnIndex, 
    int columnNumber)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| sourceCells | Hücreler | Kaynak Cells nesnesi, kopyalanacak veri ve biçimleri içerir. |
| sourceColumnIndex | Int32 | Kaynak sütun indeksi. |
| destinationColumnIndex | Int32 | Hedef sütun indeksi. |
| columnNumber | Int32 | Kopyalanan sütun numarası. |

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodCopyColumnsWithCellsInt32Int32Int32Demo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook wb = new Workbook();
            Worksheet worksheet = wb.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Sütunlara örnek veri ekle
            cells["A1"].PutValue("Source1");
            cells["B1"].PutValue("Source2");
            cells["C1"].PutValue("Source3");
            cells["D1"].PutValue("Source4");
            cells["E1"].PutValue("Source5");

            // Sütunları 1 (B) indeksinden 3 (D) indeksine kopyala, 1 sütun kopyala
            cells.CopyColumns(cells, 1, 3, 1);

            // Çalışma kitabını kaydedin
            wb.Save("output.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## CopyColumns(Cells, int, int, int, int) {#copycolumns_2}

Tüm sütunların veri ve biçimlerini kopyalar.

```csharp
public void CopyColumns(Cells sourceCells, int sourceColumnIndex, int sourceTotalColumns, 
    int destinationColumnIndex, int destinationTotalColumns)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| sourceCells | Hücreler | Kaynak Cells nesnesi, kopyalanacak veri ve biçimleri içerir. |
| sourceColumnIndex | Int32 | Kaynak sütun indeksi. |
| sourceTotalColumns | Int32 | Kaynak sütunların sayısı. |
| destinationColumnIndex | Int32 | Hedef sütun indeksi. |
| destinationTotalColumns | Int32 | Hedef sütunların sayısı. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsMethodCopyColumnsWithCellsInt32Int32Int32Int32Demo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Kaynak sütunları doldur (sütunlar 0 ve 1)
            cells[0, 0].Value = "Header 1";
            cells[0, 1].Value = "Header 2";
            for (int row = 1; row <= 4; row++)
            {
                cells[row, 0].Value = row * 100;
                cells[row, 1].Value = row * 200;
            }

            try
            {
                // 0 indeksinden hedef 3 indeksine 2 sütun kopyala, 2 sütun ekle
                cells.CopyColumns(cells, 0, 2, 3, 2);
                
                Console.WriteLine("Copied 2 source columns to destination position successfully");
                
                // Kopyayı, hedef sütunları (3 ve 4) kontrol ederek doğrula
                Console.WriteLine($"Destination column 3 value: {cells[0, 3].StringValue}");
                Console.WriteLine($"Destination column 4 value: {cells[0, 4].StringValue}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing CopyColumns: {ex.Message}");
            }

            // Değiştirilmiş çalışma kitabını kaydet
            workbook.Save("CellsMethodCopyColumnsWithCellsInt32Int32Int32Int32Demo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


