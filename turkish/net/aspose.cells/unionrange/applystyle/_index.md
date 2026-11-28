---
title: "UnionRange.ApplyStyle"
second_title: "Aspose.Cells için .NET API Referansı"
description: "UnionRange yöntemi. Tüm bir aralık için biçimleri uygular"
type: docs
url: /tr/net/aspose.cells/unionrange/applystyle/
---
## UnionRange.ApplyStyle method

Tüm bir aralık için biçimlendirmeleri uygular

```csharp
public void ApplyStyle(Style style, StyleFlag flag)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| stil | Stil | Uygulanacak stil nesnesi. |
| bayrak | StyleFlag | Uygulanan biçimlendirme özelliklerini gösteren bayraklar. |

### Açıklamalar

Bu aralıktaki her hücre bir [`Style`](../../style/) nesnesi içerir. Bu nedenle bellek tüketen bir yöntemdir. Lütfen dikkatli kullanın.

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class UnionRangeMethodApplyStyleWithStyleStyleFlagDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // A1'den B2'ye kadar hücreleri kapsayan bir birleşim aralığı oluşturun
            UnionRange unionRange = worksheet.Cells.CreateRange("A1:B2").UnionRanges(new Aspose.Cells.Range[] { worksheet.Cells.CreateRange("A1:B2") });

            // Bağlam için bazı veriler ekle
            worksheet.Cells["A1"].Value = "Sample Data";
            worksheet.Cells["B2"].Value = "More Data";

            try
            {
                // Belirli biçimlendirme ile bir stil oluşturun
                Style style = workbook.CreateStyle();
                style.Font.IsBold = true;
                style.Font.Color = Color.Red;
                style.ForegroundColor = Color.LightBlue;
                style.Pattern = BackgroundType.Solid;
                style.HorizontalAlignment = TextAlignmentType.Center;

                // Uygulanacak özellikleri belirlemek için bir StyleFlag oluşturun
                StyleFlag flag = new StyleFlag();
                flag.FontBold = true;
                flag.FontColor = true;
                flag.CellShading = true;
                flag.HorizontalAlignment = true;

                // Stil ve bayrak parametreleriyle ApplyStyle'ı çağırın
                unionRange.ApplyStyle(style, flag);

                Console.WriteLine("ApplyStyle method called successfully");
                Console.WriteLine($"Applied style to range: {unionRange.RefersTo}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling ApplyStyle: {ex.Message}");
            }

            // Çalışma kitabını kaydedin
            workbook.Save("UnionRangeMethodApplyStyleWithStyleStyleFlagDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Style](../../style/)
* class [StyleFlag](../../styleflag/)
* class [UnionRange](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


