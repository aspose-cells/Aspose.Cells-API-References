---
title: "CalculationCell.SetCalculatedValue"
second_title: "Aspose.Cells için .NET API Referansı"
description: "CalculationCell yöntemi. Hücre için hesaplanmış değeri ayarlar"
type: docs
url: /tr/net/aspose.cells/calculationcell/setcalculatedvalue/
---
## CalculationCell.SetCalculatedValue method

Hücre için hesaplanmış değeri ayarlar.

```csharp
public void SetCalculatedValue(object v)
```

### Açıklamalar

Kullanıcı, hücre için otomatik hesaplamayı yok saymak amacıyla bu yöntemle hesaplanmış sonucu ayarlayabilir.

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Reflection;

    public class CalculationCellMethodSetCalculatedValueWithObjectDemo
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

                // SetCalculatedValue yöntemi kullanarak bir hesaplanmış değer ayarla
                calcCell.SetCalculatedValue(42); // Using an integer value as the Object parameter

                // Hücre hakkında bilgiyi göster
                Console.WriteLine("Cell Row: " + calcCell.CellRow);
                Console.WriteLine("Cell Column: " + calcCell.CellColumn);
                Console.WriteLine("SetCalculatedValue method called successfully with value: 42");

                // Çalışma kitabını kaydedin
                workbook.Save("SetCalculatedValueDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling SetCalculatedValue: {ex.Message}");
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [CalculationCell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


