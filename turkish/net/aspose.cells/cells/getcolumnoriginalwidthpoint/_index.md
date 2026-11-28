---
title: "Cells.GetColumnOriginalWidthPoint"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Cells yöntemi. Sütun gizli ise, orijinal sütun yüksekliğini nokta biriminde alır"
type: docs
url: /tr/net/aspose.cells/cells/getcolumnoriginalwidthpoint/
---
## Cells.GetColumnOriginalWidthPoint method

Sütun gizli ise, orijinal sütun yüksekliğini nokta biriminde alır

```csharp
[Obsolete("Use Cells.GetColumnWidth(int ,bool , CellsUnitType ) method, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public double GetColumnOriginalWidthPoint(int column)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| sütun | Int32 | Satır indeksi. |

### Dönüş Değeri

Normal görünümde sütunun genişliği.

### Açıklamalar

NOT: Bu yöntem artık kullanımdan kaldırılmıştır. Bunun yerine lütfen Cells.GetColumnWidth(int ,bool , CellsUnitType ) yöntemini kullanın. Bu yöntem, Nisan 2024'ten itibaren 12 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsMethodGetColumnOriginalWidthPointWithInt32Demo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Sütun indeks parametresini hazırla
            int columnIndex = 0;

            try
            {
                // Orijinal sütun genişliğini nokta cinsinden al
                double originalWidth = cells.GetColumnOriginalWidthPoint(columnIndex);
                Console.WriteLine($"Original width of column {columnIndex}: {originalWidth} points");

                // Sütun genişliğini değiştir
                cells.SetColumnWidth(columnIndex, 15);
                Console.WriteLine("Set new column width to 15 points");

                // Orijinal genişliği tekrar alarak değişmediğini göster
                double unchangedWidth = cells.GetColumnOriginalWidthPoint(columnIndex);
                Console.WriteLine($"Original width remains: {unchangedWidth} points");

                // Mevcut genişliği alarak değişikliği göster
                double currentWidth = cells.GetColumnWidth(columnIndex);
                Console.WriteLine($"Current column width: {currentWidth} points");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetColumnOriginalWidthPoint method: {ex.Message}");
            }

            // Değiştirilmiş çalışma kitabını kaydet
            workbook.Save("GetColumnOriginalWidthPointDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


