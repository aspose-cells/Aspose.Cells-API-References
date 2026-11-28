---
title: "Shape.FitToTextSize"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Shape yöntemi. Tüm metin içeriğini gösterecek şekilde uygun bir metin alanını yeniden hesaplayın"
type: docs
url: /tr/net/aspose.cells.drawing/shape/fittotextsize/
---
## Shape.FitToTextSize method

Tüm metin içeriğini gösterecek şekilde uygun bir metin alanını yeniden hesapla.

```csharp
public void FitToTextSize()
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ShapeMethodFitToTextSizeDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Bir metin kutusu şekli ekle
            Shape textBox = worksheet.Shapes.AddTextBox(1, 0, 1, 0, 100, 100);
            textBox.Text = "This is a sample text that will demonstrate the FitToTextSize method functionality.";

            try
            {
                // Orijinal boyutları göster
                Console.WriteLine($"Original Width: {textBox.Width}, Height: {textBox.Height}");

                // FitToTextSize yöntemini çağırın
                textBox.FitToTextSize();

                // Ayarlanmış boyutları göster
                Console.WriteLine($"Adjusted Width: {textBox.Width}, Height: {textBox.Height}");
                Console.WriteLine("FitToTextSize method executed successfully");

                // Etkiyi göstermek için daha fazla metin ekleyin
                textBox.Text += " Adding more text to show how the shape adjusts to fit the content.";
                textBox.FitToTextSize();
                Console.WriteLine($"Final Width: {textBox.Width}, Height: {textBox.Height}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing FitToTextSize method: {ex.Message}");
            }

            // Sonucu kaydet
            workbook.Save("ShapeMethodFitToTextSizeDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


