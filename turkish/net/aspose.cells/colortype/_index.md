---
title: "Enum ColorType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.ColorType enum. Tüm renk tiplerini temsil eder"
type: docs
url: /tr/net/aspose.cells/colortype/
---
## ColorType enumeration

Tüm renk türlerini temsil eder

```csharp
public enum ColorType
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| Automatic | `0` | Otomatik renk. |
| AutomaticIndex | `1` | Bu otomatik renktir, ancak görüntülenen renk işletim sistemi ayarına bağlıdır. |
| RGB | `2` | RGB rengi. |
| IndexedColor | `3` | Renk paletindeki renk indeksi. |
| Theme | `4` | Tema rengi. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsClassColorTypeDemo
    {
        public static void Run()
        {
            try
            {
                // Demonstrasyon için yeni bir çalışma kitabı oluştur
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];

                // ColorType enum değerlerini kullanarak gösterin
                ColorType automatic = ColorType.Automatic;
                ColorType rgb = ColorType.RGB;
                ColorType theme = ColorType.Theme;

                // Enum değerlerini görüntüle
                Console.WriteLine($"Automatic color type value: {(int)automatic}");
                Console.WriteLine($"RGB color type value: {(int)rgb}");
                Console.WriteLine($"Theme color type value: {(int)theme}");

                // Bir hücre oluşturun ve değerini ayarlayın
                Cell cell = worksheet.Cells["A1"];
                cell.PutValue("ColorType Demo");

                // Bir stil oluşturun ve hücreye uygulayın
                Style style = workbook.CreateStyle();
                style.Font.Color = System.Drawing.Color.Black;
                cell.SetStyle(style);

                // Çalışma kitabını kaydedin
                workbook.Save("ColorTypeDemo.xlsx");

                Console.WriteLine("ColorType demonstration completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error in ColorType demonstration: {ex.Message}");
            }
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


