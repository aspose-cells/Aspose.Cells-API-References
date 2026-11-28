---
title: "ThemeColor.Tint"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ThemeColor özelliği. Renk tonu değerini alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells/themecolor/tint/
---
## ThemeColor.Tint property

Renk tonu değerini alır ve ayarlar.

```csharp
public double Tint { get; set; }
```

### Açıklamalar

Renk tonu değeri -1.0 ile 1.0 arasında bir double olarak saklanır; -1.0 %100 karartma, 1.0 %100 aydınlatma anlamına gelir. Ayrıca, 0.0 değişiklik olmadığını gösterir.

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ThemeColorPropertyTintDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Tema rengi ve renk tonu ile bir stil oluştur
            Style style = workbook.CreateStyle();
            style.BackgroundThemeColor = new ThemeColor(ThemeColorType.Accent1, 0.5); // 0.5 tint
            
            // Stili bir hücreye uygula
            Cell cell = worksheet.Cells["A1"];
            cell.SetStyle(style);

            // Hücrenin stilinden renk tonu değerini al
            double tintValue = cell.GetStyle().BackgroundThemeColor.Tint;
            Console.WriteLine("Tint value: " + tintValue);

            // Renk tonu değerini değiştir
            ThemeColor themeColor = cell.GetStyle().BackgroundThemeColor;
            themeColor.Tint = 0.8; // Change tint to 0.8
            cell.SetStyle(style);

            // Yeni renk tonu değerini doğrula
            Console.WriteLine("Modified tint value: " + cell.GetStyle().BackgroundThemeColor.Tint);
        }
    }
}
```

### Ayrıca Bakınız

* class [ThemeColor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


