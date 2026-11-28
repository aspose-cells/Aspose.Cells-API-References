---
title: "Cell.GetDisplayStyle"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Hücre yöntemi. Bu hücrenin görüntü stilini alır"
type: docs
url: /tr/net/aspose.cells/cell/getdisplaystyle/
---
## GetDisplayStyle() {#getdisplaystyle}

Bu hücrenin görüntüleme stilini al.

```csharp
public Style GetDisplayStyle()
```

### Dönüş Değeri

bu hücrenin görüntü stili

### Açıklamalar

`GetDisplayStyle` için SideBorders kullanmakla aynı şeydir. Yani bu yöntem, bu hücrenin üst/alt/sol/sağ kenarlarını komşu hücrelerin stiline ([`GetStyle`](../getstyle/)) göre kontrol eder ve ayarlar, ancak birleştirilmiş hücreleri kontrol etmez ve komşu hücrelerin görüntü stilini kontrol etmez.

### Örnekler

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class CellMethodGetDisplayStyleDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];
            
            // A1 hücresi için stil ayarla
            Style style1 = workbook.CreateStyle();
            style1.ForegroundColor = Color.FromArgb(157, 195, 230);
            worksheet.Cells["A1"].SetStyle(style1);
            
            // A23 hücresi için stil ayarla
            Style style2 = workbook.CreateStyle();
            style2.ForegroundColor = Color.Red;
            worksheet.Cells["A23"].SetStyle(style2);
            
            // Stilleri al ve görüntüle
            Style displayStyle1 = worksheet.Cells["A1"].GetDisplayStyle();
            Console.WriteLine("A1 Foreground Color: " + displayStyle1.ForegroundColor);
            
            Style displayStyle2 = worksheet.Cells["A23"].GetDisplayStyle();
            Console.WriteLine("A23 Foreground Color: " + displayStyle2.ForegroundColor);
        }
    }
}
```

### Ayrıca Bakınız

* class [Style](../../style/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetDisplayStyle(bool) {#getdisplaystyle_2}

Bu hücrenin görüntüleme stilini al.

```csharp
public Style GetDisplayStyle(bool includeMergedBorders)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| includeMergedBorders | Boolean | Birleştirilmiş hücrelerin kenarlarının kontrol edilip edilmediğini gösterir. |

### Dönüş Değeri

bu hücrenin görüntü stili

### Açıklamalar

Belirtilen bayrak false ise, `GetDisplayStyle` ile aynı olur. Aksi takdirde `GetDisplayStyle` için SideBorders&#x7C;DynamicStyleBorders kullanmakla aynı olur.

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodGetDisplayStyleWithBooleanDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];
            
            // B2 hücresine eriş ve bazı stil özelliklerini ayarla
            Cell cell = worksheet.Cells["B2"];
            Style cellStyle = cell.GetStyle();
            cellStyle.Borders[BorderType.RightBorder].LineStyle = CellBorderType.Thin;
            cell.SetStyle(cellStyle);
            
            // Biçimlendirme ile görüntü stilini al (true parametresi)
            Style displayStyle = cell.GetDisplayStyle(true);
            
            // Sağ kenar çizgi stilini çıkart
            Console.WriteLine("Right Border Line Style: " + displayStyle.Borders[BorderType.RightBorder].LineStyle);
        }
    }
}
```

### Ayrıca Bakınız

* class [Style](../../style/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetDisplayStyle(BorderType) {#getdisplaystyle_1}

Bu hücrenin görüntüleme stilini al.

```csharp
public Style GetDisplayStyle(BorderType adjacentBorders)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| adjacentBorders | BorderType | Komşu hücrelerin kenarlarına göre hangi kenarların kontrol edilip ayarlanması gerektiğini gösterir. |

### Dönüş Değeri

bu hücrenin görüntü stili

### Açıklamalar

Eğer bu hücre koşullu biçimlendirme, liste nesneleri vb. gibi diğer ayarlardan da etkileniyorsa, görüntü stili [`GetStyle`](../getstyle/) değerinden farklı olabilir. Komşu hücrelere göre kenarları ayarlama bayrakları için TopBorder/BottomBorder/LeftBorder/RightBorder, bu hücrenin sol/sağ/üst/alt komşu hücrelerinin alt/üst/sağ/sol kenarlarının kontrol edilip birleştirilip birleştirilmeyeceğini belirtir. Performans ve uyumluluk açısından, bazı özel işlemleri belirtmek için bazı enum'lar kullanılır: Horizontal/Vertical, birleştirilmiş hücrelerin alt/sağ kenarının bu hücreye kontrol edilip birleştirilip birleştirilmeyeceğini gösterir. Diagonal (yani DiagonalUpBorder ve DiagonalDownBorder ikisi de ayarlanmış) komşu hücrelerin görüntü stilinden kenarların kontrol edilip birleştirilmesini ifade eder. Lütfen, özellikle görüntü stillerinin kontrol edilmesi, komşu hücrelerin kenarlarını/stillerini kontrol etmenin zaman tüketen bir işlem olduğunu unutmayın. Döndürülen stil için kenarların alınmasına ihtiyaç yoksa, komşu hücrelerin işlenmesini devre dışı bırakmak için None kullanmak daha iyi performans sağlar. Diagonal ayarlamadan sadece bu hücrelerde tanımlı stillerden komşu hücrelerin kenarlarını alırken (Diagonal ayarlanmamış), performans da daha iyi olabilir çünkü tek bir hücrenin görüntü stilini kontrol etmek de zaman alır.

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodGetDisplayStyleWithBorderTypeDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            Cells cells = sheet.Cells;

            // Örnek veriyi ayarla
            for (int i = 0; i < 10; i++)
            {
                cells[i, 0].PutValue(i);
            }

            // Koşullu biçimlendirme oluştur
            FormatConditionCollection fcs = sheet.ConditionalFormattings[sheet.ConditionalFormattings.Add()];
            fcs.AddArea(CellArea.CreateCellArea(0, 0, 9, 0));
            fcs.AddCondition(FormatConditionType.ColorScale);

            // Farklı kenar tipleriyle görüntü stilini al
            for (int i = 0; i < 10; i++)
            {
                Style styleWithBorder = cells[i, 0].GetDisplayStyle(BorderType.TopBorder);
                Style styleWithoutBorder = cells[i, 0].GetDisplayStyle(BorderType.None);

                Console.WriteLine($"Cell {i + 1}:");
                Console.WriteLine($"  Style with border - Foreground: {styleWithBorder.ForegroundArgbColor:X}");
                Console.WriteLine($"  Style without border - Foreground: {styleWithoutBorder.ForegroundArgbColor:X}");
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [Style](../../style/)
* enum [BorderType](../../bordertype/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


