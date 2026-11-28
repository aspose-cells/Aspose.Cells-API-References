---
title: "Cells.UnhideColumn"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Cells yöntemi. Bir sütunun gizliliğini kaldırır"
type: docs
url: /tr/net/aspose.cells/cells/unhidecolumn/
---
## Cells.UnhideColumn method

Bir sütunu gösterir.

```csharp
public void UnhideColumn(int column, double width)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| sütun | Int32 | Sütun indeksi. |
| genişlik | Double | Sütun genişliği. |

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodUnhideColumnWithInt32DoubleDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            
            // Sütun 2'yi gizle
            cells.HideColumn(2);
            
            // Sütun 2'yi genişlik ayarıyla göster (-1, standart genişliği kullanmak anlamına gelir)
            cells.UnhideColumn(2, -1);
            
            Console.WriteLine("Column 2 width after unhiding: " + cells.Columns[2].Width);
        }
    }
}
```

### Ayrıca Bakınız

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


