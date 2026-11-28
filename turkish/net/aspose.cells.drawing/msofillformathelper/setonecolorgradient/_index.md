---
title: "MsoFillFormatHelper.SetOneColorGradient"
second_title: "Aspose.Cells için .NET API Referansı"
description: "MsoFillFormatHelper yöntemi. Belirtilen doldurmayı tek renkli bir degradeye ayarlar"
type: docs
url: /tr/net/aspose.cells.drawing/msofillformathelper/setonecolorgradient/
---
## MsoFillFormatHelper.SetOneColorGradient method

Belirtilen dolguyu tek renkli bir degrade olarak ayarlar.

```csharp
public void SetOneColorGradient(Color color, double degree, GradientStyleType style, int variant)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| color | Color | Bir degrade rengi. |
| derece | Double | Degrade derecesi. 0.0 (koyu) ile 1.0 (açık) arasında bir değer olabilir. |
| stil | GradientStyleType | Degrade gölgelendirme stili. |
| variant | Int32 | Degrade varyantı. 1 ile 4 arasında bir değer olabilir ve Doldurma Efektleri iletişim kutusundaki Degrade sekmesindeki dört varyanttan birine karşılık gelir. Stil GradientStyle.FromCenter ise, Variant argümanı yalnızca 1 veya 2 olabilir. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class MsoFillFormatHelperMethodSetOneColorGradientWithColorDoubleGradientStyleTyInt32Demo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluşturun ve ilk çalışma sayfasını alın.
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Bağlam için sayfaya basit bir etiket ekleyin
            worksheet.Cells["A1"].Value = "Gradient Fill Demo";

            try
            {
                // Yansıma kullanarak MsoFillFormatHelper örneği oluşturun (herhangi bir public ctor yok)
                MsoFillFormatHelper fillHelper = (MsoFillFormatHelper)Activator.CreateInstance(
                    typeof(MsoFillFormatHelper), nonPublic: true);

                // Degrade için parametreler
                Color gradientColor = Color.FromArgb(255, 0, 120, 215); // a shade of blue
                double degree = 45.0;                                 // gradient angle in degrees
                GradientStyleType style = GradientStyleType.Horizontal; // horizontal gradient
                int variant = 0;                                      // variant (0 = default)

                // Tek renkli degradeyi uygulayın
                fillHelper.SetOneColorGradient(gradientColor, degree, style, variant);

                // İsteğe bağlı: çağrıdan sonra özelliklerin okunabileceğini gösterin
                Console.WriteLine($"ForeColor after gradient: {fillHelper.ForeColor}");
                Console.WriteLine($"ForeColorTransparency after gradient: {fillHelper.ForeColorTransparency}");

                // Çalışma kitabını kaydedin (yardımcı şekle ekli olmadığı için görsel bir değişiklik görülmez)
                workbook.Save("SetOneColorGradientDemo.xlsx");

                Console.WriteLine("SetOneColorGradient method called successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling SetOneColorGradient: {ex.Message}");
            }
        }
    }
}
```

### Ayrıca Bakınız

* enum [GradientStyleType](../../gradientstyletype/)
* class [MsoFillFormatHelper](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


