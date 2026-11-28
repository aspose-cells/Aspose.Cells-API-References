---
title: "Enum StyleModifyFlag"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.StyleModifyFlag enum. Stil değiştirme bayrakları"
type: docs
url: /tr/net/aspose.cells/stylemodifyflag/
---
## StyleModifyFlag enumeration

Stil değiştirme bayrakları.

```csharp
public enum StyleModifyFlag
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| LeftBorder | `256` | Stil için sol kenarlığın değiştirilip değiştirilmediğini gösterir. |
| RightBorder | `512` | Stil için sağ kenarlığın değiştirilip değiştirilmediğini gösterir. |
| TopBorder | `1024` | Stil için üst kenarlığın değiştirilip değiştirilmediğini gösterir. |
| BottomBorder | `2048` | Stil için alt kenarlığın değiştirilip değiştirilmediğini gösterir. |
| DiagonalDownBorder | `4096` | Stil için çapraz aşağı kenarlığın değiştirilip değiştirilmediğini gösterir. |
| DiagonalUpBorder | `8192` | Stil için çapraz yukarı kenarlığın değiştirilip değiştirilmediğini gösterir. |
| HorizontalBorder | `32` | Stil için yatay kenarlığın değiştirilip değiştirilmediğini gösterir. Yalnızca koşullu biçimlendirme gibi dinamik stiller için. |
| VerticalBorder | `64` | Stil için dikey kenarlığın değiştirilip değiştirilmediğini gösterir. Yalnızca koşullu biçimlendirme gibi dinamik stiller için |
| SideBorders | `3840` | Dört kenar kenarını gösterir: LeftBorder, RightBorder, TopBorder ve BottomBorder. |
| Diagonal | `12288` | Çapraz kenarları gösterir: DiagonalDownBorder ve DiagonalUpBorder. |
| DynamicStyleBorders | `96` | Dinamik stilin kenarlarını gösterir: HorizontalBorder ve VerticalBorder. |
| Borders | `16224` | Stil için bir veya daha fazla kenarlığın (LeftBorder, RightBorder, TopBorder, BottomBorder, Diagonal, HorizontalBorder, VerticalBorder) değiştirilip değiştirilmediğini gösterir. |
| NumberFormat | `16384` | Numberformat'in değiştirilip değiştirilmediğini gösterir. |
| HorizontalAlignment | `32768` | Yatay hizalamanın değiştirilip değiştirilmediğini gösterir. |
| VerticalAlignment | `65536` | Dikey hizalamanın değiştirilip değiştirilmediğini gösterir. |
| Indent | `131072` | Girinti özelliğinin değiştirilip değiştirilmediğini gösterir. |
| Rotation | `262144` | Döndürme özelliğinin değiştirilip değiştirilmediğini gösterir. |
| WrapText | `524288` | Metni kaydırma özelliğinin değiştirilip değiştirilmediğini gösterir. |
| ShrinkToFit | `1048576` | Sığdırmak için küçültme özelliğinin değiştirilip değiştirilmediğini gösterir. |
| TextDirection | `2097152` | Metin yönü özelliğinin değiştirilip değiştirilmediğini gösterir. |
| RelativeIndent | `128` | Stil için göreceli girinti özelliğinin değiştirilip değiştirilmediğini gösterir. Yalnızca koşullu biçimlendirme gibi dinamik stiller için geçerlidir. |
| AlignmentSettings | `4161664` | Yatay hizalama, dikey hizalama vb. bir veya daha fazla hizalama ile ilgili özelliğin (HorizontalAlignment, VerticalAlignment, Rotation, WrapText, WrapText, Indent, ShrinkToFit, TextDirection, RelativeIndent) değiştirilip değiştirilmediğini gösterir. |
| Pattern | `4194304` | Gölgelendirme deseninin değiştirilip değiştirilmediğini gösterir. |
| ForegroundColor | `8388608` | Ön plan renginin değiştirilip değiştirilmediğini gösterir. |
| BackgroundColor | `16777216` | Arka plan renginin değiştirilip değiştirilmediğini gösterir. |
| CellShading | `29360128` | Desen, ön plan renginin, arka plan renginin gibi bir veya daha fazla gölgelendirme ile ilgili özelliğin (Pattern, ForegroundColor, BackgroundColor) değiştirilip değiştirilmediğini gösterir. |
| Locked | `67108864` | Kilitli özelliğinin değiştirilip değiştirilmediğini gösterir. |
| HideFormula | `134217728` | Formülü gizle özelliğinin değiştirilip değiştirilmediğini gösterir. |
| ProtectionSettings | `201326592` | Kilitli, HideFormula gibi bir veya daha fazla koruma ile ilgili özelliğin (Locked, HideFormula) değiştirilip değiştirilmediğini gösterir. |
| FontSize | `1` | Yazı tipi boyutunun değiştirilip değiştirilmediğini gösterir. |
| FontName | `2` | Yazı tipi adının değiştirilip değiştirilmediğini gösterir. |
| FontColor | `3` | Yazı tipi renginin değiştirilip değiştirilmediğini gösterir. |
| FontWeight | `4` | Yazı tipi kalınlığının değiştirilip değiştirilmediğini gösterir. |
| FontItalic | `5` | Yazı tipinin italik özelliğinin değiştirilip değiştirilmediğini gösterir. |
| FontUnderline | `6` | Yazı tipinin alt çizgi özelliğinin değiştirilip değiştirilmediğini gösterir. |
| FontStrike | `7` | Yazı tipinin üstü çizili özelliğinin değiştirilip değiştirilmediğini gösterir. |
| FontScript | `8` | Yazı tipinin alt simge veya üst simge özelliğinin değiştirilip değiştirilmediğini gösterir. |
| FontFamily | `9` | Yazı tipi ailesinin değiştirilip değiştirilmediğini gösterir. |
| FontCharset | `10` | Yazı tipinin karakter kümesinin değiştirilip değiştirilmediğini gösterir. |
| FontScheme | `11` | kullanılmıyor. |
| FontDirty | `12` | kullanılmıyor. |
| FontSpellingError | `13` | kullanılmıyor. |
| FontUFillTx | `14` | kullanılmıyor. |
| FontSpacing | `15` | kullanılmıyor. |
| FontKerning | `16` | kullanılmıyor. |
| FontEqualize | `17` | kullanılmıyor. |
| FontCap | `18` | kullanılmıyor. |
| FontVerticalText | `19` |  |
| Font | `31` | Stil yazı tipinin bir veya daha fazla özelliğinin değiştirilip değiştirilmediğini gösterir. |
| All | `234881023` | Stil için değiştirilebilecek tüm özellikler. |
| None | `0` | Hiçbir özellik belirtilmemiştir. |

### Açıklamalar

Kullanıcı rahatlığı için birden fazla özelliğin kombinasyonları tanımlanmıştır. Bir stil için bunların değiştirilip değiştirilmediği kontrol edildiğinde, döndürülen değer kombinasyondaki bir veya daha fazla özelliğin değiştirilip değiştirilmediğini gösterir.

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class StyleModifyFlagDemo
    {
        public static void StyleModifyFlagExample()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();

            // Çalışma kitabına yeni bir çalışma sayfası ekle
            Worksheet worksheet = workbook.Worksheets[0];

            // Çalışma sayfasında bazı değerleri ayarla
            worksheet.Cells["A1"].PutValue("Sample Text");
            worksheet.Cells["A2"].PutValue(123.45);

            // Yeni bir stil oluştur
            Style style = workbook.CreateStyle();
            style.Font.Name = "Arial";
            style.Font.Size = 12;
            style.Font.Color = System.Drawing.Color.Blue;
            style.HorizontalAlignment = TextAlignmentType.Center;
            style.VerticalAlignment = TextAlignmentType.Center;

            // Stili bir hücreye uygula
            worksheet.Cells["A1"].SetStyle(style);

            // Hangi stil özelliklerinin değiştirildiğini kontrol et
            bool isFontModified = style.IsModified(StyleModifyFlag.Font);
            bool isFontSizeModified = style.IsModified(StyleModifyFlag.FontSize);
            bool isFontColorModified = style.IsModified(StyleModifyFlag.FontColor);
            bool isHorizontalAlignmentModified = style.IsModified(StyleModifyFlag.HorizontalAlignment);

            // Sonuçları çıktı olarak ver.
            Console.WriteLine("Font Modified: " + isFontModified);
            Console.WriteLine("Font Size Modified: " + isFontSizeModified);
            Console.WriteLine("Font Color Modified: " + isFontColorModified);
            Console.WriteLine("Horizontal Alignment Modified: " + isHorizontalAlignmentModified);

            // Çalışma kitabını kaydedin
            workbook.Save("StyleModifyFlagExample.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


