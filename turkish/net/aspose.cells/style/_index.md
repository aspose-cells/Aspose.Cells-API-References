---
title: "Sınıf Style"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Style class. Excel belgelerinin, örneğin fontcoloralignmentborderetc gibi görüntü stilini temsil eder. Style nesnesi, tüm stil özelliklerini (font, sayı formatı, hizalama vb.) özellikler olarak içerir."
type: docs
url: /tr/net/aspose.cells/style/
---
## Style class

Excel belgesinin görüntü stilini temsil eder, örneğin yazı tipi, renk, hizalama, kenarlık vb. Style nesnesi, tüm stil özelliklerini (yazı tipi, sayı biçimi, hizalama vb.) özellikler olarak içerir.

```csharp
public class Style
```

## Yapıcılar

| Ad | Açıklama |
| --- | --- |
| [Style](style/)() | (**Obsolete.**) `Style` sınıfının yeni bir örneğini başlatır. |

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [BackgroundArgbColor](../../aspose.cells/style/backgroundargbcolor/) { get; set; } | 32-bit ARGB değeriyle arka plan rengini alır ve ayarlar. |
| [BackgroundColor](../../aspose.cells/style/backgroundcolor/) { get; set; } | Bir stilin arka plan rengini alır veya ayarlar. |
| [BackgroundThemeColor](../../aspose.cells/style/backgroundthemecolor/) { get; set; } | Arka plan tema rengini alır ve ayarlar. |
| [Borders](../../aspose.cells/style/borders/) { get; } | Stilin [`BorderCollection`](../bordercollection/) öğesini alır. |
| [BottomBorder](../../aspose.cells/style/bottomborder/) { get; } | Alt kenarlığı alır. |
| [CultureCustom](../../aspose.cells/style/culturecustom/) { get; set; } | Sayı formatı için kültüre bağlı desen dizesini alır ve ayarlar. Bu nesne için hiçbir sayı formatı ayarlanmamışsa, null döndürülür. Sayı formatı yerleşik ise, yerleşik sayıya karşılık gelen desen dizesi döndürülür. |
| [Custom](../../aspose.cells/style/custom/) { get; set; } | Bu stil nesnesinin özel sayı formatı dizesini temsil eder. Özel sayı formatı ayarlanmamışsa (örneğin, sayı formatı yerleşik ise), \"\" döndürülür. |
| [Font](../../aspose.cells/style/font/) { get; } | Bir [`Font`](./font/) nesnesi alır. |
| [ForegroundArgbColor](../../aspose.cells/style/foregroundargbcolor/) { get; set; } | 32-bit ARGB değeriyle ön plan rengini alır ve ayarlar. |
| [ForegroundColor](../../aspose.cells/style/foregroundcolor/) { get; set; } | Bir stilin ön plan rengini alır veya ayarlar. |
| [ForegroundThemeColor](../../aspose.cells/style/foregroundthemecolor/) { get; set; } | Ön plan tema rengini alır ve ayarlar. |
| [HasBorders](../../aspose.cells/style/hasborders/) { get; } | Stil için kenarlıkların ayarlanıp ayarlanmadığını kontrol eder. |
| [HorizontalAlignment](../../aspose.cells/style/horizontalalignment/) { get; set; } | Bir hücredeki metnin yatay hizalama türünü alır veya ayarlar. |
| [IndentLevel](../../aspose.cells/style/indentlevel/) { get; set; } | Hücre veya aralık için girinti seviyesini temsil eder. Yalnızca 0 ile 250 arasında bir tam sayı olabilir. |
| [InvariantCustom](../../aspose.cells/style/invariantcustom/) { get; } | Sayı biçimi için kültür bağımsız desen dizesini alır. Bu nesne için bir sayı biçimi ayarlanmamışsa null döndürülür. Sayı biçimi yerleşik ise, yerleşik sayıya karşılık gelen desen dizesi döndürülür. |
| [IsAlignmentApplied](../../aspose.cells/style/isalignmentapplied/) { get; set; } | Hizalama biçimlendirmesinin uygulanıp uygulanmayacağını belirt. |
| [IsBorderApplied](../../aspose.cells/style/isborderapplied/) { get; set; } | Kenarlık biçimlendirmesinin uygulanıp uygulanmayacağını belirt. |
| [IsCheckBox](../../aspose.cells/style/ischeckbox/) { get; set; } | Bir onay kutusu stili olup olmadığını gösterir. |
| [IsDateTime](../../aspose.cells/style/isdatetime/) { get; } | Sayı biçiminin tarih biçimi olup olmadığını gösterir. |
| [IsFillApplied](../../aspose.cells/style/isfillapplied/) { get; set; } | Dolgu biçimlendirmesinin uygulanıp uygulanmayacağını belirt. |
| [IsFontApplied](../../aspose.cells/style/isfontapplied/) { get; set; } | Yazı tipi biçimlendirmesinin uygulanıp uygulanmayacağını belirt. |
| [IsFormulaHidden](../../aspose.cells/style/isformulahidden/) { get; set; } | Çalışma sayfası korunduğunda formülün gizlenip gizlenmeyeceğini temsil eder. |
| [IsGradient](../../aspose.cells/style/isgradient/) { get; set; } | Hücre gölgelendirmenin bir degrade deseni olup olmadığını gösterir. |
| [IsJustifyDistributed](../../aspose.cells/style/isjustifydistributed/) { get; set; } | Hücrelerin son satırdaki metin için iki yana hizalama veya dağıtılmış hizalama kullanıp kullanmayacağını gösterir. |
| [IsLocked](../../aspose.cells/style/islocked/) { get; set; } | Bir hücrenin değiştirilebilir olup olmadığını gösteren bir değeri alır veya ayarlar. |
| [IsNumberFormatApplied](../../aspose.cells/style/isnumberformatapplied/) { get; set; } | Sayı biçimlendirmesinin uygulanıp uygulanmayacağını belirt. |
| [IsPercent](../../aspose.cells/style/ispercent/) { get; } | Sayı biçiminin yüzde biçimi olup olmadığını gösterir. |
| [IsProtectionApplied](../../aspose.cells/style/isprotectionapplied/) { get; set; } | Koruma biçimlendirmesinin uygulanıp uygulanmayacağını belirt. |
| [IsTextWrapped](../../aspose.cells/style/istextwrapped/) { get; set; } | Bir hücre içindeki metnin kaydırılıp kaydırılmayacağını gösteren bir değeri alır veya ayarlar. |
| [LeftBorder](../../aspose.cells/style/leftborder/) { get; } | Sol kenarlığı alır. |
| [Name](../../aspose.cells/style/name/) { get; set; } | Stil adını alır veya ayarlar. |
| [Number](../../aspose.cells/style/number/) { get; set; } | Sayıların ve tarihlerin görüntüleme biçimini alır veya ayarlar. Biçimlendirme desenleri farklı bölgeler için farklıdır. |
| [ParentStyle](../../aspose.cells/style/parentstyle/) { get; } | Bu stilin üst stilini alır. |
| [Pattern](../../aspose.cells/style/pattern/) { get; set; } | Hücre arka planı desen türünü alır veya ayarlar. |
| [QuotePrefix](../../aspose.cells/style/quoteprefix/) { get; set; } | Hücrenin değerinin tek tırnak işaretiyle başlayıp başlamadığını gösterir. |
| [RightBorder](../../aspose.cells/style/rightborder/) { get; } | Sağ kenarı alır. |
| [RotationAngle](../../aspose.cells/style/rotationangle/) { get; set; } | Metin döndürme açısını temsil eder. |
| [ShrinkToFit](../../aspose.cells/style/shrinktofit/) { get; set; } | Metnin kullanılabilir sütun genişliğine sığacak şekilde otomatik olarak küçültülüp küçültülmediğini temsil eder. |
| [TextDirection](../../aspose.cells/style/textdirection/) { get; set; } | Metin okuma sırasını temsil eder. |
| [TopBorder](../../aspose.cells/style/topborder/) { get; } | Üst kenarı alır. |
| [VerticalAlignment](../../aspose.cells/style/verticalalignment/) { get; set; } | Bir hücredeki metnin dikey hizalama türünü alır veya ayarlar. |

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| [Copy](../../aspose.cells/style/copy/)(Style) | Başka bir stil nesnesinden verileri kopyalar. |
| override [Equals](../../aspose.cells/style/equals/)(object) | İki Style örneğinin eşit olup olmadığını belirler. |
| override [GetHashCode](../../aspose.cells/style/gethashcode/)() | Bir Style nesnesi için hash işlevi olarak hizmet eder. |
| [GetTwoColorGradient](../../aspose.cells/style/gettwocolorgradient/)(out Color, out Color, out GradientStyleType, out int) | (**Obsolete.**) İki renkli degrade ayarını al. |
| [GetTwoColorGradientSetting](../../aspose.cells/style/gettwocolorgradientsetting/)() | İki renkli degrade ayarını al. |
| [IsModified](../../aspose.cells/style/ismodified/)(StyleModifyFlag) | Stilin belirtilen özelliklerinin değiştirilip değiştirilmediğini kontrol eder. Hücreye ConditionalFormattings uygulanırken bu stilin belirtilen özelliklerinin kullanılıp kullanılmayacağını kontrol etmek için ConditionalFormattings stilinde kullanılır. |
| [SetBorder](../../aspose.cells/style/setborder/#setborder)(BorderType, CellBorderType, CellsColor) | Stilin kenarlarını ayarlar. |
| [SetBorder](../../aspose.cells/style/setborder/#setborder_1)(BorderType, CellBorderType, Color) | Stilin kenarlarını ayarlar. |
| [SetCustom](../../aspose.cells/style/setcustom/)(string, bool) | Bir hücrenin Özel sayı biçim dizesini ayarlar. |
| [SetOutlineBorders](../../aspose.cells/style/setoutlineborders/#setoutlineborders)(CellBorderType, CellsColor) | Anahat kenarlarını ayarla. |
| [SetOutlineBorders](../../aspose.cells/style/setoutlineborders/#setoutlineborders_1)(CellBorderType, Color) | Anahat kenarlarını ayarla. |
| [SetPatternColor](../../aspose.cells/style/setpatterncolor/)(BackgroundType, Color, Color) | Arka plan rengini ayarlar. |
| [SetTwoColorGradient](../../aspose.cells/style/settwocolorgradient/)(Color, Color, GradientStyleType, int) | Belirtilen doldurmayı iki renkli degradeye ayarlar. |
| [ToJson](../../aspose.cells/style/tojson/)() | `Style`'ı JSON yapı verisine dönüştür. |
| [Update](../../aspose.cells/style/update/)() | Adlandırılmış stili, bu adlandırılmış stili kullanan hücrelerin stillerine uygula. Stil üzerinde değişiklikleri tamamladıktan sonra "ok" düğmesine tıklamaya benzer şekilde çalışır. Yalnızca adlandırılmış stil için geçerlidir. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class StyleDemo
    {
        public static void StyleExample()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Çalışma sayfasından bir hücreye erişin
            Cell cell = worksheet.Cells["A1"];
            
            // Hücrenin stilini al
            Style style = cell.GetStyle();
            
            // Stilin çeşitli özelliklerini ayarla
            style.Font.Name = "Times New Roman";
            style.Font.Color = Color.Blue;
            style.BackgroundColor = Color.Yellow;
            style.ForegroundColor = Color.Red;
            style.Pattern = BackgroundType.Solid;
            style.HorizontalAlignment = TextAlignmentType.Center;
            style.VerticalAlignment = TextAlignmentType.Center;
            style.IsTextWrapped = true;
            style.IsLocked = true;
            style.Number = 15; // Date format
            style.IndentLevel = 2;
            style.RotationAngle = 45;
            style.IsFormulaHidden = true;
            style.ShrinkToFit = true;
            style.TextDirection = TextDirectionType.RightToLeft;
            style.IsJustifyDistributed = true;
            style.QuotePrefix = true;
            style.IsGradient = true;
            style.IsNumberFormatApplied = true;
            style.IsFontApplied = true;
            style.IsAlignmentApplied = true;
            style.IsBorderApplied = true;
            style.IsFillApplied = true;
            style.IsProtectionApplied = true;
            style.BackgroundArgbColor = Color.Yellow.ToArgb();
            style.ForegroundArgbColor = Color.Red.ToArgb();
            style.Custom = "0.00%";
            style.CultureCustom = "0.00%";
            
            // Stili hücreye ayarla
            cell.SetStyle(style);
            
            // Çalışma kitabını kaydedin
            workbook.Save("StyleExample.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


