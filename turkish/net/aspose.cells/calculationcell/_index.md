---
title: "Sınıf CalculationCell"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.CalculationCell sınıfı. Hesaplanan bir hücre hakkında hesaplamayla ilgili verileri temsil eder"
type: docs
url: /tr/net/aspose.cells/calculationcell/
---
## CalculationCell class

Hesaplanan bir hücreyle ilgili hesaplama verilerini temsil eder.

```csharp
public class CalculationCell
```

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [Cell](../../aspose.cells/calculationcell/cell/) { get; } | Hesaplanan Cell nesnesini alır. |
| [CellColumn](../../aspose.cells/calculationcell/cellcolumn/) { get; } | Hücrenin sütun indeksini alır. |
| [CellRow](../../aspose.cells/calculationcell/cellrow/) { get; } | Hücrenin satır indeksini alır. |
| [Workbook](../../aspose.cells/calculationcell/workbook/) { get; } | Workbook nesnesini alır. |
| [Worksheet](../../aspose.cells/calculationcell/worksheet/) { get; } | Hücrenin bulunduğu Worksheet nesnesini alır. |

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| [SetCalculatedValue](../../aspose.cells/calculationcell/setcalculatedvalue/)(object) | Hücre için hesaplanmış değeri ayarlar. |

### Açıklamalar

Kullanıcı, formül hesaplama sürecinde Workbook'taki herhangi bir veriyi değiştirmemelidir, aksi takdirde beklenmeyen sonuçlar veya Exception oluşabilir. Bu nedenle, bu sınıf tarafından sağlanan tüm nesneler (örneğin [`Cell`](./cell/) nesnesi) yalnızca "okuma" amacıyla kullanılmalıdır.

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Reflection;

    public class CellsClassCalculationCellDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluşturun ve ilk çalışma sayfasını alın.
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Örnek veri ekleyin
            worksheet.Cells["A1"].Value = 10;
            worksheet.Cells["B1"].Formula = "=A1*2";

            try
            {
                // Yapıcı erişime açık olmadığından, yansıma kullanarak CalculationCell örneği oluştur.
                CalculationCell calcCell = (CalculationCell)Activator.CreateInstance(
                    typeof(CalculationCell),
                    BindingFlags.NonPublic | BindingFlags.Instance,
                    null,
                    new object[] { workbook, worksheet, 0, 1, worksheet.Cells["B1"] },
                    null);

                // Temel özellikleri göster
                Console.WriteLine($"Cell Row: {calcCell.CellRow}");
                Console.WriteLine($"Cell Column: {calcCell.CellColumn}");
                Console.WriteLine($"Cell Value: {calcCell.Cell.Value}");
                Console.WriteLine($"Workbook Name: {calcCell.Workbook.FileName}");
                Console.WriteLine($"Worksheet Name: {calcCell.Worksheet.Name}");

                // Çalışma kitabını kaydedin
                workbook.Save("CalculationCellDemo.xlsx");
                Console.WriteLine("CalculationCell demonstration completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


