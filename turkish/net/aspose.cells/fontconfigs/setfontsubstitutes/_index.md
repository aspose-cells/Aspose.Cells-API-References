---
title: "FontConfigs.SetFontSubstitutes"
second_title: "Aspose.Cells için .NET API Referansı"
description: "FontConfigs yöntemi. Verilen orijinal yazı tipi adı için yazı tipi ikame adları"
type: docs
url: /tr/net/aspose.cells/fontconfigs/setfontsubstitutes/
---
## FontConfigs.SetFontSubstitutes method

Verilen orijinal yazı tipi adı için ikame yazı tipi adları.

```csharp
public static void SetFontSubstitutes(string originalFontName, string[] substituteFontNames)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| originalFontName | String | Orijinal yazı tipi adı. |
| substituteFontNames | String[] | Orijinal yazı tipi mevcut değilse kullanılacak yazı tipi ikame adlarının listesi. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class FontConfigsMethodSetFontSubstitutesWithStringStringDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Mevcut olmayabilecek orijinal yazı tipi adı
            string originalFontName = "Arial";
            
            // Orijinal mevcut olmadığında kullanılacak ikame yazı tipi adları
            string[] substituteFontNames = new string[] { "Liberation Sans", "Helvetica", "Verdana" };
            
            try
            {
                // Yazı tipi ikamelerini yapılandırmak için SetFontSubstitutes yöntemini çağırın
                FontConfigs.SetFontSubstitutes(originalFontName, substituteFontNames);
                
                Console.WriteLine($"Font substitutes set successfully for '{originalFontName}'");
                
                // İkameleri alarak doğrulayın
                string[] retrievedSubstitutes = FontConfigs.GetFontSubstitutes(originalFontName);
                Console.WriteLine("Current substitutes for '{0}':", originalFontName);
                foreach (string font in retrievedSubstitutes)
                {
                    Console.WriteLine("- " + font);
                }
                
                // İkameyi göstermek için yazı tipini bir hücreye uygulayın
                worksheet.Cells["A1"].PutValue("Text with potential font substitution");
                Style style = worksheet.Cells["A1"].GetStyle();
                style.Font.Name = originalFontName;
                worksheet.Cells["A1"].SetStyle(style);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetFontSubstitutes method: {ex.Message}");
            }
            
            // Çalışma kitabını kaydedin
            workbook.Save("FontSubstitutionDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [FontConfigs](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


