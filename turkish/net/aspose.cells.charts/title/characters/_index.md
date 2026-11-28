---
title: "Title.Characters"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Title yöntemi. Bu başlığın zengin metin biçimlendirmesini alır"
type: docs
url: /tr/net/aspose.cells.charts/title/characters/
---
## Title.Characters method

Bu Başlığın zengin metin biçimlendirmesini alır.

```csharp
public FontSetting[] Characters()
```

### Dönüş Değeri

FontSetting dizisini döndürür

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class TitleMethodCharactersDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Çalışma sayfasına örnek veri ekle
            worksheet.Cells["A1"].PutValue("Item");
            worksheet.Cells["B1"].PutValue("Quantity");
            worksheet.Cells["A2"].PutValue("Apples");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["A3"].PutValue("Oranges");
            worksheet.Cells["B3"].PutValue(5);

            // Bir grafik oluştur
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Grafik veri aralığını ayarla
            chart.NSeries.Add("B2:B3", true);
            chart.NSeries.CategoryData = "A2:A3";

            // Grafik başlığını ayarla
            chart.Title.Text = "Fruit Sales Report";
            chart.Title.IsVisible = true;

            try
            {
                // Başlığın zengin metin biçimlendirmesini al
                FontSetting[] titleCharacters = chart.Title.Characters();
                
                // İlk karakterin yazı tipini değiştir
                if (titleCharacters.Length > 0)
                {
                    titleCharacters[0].Font.Color = System.Drawing.Color.Red;
                    titleCharacters[0].Font.IsBold = true;
                    titleCharacters[0].Font.Size = 14;
                }

                Console.WriteLine("Characters method executed successfully");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Characters method: {ex.Message}");
            }
            
            // Sonucu kaydet
            workbook.Save("TitleMethodCharactersDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [FontSetting](../../../aspose.cells/fontsetting/)
* class [Title](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


