---
title: "Cells.UnhideColumns"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Cells yöntemi. Birden fazla sütunu gizlemeyi kaldırır"
type: docs
url: /tr/net/aspose.cells/cells/unhidecolumns/
---
## Cells.UnhideColumns method

Birden çok sütunu gösterir.

```csharp
public void UnhideColumns(int column, int totalColumns, double width)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| sütun | Int32 | Sütun indeksi. |
| totalColumns | Int32 | Sütun numarası |
| genişlik | Double | Sütun genişliği. |

### Açıklamalar

Sütun genişliğini yalnızca gizli sütunlara uygular.

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsMethodUnhideColumnsWithInt32Int32DoubleDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur ve ilk çalışma sayfasına eriş.
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Başlangıçta 1-3 sütunlarını (sıfır tabanlı) gizle
            worksheet.Cells.HideColumns(1, 3);

            try
            {
                // 1. indeksten (ikinci sütun) başlayan, 3 sütun genişliğinde sütunların gizlemeyi kaldır, genişliği 15.5 olarak ayarla
                worksheet.Cells.UnhideColumns(1, 3, 15.5);

                // Gizlemeyi kaldırılan sütunların genişliğini kontrol ederek doğrulayın
                Console.WriteLine($"Column 1 width after unhiding: {worksheet.Cells.GetColumnWidth(1)}");
                Console.WriteLine("Columns 1-3 successfully unhidden with specified width");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing UnhideColumns: {ex.Message}");
            }

            // Değiştirilmiş çalışma kitabını kaydet
            workbook.Save("UnhideColumnsWithWidthDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


