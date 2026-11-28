---
title: "RadioButton.GetOptionIndex"
second_title: "Aspose.Cells için .NET API Referansı"
description: "RadioButton yöntemi. Bu radyo düğmesini içeren GroupBox'taki tüm radyo düğmelerinde bir bazlı seçenek indeksini alır"
type: docs
url: /tr/net/aspose.cells.drawing/radiobutton/getoptionindex/
---
## RadioButton.GetOptionIndex method

Bu radyo düğmesini içeren GroupBox'taki tüm radyo düğmelerinde seçenek indeksini (bir tabanlı) alır.

```csharp
public int GetOptionIndex()
```

### Açıklamalar

Bu radyo düğmesi GroupBox içinde değilse, herhangi bir GroupBox içinde olmayan tüm radyo düğmelerindeki seçenek indeksini döndürür

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class RadioButtonMethodGetOptionIndexDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Radyo düğmelerini içerecek bir grup kutusu ekle
            GroupBox groupBox = worksheet.Shapes.AddGroupBox(1, 0, 100, 200, 100, 200);

            // Grup kutusuna üç radyo düğmesi ekle
            RadioButton radioButton1 = (RadioButton)worksheet.Shapes.AddRadioButton(3, 0, 20, 100, 20, 100);
            RadioButton radioButton2 = (RadioButton)worksheet.Shapes.AddRadioButton(3, 0, 50, 100, 20, 100);
            RadioButton radioButton3 = (RadioButton)worksheet.Shapes.AddRadioButton(3, 0, 80, 100, 20, 100);

            // Radyo düğmelerini grup kutusunun bir parçası olacak şekilde ayarla
            radioButton1.Placement = PlacementType.FreeFloating;
            radioButton2.Placement = PlacementType.FreeFloating;
            radioButton3.Placement = PlacementType.FreeFloating;

            try
            {
                // Her radyo düğmesi için seçenek indeksini al
                int index1 = radioButton1.GetOptionIndex();
                int index2 = radioButton2.GetOptionIndex();
                int index3 = radioButton3.GetOptionIndex();

                Console.WriteLine($"RadioButton1 Option Index: {index1}");
                Console.WriteLine($"RadioButton2 Option Index: {index2}");
                Console.WriteLine($"RadioButton3 Option Index: {index3}");

                // Seçimi göstermek için ilk radyo düğmesini işaretle
                radioButton1.IsChecked = true;
                Console.WriteLine("RadioButton1 is checked");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetOptionIndex method: {ex.Message}");
            }

            // Sonucu kaydet
            workbook.Save("RadioButtonMethodGetOptionIndexDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [RadioButton](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


