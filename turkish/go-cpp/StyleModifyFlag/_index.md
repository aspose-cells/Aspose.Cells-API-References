---
title: "StyleModifyFlag Enum'ı"
linktitle: "StyleModifyFlag"
second_title: "C++ API Referansı aracılığıyla Go için Aspose.Cells"
description: "StyleModifyFlag enum. Go'da stylemodifyflag'i temsil eden nesneyi kapsüller."
type: docs
weight: 200
url: /tr/go-cpp/stylemodifyflag/
---

## StyleModifyFlag Enum

Stil değiştirilmiş bayrakları.

```go

type StyleModifyFlag int32


```

## Alanlar

| Alan | Açıklama |
| --- | --- |
| [LeftBorder](./leftborder/) | Stil için sol kenarın değiştirilip değiştirilmediğini gösterir. |
| [RightBorder](./rightborder/) | Stil için sağ kenarın değiştirilip değiştirilmediğini gösterir. |
| [TopBorder](./topborder/) | Stil için üst kenarın değiştirilip değiştirilmediğini gösterir. |
| [BottomBorder](./bottomborder/) | Stil için alt kenarın değiştirilip değiştirilmediğini gösterir. |
| [DiagonalDownBorder](./diagonaldownborder/) | Stil için çapraz aşağı kenarın değiştirilip değiştirilmediğini gösterir. |
| [DiagonalUpBorder](./diagonalupborder/) | Stil için çapraz yukarı kenarın değiştirilip değiştirilmediğini gösterir. |
| [HorizontalBorder](./horizontalborder/) | Stil için yatay kenarın değiştirilip değiştirilmediğini gösterir. Yalnızca koşullu biçimlendirme gibi dinamik stiller için. |
| [VerticalBorder](./verticalborder/) | Stil için dikey kenarın değiştirilip değiştirilmediğini gösterir. Yalnızca koşullu biçimlendirme gibi dinamik stiller için. |
| [SideBorders](./sideborders/) | Dört kenar sınırını gösterir: <see cref=\"LeftBorder\"/>,<see cref=\"RightBorder\"/>, <see cref=\"TopBorder\"/> ve <see cref=\"BottomBorder\"/>. |
| [Diagonal](./diagonal/) | Çapraz kenarları gösterir: <see cref="DiagonalDownBorder"/> ve <see cref="DiagonalUpBorder"/>. |
| [DynamicStyleBorders](./dynamicstyleborders/) | Dinamik stilin kenarlarını gösterir: <see cref="HorizontalBorder"/> ve <see cref="VerticalBorder"/>. |
| [Borders](./borders/) | Stil için bir veya daha fazla kenarın (<see cref="LeftBorder"/>,<see cref="RightBorder"/>, <see cref="TopBorder"/>, <see cref="BottomBorder"/>,<see cref="Diagonal"/>, <see cref="HorizontalBorder"/>, <see cref="VerticalBorder"/>) değiştirilip değiştirilmediğini gösterir. |
| [NumberFormat](./numberformat/) | Sayı biçiminin değiştirilip değiştirilmediğini gösterir. |
| [HorizontalAlignment](./horizontalalignment/) | Yatay hizalamanın değiştirilip değiştirilmediğini gösterir. |
| [VerticalAlignment](./verticalalignment/) | Dikey hizalamanın değiştirilip değiştirilmediğini gösterir. |
| [Indent](./indent/) | Girinti özelliğinin değiştirilip değiştirilmediğini gösterir. |
| [Rotation](./rotation/) | Rotasyon özelliğinin değiştirilip değiştirilmediğini gösterir. |
| [WrapText](./wraptext/) | Metni kaydırma özelliğinin değiştirilip değiştirilmediğini gösterir. |
| [ShrinkToFit](./shrinktofit/) | Uygun boyuta küçültme özelliğinin değiştirilip değiştirilmediğini gösterir. |
| [TextDirection](./textdirection/) | Metin yönü özelliğinin değiştirilip değiştirilmediğini gösterir. |
| [RelativeIndent](./relativeindent/) | Stil için göreceli girinti özelliğinin değiştirilip değiştirilmediğini gösterir. Yalnızca koşullu biçimlendirme gibi dinamik stiller için. |
| [AlignmentSettings](./alignmentsettings/) | Bir veya daha fazla hizalama ile ilgili özelliklerin(<see cref=\"HorizontalAlignment\"/>,<see cref=\"VerticalAlignment\"/>, <see cref=\"Rotation\"/>, <see cref=\"WrapText\"/>,<see cref=\"WrapText\"/>, <see cref=\"Indent\"/>, <see cref=\"ShrinkToFit\"/>, <see cref=\"TextDirection\"/>,<see cref=\"RelativeIndent\"/>) değiştirilip değiştirilmediğini gösterir. |
| [Pattern](./pattern/) | Gölgelendirme deseninin değiştirilip değiştirilmediğini gösterir. |
| [ForegroundColor](./foregroundcolor/) | Ön plan renginin değiştirilip değiştirilmediğini gösterir. |
| [BackgroundColor](./backgroundcolor/) | Arka plan renginin değiştirilip değiştirilmediğini gösterir. |
| [CellShading](./cellshading/) | Bir veya daha fazla gölgelendirme ile ilgili özelliklerin(<see cref=\"Pattern\"/>,<see cref=\"ForegroundColor\"/>, <see cref=\"BackgroundColor\"/>) değiştirilip değiştirilmediğini gösterir. |
| [Locked](./locked/) | Kilitli özelliğinin değiştirilip değiştirilmediğini gösterir. |
| [HideFormula](./hideformula/) | Formülü gizleme özelliğinin değiştirilip değiştirilmediğini gösterir. |
| [ProtectionSettings](./protectionsettings/) | Bir veya daha fazla koruma ile ilgili özelliklerin(<see cref=\"Locked\"/>,<see cref=\"HideFormula\"/>) değiştirilip değiştirilmediğini gösterir. |
| [FontSize](./fontsize/) | Yazı tipi boyutunun değiştirilip değiştirilmediğini gösterir. |
| [FontName](./fontname/) | Yazı tipi adının değiştirilip değiştirilmediğini gösterir. |
| [FontColor](./fontcolor/) | Yazı tipi renginin değiştirilip değiştirilmediğini gösterir. |
| [FontWeight](./fontweight/) | Yazı tipi kalınlığının değiştirilip değiştirilmediğini gösterir. |
| [FontItalic](./fontitalic/) | Yazı tipinin italik özelliğinin değiştirilip değiştirilmediğini gösterir. |
| [FontUnderline](./fontunderline/) | Yazı tipinin alt çizgi özelliğinin değiştirilip değiştirilmediğini gösterir. |
| [FontStrike](./fontstrike/) | Yazı tipinin üstü çizili özelliğinin değiştirilip değiştirilmediğini gösterir. |
| [FontScript](./fontscript/) | Yazı tipinin alt simge veya üst simge özelliğinin değiştirilip değiştirilmediğini gösterir. |
| [FontFamily](./fontfamily/) | Yazı tipi ailesinin değiştirilip değiştirilmediğini gösterir. |
| [FontCharset](./fontcharset/) | Yazı tipinin karakter kümesinin değiştirilip değiştirilmediğini gösterir. |
| [FontScheme](./fontscheme/) | kullanılmamış. |
| [FontDirty](./fontdirty/) | kullanılmamış. |
| [FontSpellingError](./fontspellingerror/) | kullanılmamış. |
| [FontUFillTx](./fontufilltx/) | kullanılmamış. |
| [FontSpacing](./fontspacing/) | kullanılmamış. |
| [FontKerning](./fontkerning/) | kullanılmamış. |
| [FontEqualize](./fontequalize/) | kullanılmamış. |
| [FontCap](./fontcap/) | kullanılmamış. |
|[FontVerticalText](./fontverticaltext/) |  | 
| [Font](./font/) | Stil yazı tipinin bir veya daha fazla özelliğinin değiştirilip değiştirilmediğini gösterir. |
| [All](./all/) | Stil için değiştirilebilecek tüm özellikler. |
| [None](./none/) | Hiçbir özellik belirtilmemiştir. |
