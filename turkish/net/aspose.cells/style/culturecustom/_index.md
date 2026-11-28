---
title: "Style.CultureCustom"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Style özelliği. Sayı biçimi için kültüre bağımlı desen dizgisini alır ve ayarlar. Bu nesne için hiçbir sayı biçimi ayarlanmamışsa null döndürülür. Sayı biçimi yerleşik ise, yerleşik sayıya karşılık gelen desen dizgisi döndürülür."
type: docs
url: /tr/net/aspose.cells/style/culturecustom/
---
## Style.CultureCustom property

Sayı formatı için kültüre bağlı desen dizesini alır ve ayarlar. Bu nesne için hiçbir sayı formatı ayarlanmamışsa, null döndürülür. Sayı formatı yerleşik ise, yerleşik sayıya karşılık gelen desen dizesi döndürülür.

```csharp
public string CultureCustom { get; set; }
```

### Açıklamalar

Yerleşik sayı biçimi için, desen içeriği (örneğin, bazı yerel ayarlarda bir yerleşik tarih biçimi "m/d/y" iken, diğerlerinde "d/m/y" olur) ve biçim belirteci (örneğin, bazı yerel ayarlarda yıl kısmını temsil etmek için 'y' dışındaki bir karakter kullanılır) kültüre bağlıdır; Kullanıcı tarafından belirtilen özel biçim için ise yalnızca biçim belirteçleri kültüre göre değiştirilir, biçim deseninin diğer bölümleri değiştirilmez.

### Örnekler

```csharp
using System;
using System.Globalization;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StylePropertyCultureCustomDemo
    {
        public static void Run()
        {
            // Bir çalışma kitabı oluşturun ve Macar kültürünü ayarlayın
            Workbook wb = new Workbook();
            wb.Settings.CultureInfo = new CultureInfo("hu-HU");

            // İlk hücreyi ve stilini alın
            Cell cell = wb.Worksheets[0].Cells[0, 0];
            Style style = cell.GetStyle();

            // Özel biçim ayarlayın ve CultureCustom dönüşümünü gösterin
            string customFormat = "yyyy-MM-dd hh:mm:ss ddd dddd MMM MMMM MMMMM";
            string cultureCustomFormat = "éééé-hh-nn óó:pp:mm nnn nnnn hhh hhhh hhhhh";
            
            style.Custom = customFormat;
            Console.WriteLine("CultureCustom from Custom: " + style.CultureCustom);
            
            style.CultureCustom = cultureCustomFormat;
            Console.WriteLine("Custom from CultureCustom: " + style.Custom);

            // Stili uygulayın ve kültüre duyarlı biçimlendirmeyi gösterin
            cell.SetStyle(style);
            cell.PutValue(47512); // January 29, 2030
            Console.WriteLine("Formatted value: " + cell.StringValue);

            // Kültür biçimlendirmeli formülü gösterin
            cell.Formula = "=TEXT(47512,\"" + cultureCustomFormat + "\")";
            wb.CalculateFormula();
            Console.WriteLine("Calculated value: " + cell.StringValue);
        }
    }
}
```

### Ayrıca Bakınız

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


