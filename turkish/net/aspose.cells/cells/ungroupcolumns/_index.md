---
title: "Cells.UngroupColumns"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Cells yöntemi. Sütunları gruptan çıkarır"
type: docs
url: /tr/net/aspose.cells/cells/ungroupcolumns/
---
## Cells.UngroupColumns method

Sütunların gruplamasını kaldırır.

```csharp
public void UngroupColumns(int firstIndex, int lastIndex)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| firstIndex | Int32 | Grup dışı bırakılacak ilk sütun indeksi. |
| lastIndex | Int32 | Grup dışı bırakılacak son sütun indeksi. |

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodUngroupColumnsWithInt32Int32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Gruplamayı göstermek için önce sütunları gruplayın
            worksheet.Cells.GroupColumns(0, 2);

            // Sütunları gruptan çıkar (0'dan 2'ye)
            worksheet.Cells.UngroupColumns(0, 2);

            workbook.Save("output.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


