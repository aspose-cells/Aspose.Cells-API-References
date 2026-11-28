---
title: "Cells.GroupRows"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Cells yöntemi. Satırları gruplar"
type: docs
url: /tr/net/aspose.cells/cells/grouprows/
---
## GroupRows(int, int, bool) {#grouprows_1}

Satırları gruplar.

```csharp
public void GroupRows(int firstIndex, int lastIndex, bool isHidden)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| firstIndex | Int32 | Gruplanacak ilk satır indeksi. |
| lastIndex | Int32 | Gruplanacak son satır indeksi. |
| isHidden | Boolean | Gruplanan satırların gizli olup olmadığını belirtir. |

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodGroupRowsWithInt32Int32BooleanDemo
    {
        public static void Run()
        {
            // Bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Bazı verileri doldurun
            for (int i = 0; i < 10; i++)
            {
                cells[i, 0].PutValue($"Group {i + 1}");
                for (int j = 1; j <= 5; j++)
                {
                    cells[i, j].PutValue($"Data {j}");
                }
            }

            // Satırları 1'den 5'e (0 tabanlı indeks) gruplayın ve gizleyin
            cells.GroupRows(1, 5, true);

            // Grubun altına özet satırı ayarla
            worksheet.Outline.SummaryRowBelow = false;

            // Çalışma kitabını kaydedin
            workbook.Save("GroupRowsDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GroupRows(int, int) {#grouprows}

Satırları gruplar.

```csharp
public void GroupRows(int firstIndex, int lastIndex)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| firstIndex | Int32 | Gruplanacak ilk satır indeksi. |
| lastIndex | Int32 | Gruplanacak son satır indeksi. |

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodGroupRowsWithInt32Int32Demo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Biraz örnek veri doldurun
            for (int i = 0; i < 10; i++)
            {
                cells[i, 0].PutValue("Row " + (i + 1));
            }

            // Satırları 2'den 5'e (sıfır tabanlı indeks) gruplayın
            cells.GroupRows(1, 4);

            // Çalışma kitabını kaydedin
            workbook.Save("GroupRowsExample.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


