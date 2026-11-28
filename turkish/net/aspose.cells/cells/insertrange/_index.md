---
title: "Cells.InsertRange"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Cells yöntemi. Bir hücre aralığını ekler ve hücreleri kaydırma seçeneğine göre kaydırır"
type: docs
url: /tr/net/aspose.cells/cells/insertrange/
---
## InsertRange(CellArea, int, ShiftType, bool) {#insertrange_2}

Bir hücre aralığını ekler ve hücreleri kaydırma seçeneğine göre kaydırır.

```csharp
public void InsertRange(CellArea area, int shiftNumber, ShiftType shiftType, bool updateReference)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| alan | CellArea | Kaydırma alanı. |
| shiftNumber | Int32 | Eklenecek satır veya sütun sayısı. |
| shiftType | ShiftType | Hücreleri kaydırma seçeneği. |
| updateReference | Boolean | Diğer çalışma sayfalarındaki referansların güncellenip güncellenmeyeceğini gösterir. |

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodInsertRangeWithCellAreaInt32ShiftTypeBooleanDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Biraz örnek veri doldurun
            cells["A1"].PutValue("Header");
            cells["A2"].PutValue(100);
            cells["A3"].PutValue(200);

            // Eklenecek alanı tanımlayın (satırlar 2-3, sütun A)
            CellArea area = CellArea.CreateCellArea(1, 0, 2, 0);

            // Aralığı ekle, hücreleri sağa kaydır ve referansları güncelle
            cells.InsertRange(area, 1, ShiftType.Right, true);

            // Değerleri kontrol ederek işlemi doğrulayın
            Console.WriteLine("A2 value after insert: " + cells["A2"].StringValue);
            Console.WriteLine("B2 value after insert: " + cells["B2"].StringValue);
        }
    }
}
```

### Ayrıca Bakınız

* struct [CellArea](../../cellarea/)
* enum [ShiftType](../../shifttype/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## InsertRange(CellArea, ShiftType) {#insertrange}

Bir hücre aralığını ekler ve hücreleri kaydırma seçeneğine göre kaydırır.

```csharp
public void InsertRange(CellArea area, ShiftType shiftType)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| alan | CellArea | Kaydırma alanı. |
| shiftType | ShiftType | Hücreleri kaydırma seçeneği. |

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodInsertRangeWithCellAreaShiftTypeDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Bazı örnek veri doldurun
            for (int row = 0; row < 10; row++)
            {
                for (int col = 0; col < 5; col++)
                {
                    cells[row, col].PutValue($"R{row}C{col}");
                }
            }

            // Eklenecek hücre alanını tanımlayın
            CellArea area = new CellArea();
            area.StartRow = 2;
            area.EndRow = 4;
            area.StartColumn = 1;
            area.EndColumn = 3;

            // Aralığı ekle ve hücreleri aşağı kaydır
            cells.InsertRange(area, ShiftType.Down);

            // Çalışma kitabını kaydedin
            workbook.Save("InsertRangeDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* struct [CellArea](../../cellarea/)
* enum [ShiftType](../../shifttype/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## InsertRange(CellArea, int, ShiftType) {#insertrange_1}

Bir hücre aralığını ekler ve hücreleri kaydırma seçeneğine göre kaydırır.

```csharp
public void InsertRange(CellArea area, int shiftNumber, ShiftType shiftType)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| alan | CellArea | Kaydırma alanı. |
| shiftNumber | Int32 | Eklenecek satır veya sütun sayısı. |
| shiftType | ShiftType | Hücreleri kaydırma seçeneği. |

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodInsertRangeWithCellAreaInt32ShiftTypeDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Örnek veri ekleyin
            worksheet.Cells["A1"].PutValue("Original Data");
            worksheet.Cells["B1"].PutValue(100);
            worksheet.Cells["C1"].PutValue(200);
            
            // Eklenecek hücre alanını tanımlayın (tek hücre B1)
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.EndRow = 0;
            area.StartColumn = 1;
            area.EndColumn = 1;
            
            // Aralığı ekle, hücreleri sağa kaydır
            worksheet.Cells.InsertRange(area, 1, ShiftType.Right);
            
            // Çalışma kitabını kaydedin
            workbook.Save("InsertRangeDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* struct [CellArea](../../cellarea/)
* enum [ShiftType](../../shifttype/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


