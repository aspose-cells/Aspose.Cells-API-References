---
title: "DataSorter.Sort"
second_title: "Aspose.Cells için .NET API Referansı"
description: "DataSorter yöntemi. Alanın verilerini sıralar"
type: docs
url: /tr/net/aspose.cells/datasorter/sort/
---
## Sort(Cells, int, int, int, int) {#sort_2}

Alan verilerini sıralar.

```csharp
public int[] Sort(Cells cells, int startRow, int startColumn, int endRow, int endColumn)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| hücreler | Hücreler | Hücreler veri alanını içerir. |
| startRow | Int32 | Alanının başlangıç satırı. |
| startColumn | Int32 | Alanının başlangıç sütunu. |
| endRow | Int32 | Alanının son satırı. |
| endColumn | Int32 | Alanının son sütunu. |

### Dönüş Değeri

Sıralanan satırların/sütunların orijinal indeksleri (mutlak konum, örneğin sütun A 0, B 1, ...) . Bu sıralama işlemiyle taşınması gereken satır/sütun yoksa, null döndürülür.

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DataSorterMethodSortWithCellsInt32Int32Int32Int32Demo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Cells cells = wb.Worksheets[0].Cells;
            
            // Örnek verileri doldur
            for (int i = 0; i < 6; i++)
            {
                cells[i, 0].PutValue(6 - i);
            }
            
            // Gizli satırlarla sıralamayı göstermek için bir satırı gizleyin
            cells.Rows[1].IsHidden = true;
            
            // Sıralayıcıyı oluşturun ve yapılandırın
            DataSorter sorter = wb.DataSorter;
            sorter.AddKey(0, SortOrder.Ascending);
            
            // Cells ve Int32 parametreleriyle Sort yöntemini gösterin
            sorter.Sort(cells, 0, 0, 5, 0);
            
            // Sonuçları konsola yazdırın
            for (int i = 0; i < 6; i++)
            {
                Console.WriteLine($"Cell A{i+1}: {cells[i, 0].IntValue}");
            }
            Console.WriteLine($"Is row 2 hidden? {cells.Rows[1].IsHidden}");
        }
    }
}
```

### Ayrıca Bakınız

* class [Cells](../../cells/)
* class [DataSorter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Sort(Cells, CellArea) {#sort_1}

Alan verilerini sırala.

```csharp
public int[] Sort(Cells cells, CellArea area)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| hücreler | Hücreler | Hücreler veri alanını içerir. |
| alan | CellArea | Sıralama için gereken alan |

### Dönüş Değeri

Sıralanan satırların/sütunların orijinal indeksleri (mutlak konum, örneğin sütun A 0, B 1, ...) . Bu sıralama işlemiyle taşınması gereken satır/sütun yoksa, null döndürülür.

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DataSorterMethodSortWithCellsCellAreaDemo
    {
        public static void Run()
        {
            // Örnek veri içeren bir çalışma kitabı oluşturun.
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Örnek veri ekleyin.
            worksheet.Cells["A1"].PutValue("Year");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["A2"].PutValue(1995);
            worksheet.Cells["B2"].PutValue(10000);
            worksheet.Cells["A3"].PutValue(1996);
            worksheet.Cells["B3"].PutValue(15000);
            worksheet.Cells["A4"].PutValue(1997);
            worksheet.Cells["B4"].PutValue(12000);
            worksheet.Cells["A5"].PutValue(1998);
            worksheet.Cells["B5"].PutValue(18000);

            // Veri sıralayıcı oluştur
            DataSorter dataSorter = workbook.DataSorter;
            dataSorter.HasHeaders = true;
            dataSorter.Key1 = 0; // Sort by first column (Year)
            dataSorter.Order1 = SortOrder.Descending;

            // Sıralama alanını tanımla
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.StartColumn = 0;
            area.EndRow = 4;
            area.EndColumn = 1;

            // Sıralamayı gerçekleştir
            dataSorter.Sort(worksheet.Cells, area);

            // Çalışma kitabını kaydedin
            workbook.Save("SortedData.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Cells](../../cells/)
* struct [CellArea](../../cellarea/)
* class [DataSorter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Sort() {#sort}

Aralıktaki verileri sırala.

```csharp
public int[] Sort()
```

### Dönüş Değeri

Sıralanan satırların/sütunların orijinal indeksleri (mutlak konum, örneğin sütun A 0, B 1, ...) . Bu sıralama işlemiyle taşınması gereken satır/sütun yoksa, null döndürülür.

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DataSorterMethodSortDemo
    {
        public static void Run()
        {
            // Örnek veri içeren bir çalışma kitabı oluşturun.
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Sıralamak için örnek veri ekle
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("C");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue("A");
            worksheet.Cells["B3"].PutValue(10);
            worksheet.Cells["A4"].PutValue("B");
            worksheet.Cells["B4"].PutValue(20);

            // Bir tablo/list nesnesi oluştur
            int index = worksheet.ListObjects.Add(0, 0, 3, 1, true);
            Aspose.Cells.Tables.ListObject table = worksheet.ListObjects[index];
            table.ShowTotals = true;

            // Verileri ilk sütuna göre sırala
            table.AutoFilter.Sorter.Sort();

            // Çalışma kitabını kaydedin
            workbook.Save("SortedData.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Ayrıca Bakınız

* class [DataSorter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


