---
title: "Style.InvariantCustom"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Style özelliği. Sayı biçimi için kültür bağımsız desen dizesini alır. Bu nesne için bir sayı biçimi ayarlanmamışsa null döndürülür. Sayı biçimi yerleşik ise, yerleşik sayıya karşılık gelen desen dizesi döndürülür."
type: docs
url: /tr/net/aspose.cells/style/invariantcustom/
---
## Style.InvariantCustom property

Sayı biçimi için kültür bağımsız desen dizesini alır. Bu nesne için bir sayı biçimi ayarlanmamışsa null döndürülür. Sayı biçimi yerleşik ise, yerleşik sayıya karşılık gelen desen dizesi döndürülür.

```csharp
public string InvariantCustom { get; }
```

### Açıklamalar

Yerleşik sayı biçimleri için, döndürülen desen içeriği hâlâ kültüre bağlıdır; örneğin bazı yerel ayarlarda "m/d/y" ve diğer bazı yerel ayarlarda "d/m/y" döndürür. [`CultureCustom`](../culturecustom/) ile farkı (bu aynı zamanda kültür bağımsızının ne anlama geldiğidir): biçim belirteçleri ve ayırıcılar standart olarak tutulur; örneğin '/' her zaman tarih‑saat ayırıcı olarak kullanılır ve "y" her zaman "yıl" kısmı olarak kullanılır, belirli yerel ayar için başka özel karakter kullanılsa bile.

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StylePropertyInvariantCustomDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            wb.Settings.Region = CountryCode.Germany;
            Cell cell = wb.Worksheets[0].Cells[0, 0];
            Style style = cell.GetStyle();
            
            // Tarih biçimini ve değerini ayarlayın
            style.Number = 14; // Date format
            style.Custom = "dd/MM/yyyy"; // Set custom format which affects both CultureCustom and InvariantCustom
            cell.PutValue(new DateTime(2019, 10, 12));
            cell.SetStyle(style);

            // Sonuçları çıktı olarak ver
            Console.WriteLine("Formatted value: " + cell.StringValue);
            Console.WriteLine("CultureCustom: " + style.CultureCustom);
            Console.WriteLine("InvariantCustom: " + style.InvariantCustom);
        }
    }
}
```

### Ayrıca Bakınız

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


