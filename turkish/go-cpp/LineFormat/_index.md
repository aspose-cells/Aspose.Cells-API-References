---
title: "LineFormat Sınıfı"
linktitle: "LineFormat"
second_title: "C++ API Referansı aracılığıyla Go için Aspose.Cells"
description: "LineFormat sınıfı. Go dilinde lineformat'ı temsil eden nesneyi kapsüller."
type: docs
weight: 200
url: /tr/go-cpp/lineformat/
---

## LineFormat class

Çizginin tüm ayarlarını temsil eder.

```go

type LineFormat struct  {
	ptr unsafe.Pointer
}

```
## Yapıcılar

| Metot | Açıklama |
| --- | --- |
| [NewLineFormat](./newlineformat/) | Bir üst nesneden oluşturur. |

## Metotlar

| Metot | Açıklama |
| --- | --- |
| [IsNull](./isnull/) | Uygulama nesnesinin nullptr olup olmadığını kontrol eder. |
| [GetHashCode](./gethashcode/) | Karma kodu alır. |
| [Equals](./equals/) | Bu örneğin, belirtilen başka bir LineFormat nesnesiyle aynı değere sahip olup olmadığını belirler. |
| [GetCompoundType](./getcompoundtype/) | Satır birleşik tipini belirtir. |
| [SetCompoundType](./setcompoundtype/) | Satır birleşik tipini belirtir. |
| [GetDashStyle](./getdashstyle/) | Satır tire tipini belirtir. |
| [SetDashStyle](./setdashstyle/) | Satır tire tipini belirtir. |
| [GetCapType](./getcaptype/) | Bitiş kapaklarını belirtir. |
| [SetCapType](./setcaptype/) | Bitiş kapaklarını belirtir. |
| [GetJoinType](./getjointype/) | Satır birleşim tipini belirtir. |
| [SetJoinType](./setjointype/) | Satır birleşim tipini belirtir. |
| [GetBeginArrowheadStyle](./getbeginarrowheadstyle/) | Satırın başlangıç ok tipini alır ve ayarlar. |
| [SetBeginArrowheadStyle](./setbeginarrowheadstyle/) | Satırın başlangıç ok tipini alır ve ayarlar. |
| [GetBeginArrowheadWidth](./getbeginarrowheadwidth/) | Satırın başlangıç ok genişlik tipini alır ve ayarlar. |
| [SetBeginArrowheadWidth](./setbeginarrowheadwidth/) | Satırın başlangıç ok genişlik tipini alır ve ayarlar. |
| [GetBeginArrowheadLength](./getbeginarrowheadlength/) | Satırın başlangıç ok uzunluk tipini alır ve ayarlar. |
| [SetBeginArrowheadLength](./setbeginarrowheadlength/) | Satırın başlangıç ok uzunluk tipini alır ve ayarlar. |
| [GetEndArrowheadStyle](./getendarrowheadstyle/) | Satırın bitiş ok tipini alır ve ayarlar. |
| [SetEndArrowheadStyle](./setendarrowheadstyle/) | Satırın bitiş ok tipini alır ve ayarlar. |
| [GetEndArrowheadWidth](./getendarrowheadwidth/) | Satırın bitiş ok genişlik tipini alır ve ayarlar. |
| [SetEndArrowheadWidth](./setendarrowheadwidth/) | Satırın bitiş ok genişlik tipini alır ve ayarlar. |
| [GetEndArrowheadLength](./getendarrowheadlength/) | Satırın bitiş ok uzunluk tipini alır ve ayarlar. |
| [SetEndArrowheadLength](./setendarrowheadlength/) | Satırın bitiş ok uzunluk tipini alır ve ayarlar. |
| [GetWeight](./getweight/) | Çizginin ağırlığını puan biriminde alır veya ayarlar. |
| [SetWeight](./setweight/) | Çizginin ağırlığını puan biriminde alır veya ayarlar. |
| [GetFillType](./getfilltype/) | Dolgu tipini alır ve ayarlar |
| [SetFillType](./setfilltype/) | Dolgu tipini alır ve ayarlar |
| [GetTransparency](./gettransparency/) | Alanının şeffaflık derecesini 0.0 (opak) ile 1.0 (şeffaf) arasında bir değer olarak döndürür veya ayarlar. |
| [SetTransparency](./settransparency/) | Alanının şeffaflık derecesini 0.0 (opak) ile 1.0 (şeffaf) arasında bir değer olarak döndürür veya ayarlar. |
| [GetGradientFill](./getgradientfill/) | GradientFill nesnesini alır. |
| [GetTextureFill](./gettexturefill/) | TextureFill nesnesini alır. |
| [GetSolidFill](./getsolidfill/) | SolidFill nesnesini alır. |
| [GetPatternFill](./getpatternfill/) | PatternFill nesnesini alır. |
| [GetGradientColorType](./getgradientcolortype/) | Belirtilen dolgu için degrade renk tipini döndürür. |
| [GetGradientStyle](./getgradientstyle/) | Belirtilen dolgu için degrade stilini döndürür. |
| [GetGradientColor1](./getgradientcolor1/) | Belirtilen dolgu için degrade renk 1'i döndürür. |
| [GetGradientColor2](./getgradientcolor2/) | Belirtilen dolgu için degrade renk 2'yi döndürür. |
| [GetGradientDegree](./getgradientdegree/) | Belirtilen dolgu için degrade derecesini döndürür. Yalnızca Excel 2007 için geçerlidir. |
| [GetGradientVariant](./getgradientvariant/) | Belirtilen dolgu için degrade varyantını döndürür. Yalnızca Excel 2007 için geçerlidir. |
| [GetPresetColor](./getpresetcolor/) | Belirtilen doldurma için gradyan ön ayar rengini döndürür. |
| [SetOneColorGradient](./setonecolorgradient/) | Belirtilen doldurmayı tek renkli bir gradient olarak ayarlar. Yalnızca Excel 2007 için geçerlidir. |
| [SetTwoColorGradient_Color_Color_GradientStyleType_Int](./settwocolorgradient_color_color_gradientstyletype_int/) | Belirtilen doldurmayı iki renkli bir gradient olarak ayarlar. Yalnızca Excel 2007 için geçerlidir. |
| [SetPresetColorGradient](./setpresetcolorgradient/) | Belirtilen doldurmayı ön ayarlı renk gradyanına ayarlar. Yalnızca Excel 2007 için geçerlidir. |
| [GetTexture](./gettexture/) | Belirtilen doldurma için doku tipini temsil eder. |
| [SetTexture](./settexture/) | Belirtilen doldurma için doku tipini temsil eder. |
| [GetPattern](./getpattern/) | Bir alanın görüntü desenini temsil eder. |
| [SetPattern](./setpattern/) | Bir alanın görüntü desenini temsil eder. |
| [GetPictureFormatType](./getpictureformattype/) | Resim formatı tipini alır ve ayarlar. |
| [SetPictureFormatType](./setpictureformattype/) | Resim formatı tipini alır ve ayarlar. |
| [GetScale](./getscale/) | Resim formatı ölçeğini alır ve ayarlar. |
| [SetScale](./setscale/) | Resim formatı ölçeğini alır ve ayarlar. |
| [GetImageData](./getimagedata/) | Resim veri bilgisini alır ve ayarlar. |
| [SetImageData](./setimagedata/) | Resim veri bilgisini alır ve ayarlar. |
