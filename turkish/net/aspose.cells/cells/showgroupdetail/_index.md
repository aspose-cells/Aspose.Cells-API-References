---
title: "Cells.ShowGroupDetail"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Cells yöntemi. Gruplanmış satırları/sütunları genişletir"
type: docs
url: /tr/net/aspose.cells/cells/showgroupdetail/
---
## Cells.ShowGroupDetail method

Gruplanmış satırları/sütunları genişletir.

```csharp
public void ShowGroupDetail(bool isVertical, int index)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| isVertical | Boolean | Doğru, gruplandırılmış satırları genişletir. |
| indeks | Int32 | Satır/sütun indeksi |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsMethodShowGroupDetailWithBooleanInt32Demo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur ve ilk çalışma sayfasına eriş.
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // 5-7 satırlarına (sıfır tabanlı indeks 4-6) örnek veri doldur
            for (int row = 4; row <= 6; row++)
            {
                worksheet.Cells[row, 0].PutValue($"Row {row + 1}");
            }

            // 4-6 satırlarını (Excel satırları 5-7) grupla ve başlangıçta daralt
            worksheet.Cells.GroupRows(4, 6, true);

            try
            {
                // ShowGroupDetail kullanarak gruplandırılmış satırları genişlet (satırlar için isVertical: false, indeks: 4)
                worksheet.Cells.ShowGroupDetail(false, 4);
                Console.WriteLine("ShowGroupDetail method executed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing ShowGroupDetail: {ex.Message}");
            }

            // Etkiyi göstermek için çalışma kitabını kaydedin
            workbook.Save("ShowGroupDetailWithBooleanInt32Demo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


