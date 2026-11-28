---
title: "Cells.DeleteRange"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Cells yöntemi. Bir hücre aralığını siler ve hücreleri kaydırma seçeneğine göre kaydırır."
type: docs
url: /tr/net/aspose.cells/cells/deleterange/
---
## Cells.DeleteRange method

Bir hücre aralığını siler ve hücreleri kaydırma seçeneğine göre kaydırır.

```csharp
public void DeleteRange(int startRow, int startColumn, int endRow, int endColumn, 
    ShiftType shiftType)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| startRow | Int32 | Başlangıç satır indeksi. |
| startColumn | Int32 | Başlangıç sütun indeksi. |
| endRow | Int32 | Bitiş satır indeksi. |
| endColumn | Int32 | Bitiş sütun indeksi. |
| shiftType | ShiftType | Hücreleri kaydırma seçeneği. |

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodDeleteRangeWithInt32Int32Int32Int32ShiftTypeDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Biraz örnek veri doldurun
            sheet.Cells["A1"].PutValue("A1");
            sheet.Cells["B1"].PutValue("B1");
            sheet.Cells["C1"].PutValue("C1");
            sheet.Cells["A2"].PutValue("A2");
            sheet.Cells["B2"].PutValue("B2");
            sheet.Cells["C2"].PutValue("C2");

            // Aralığı sil ve sola kaydır.
            sheet.Cells.DeleteRange(0, 1, 1, 2, ShiftType.Left);

            // Çalışma kitabını kaydedin
            workbook.Save("DeleteRangeExample.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* enum [ShiftType](../../shifttype/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


