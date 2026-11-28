---
title: "Cells.UngroupRows"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Cells yöntemi. Satırları gruplamadan çıkarır."
type: docs
url: /tr/net/aspose.cells/cells/ungrouprows/
---
## UngroupRows(int, int, bool) {#ungrouprows_1}

Satırların gruplamasını kaldırır.

```csharp
public void UngroupRows(int firstIndex, int lastIndex, bool isAll)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| firstIndex | Int32 | Gruplanması kaldırılacak ilk satır indeksi. |
| lastIndex | Int32 | Gruplanması kaldırılacak son satır indeksi. |
| isAll | Boolean | True, tüm gruplanmış bilgileri kaldırır. Aksi takdirde, dış grup bilgisini kaldırır. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsMethodUngroupRowsWithInt32Int32BooleanDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Demonstrasyon için iç içe satır gruplamaları oluşturun
            worksheet.Cells.GroupRows(5, 7);  // First level grouping
            worksheet.Cells.GroupRows(5, 7);  // Second level grouping

            try
            {
                // 5-7 satırların tüm seviyelerinin gruplamasını kaldırın
                worksheet.Cells.UngroupRows(5, 7, true);

                Console.WriteLine("Rows 5-7 successfully ungrouped with all levels removed");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing UngroupRows: {ex.Message}");
            }

            // Değiştirilmiş çalışma kitabını kaydet
            workbook.Save("UngroupRowsWithBooleanDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## UngroupRows(int, int) {#ungrouprows}

Satırların gruplamasını kaldırır.

```csharp
public void UngroupRows(int firstIndex, int lastIndex)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| firstIndex | Int32 | Gruplanması kaldırılacak ilk satır indeksi. |
| lastIndex | Int32 | Gruplanması kaldırılacak son satır indeksi. |

### Açıklamalar

Yalnızca dış grup bilgisini kaldırır.

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodUngroupRowsWithInt32Int32Demo
    {
        public static void Run()
        {
            // Bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Bazı verileri doldurun
            for (int i = 0; i < 6; i++)
            {
                cells[i, 0].PutValue($"Row {i}");
            }

            // Satırları 1'den 3'e (0 tabanlı indeks) gruplayın
            cells.GroupRows(1, 3, true);

            Console.WriteLine("Rows grouped from index 1 to 3");

            // Aynı satırların gruplamasını kaldırın
            cells.UngroupRows(1, 3);

            Console.WriteLine("Rows ungrouped from index 1 to 3");

            // Çalışma kitabını kaydedin
            workbook.Save("UngroupRowsDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


