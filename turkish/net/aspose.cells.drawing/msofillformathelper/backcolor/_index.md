---
title: "MsoFillFormatHelper.BackColor"
second_title: "Aspose.Cells için .NET API Referansı"
description: "MsoFillFormatHelper özelliği. Doldurma arka rengini alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells.drawing/msofillformathelper/backcolor/
---
## MsoFillFormatHelper.BackColor property

Dosyanın arka rengini alır ve ayarlar.

```csharp
public Color BackColor { get; set; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class MsoFillFormatHelperPropertyBackColorDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluşturun ve ilk çalışma sayfasını alın.
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Sayfada biraz içerik olması için sadece bir etiket ekle
            worksheet.Cells["A1"].Value = "BackColor Property Demo";

            try
            {
                // MsoFillFormatHelper genel bir yapıcı sunmaz, örneklemek için yansıma (reflection) kullan
                MsoFillFormatHelper fillHelper = (MsoFillFormatHelper)Activator.CreateInstance(
                    typeof(MsoFillFormatHelper), nonPublic: true);

                // BackColor'ı bilinen bir renge ayarla (örn., LightCoral)
                fillHelper.BackColor = Color.LightCoral;

                // BackColor değerini geri oku ve göster
                Console.WriteLine($"BackColor is set to: {fillHelper.BackColor}");

                // İsteğe bağlı olarak ForeColor'ı da okuyabilir ve varsayılan kaldığını gösterebilirsiniz
                Console.WriteLine($"ForeColor (default) : {fillHelper.ForeColor}");

                // Çalışma kitabını kaydet – doldurma yardımcı programı bir şekle eklenmemiş,
                // ancak kaydetmek, kodun hatasız çalıştığını gösterir.
                workbook.Save("BackColorDemo.xlsx");

                Console.WriteLine("Demo completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error during BackColor demo: {ex.Message}");
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [MsoFillFormatHelper](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


