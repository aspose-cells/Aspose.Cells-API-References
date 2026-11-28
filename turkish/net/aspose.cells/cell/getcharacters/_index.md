---
title: "Cell.GetCharacters"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Cell yöntemi. Hücre metni içindeki bir karakter aralığını temsil eden tüm Characters nesnelerini döndürür"
type: docs
url: /tr/net/aspose.cells/cell/getcharacters/
---
## GetCharacters() {#getcharacters}

Hücre metni içinde bir karakter aralığını temsil eden tüm Characters nesnelerini döndürür.

```csharp
public FontSetting[] GetCharacters()
```

### Dönüş Değeri

Tüm Characters nesneleri

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodGetCharactersDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // A1 hücresine farklı biçimlendirme bölümleriyle HTML biçimlendirilmiş metin ayarlayın
            worksheet.Cells["A1"].HtmlString = "Normal text<div style=\"color: red;\">Red text</div>";

            // A1 hücresinden karakter biçimlendirme bilgilerini alın
            FontSetting[] fontSettings = worksheet.Cells["A1"].GetCharacters();

            // Biçimlendirme bilgisini çıktı olarak verin
            Console.WriteLine("Character formatting in cell A1:");
            for (int i = 0; i < fontSettings.Length; i++)
            {
                Console.WriteLine($"Part {i + 1}:");
                Console.WriteLine($"Start index: {fontSettings[i].StartIndex}");
                Console.WriteLine($"Length: {fontSettings[i].Length}");
                Console.WriteLine($"Font color: {fontSettings[i].Font.Color}");
                Console.WriteLine();
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [FontSetting](../../fontsetting/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetCharacters(bool) {#getcharacters_1}

Hücre metni içinde bir karakter aralığını temsil eden tüm Characters nesnelerini döndürür.

```csharp
public FontSetting[] GetCharacters(bool flag)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| bayrak | Boolean | Hücre bir tablo içinde ise tablo stilinin hücreye uygulanıp uygulanmayacağını gösterir. |

### Dönüş Değeri

Tüm Characters nesneleri

### Örnekler

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class CellMethodGetCharactersWithBooleanDemo
    {
        public static void Run()
        {
            // Bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];
            
            // C8 hücresine biçimlendirme ile metin ekleyin
            Cell cell = worksheet.Cells["C8"];
            cell.PutValue("Formatted Text");
            
            // Metnin bölümlerini biçimlendir
            FontSetting fs1 = cell.Characters(0, 8);
            fs1.Font.Color = System.Drawing.Color.White;
            
            FontSetting fs2 = cell.Characters(9, 4);
            fs2.Font.Color = System.Drawing.Color.Blue;
            
            // Biçimlendirme ile tüm yazı tipi ayarlarını al
            FontSetting[] fontSettings = cell.GetCharacters(true);
            
            // Yazı tipi renklerini göster
            Console.WriteLine("Font colors in cell C8:");
            foreach (FontSetting fs in fontSettings)
            {
                Console.WriteLine(fs.Font.Color);
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [FontSetting](../../fontsetting/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


