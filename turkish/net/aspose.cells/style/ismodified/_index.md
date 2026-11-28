---
title: "Style.IsModified"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Style yöntemi. Stil'in belirtilen özelliklerinin değiştirilip değiştirilmediğini kontrol eder. ConditionalFormattings stilinde, bu stilin belirtilen özelliklerinin bir hücreye ConditionalFormattings uygulanırken kullanılıp kullanılmayacağını kontrol etmek için kullanılır."
type: docs
url: /tr/net/aspose.cells/style/ismodified/
---
## Style.IsModified method

Stilin belirtilen özelliklerinin değiştirilip değiştirilmediğini kontrol eder. Hücreye ConditionalFormattings uygulanırken bu stilin belirtilen özelliklerinin kullanılıp kullanılmayacağını kontrol etmek için ConditionalFormattings stilinde kullanılır.

```csharp
public bool IsModified(StyleModifyFlag modifyFlag)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| modifyFlag | StyleModifyFlag | Style değiştirilmiş bayrakları |

### Dönüş Değeri

belirtilen özellikler değiştirilmişse doğru

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StyleMethodIsModifiedWithStyleModifyFlagDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];
            
            // A1 hücresinin stilini al
            Style style = worksheet.Cells["A1"].GetStyle();
            
            // Stil'in desenini (arka plan) değiştir
            style.Pattern = BackgroundType.Solid;
            style.ForegroundColor = System.Drawing.Color.Yellow;
            
            // Desenin değiştirilip değiştirilmediğini kontrol et
            bool isPatternModified = style.IsModified(StyleModifyFlag.Pattern);
            
            // Sonucu çıktı olarak ver
            Console.WriteLine("Is pattern modified: " + isPatternModified);
        }
    }
}
```

### Ayrıca Bakınız

* enum [StyleModifyFlag](../../stylemodifyflag/)
* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


