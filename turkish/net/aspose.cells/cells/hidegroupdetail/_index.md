---
title: "Cells.HideGroupDetail"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Cells metodu. Gruplandırılmış satırları/sütunları daraltır"
type: docs
url: /tr/net/aspose.cells/cells/hidegroupdetail/
---
## Cells.HideGroupDetail method

Gruplanmış satırları/sütunları daraltır.

```csharp
public void HideGroupDetail(bool isVertical, int index)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| isVertical | Boolean | True, gruplandırılmış satırları daralt. |
| indeks | Int32 | Satır/sütun indeksi |

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodHideGroupDetailWithBooleanInt32Demo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Satırları grupla ve detayları gizle
            worksheet.Cells.GroupRows(0, 9, false);
            worksheet.Cells.HideGroupDetail(true, 4);
            worksheet.Cells.HideGroupDetail(true, 7);

            // Çalışma kitabını kaydedin
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


