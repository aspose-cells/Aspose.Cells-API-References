---
title: "Cells.HideColumns"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Cells yöntemi. Birden fazla sütunu gizle"
type: docs
url: /tr/net/aspose.cells/cells/hidecolumns/
---
## Cells.HideColumns method

Birden fazla sütunu gizler.

```csharp
public void HideColumns(int column, int totalColumns)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| sütun | Int32 | Sütun indeksi. |
| totalColumns | Int32 | Sütun numarası. |

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodHideColumnsWithInt32Int32Demo
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
                for (int j = 0; j < 10; j++)
                {
                    cells[i, j].PutValue($"Data {i},{j}");
                }
            }

            // Sütun 3'ten 5'e kadar gizle (sıfır tabanlı indeks)
            int startColumn = 2; // Column C
            int columnCount = 3;  // Hide 3 columns
            cells.HideColumns(startColumn, columnCount);

            // Çalışma kitabını kaydedin
            workbook.Save("HideColumnsDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Ayrıca Bakınız

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


