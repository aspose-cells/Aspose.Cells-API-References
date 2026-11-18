---
title: "SvgImageOptions Sınıfı"
linktitle: "SvgImageOptions"
second_title: "C++ API Referansı aracılığıyla Go için Aspose.Cells"
description: "SvgImageOptions sınıfı. Go dilinde svgimageoptions nesnesini temsil eden nesneyi kapsüller."
type: docs
weight: 200
url: /tr/go-cpp/svgimageoptions/
---

## SvgImageOptions class

Svg görüntüsü oluşturma seçenekleri.

```go

type SvgImageOptions struct  {
	ptr unsafe.Pointer
}

```
## Yapıcılar

| Metot | Açıklama |
| --- | --- |
| [NewSvgImageOptions](./newsvgimageoptions/) | Yapıcı. |
| [NewSvgImageOptions_ImageOrPrintOptions](./newsvgimageoptions_imageorprintoptions/) | Bir üst nesneden oluşturur. |

## Metotlar

| Metot | Açıklama |
| --- | --- |
| [IsNull](./isnull/) | Uygulama nesnesinin nullptr olup olmadığını kontrol eder. |
| [GetImageType](./getimagetype/) | Üretilen görüntülerin formatını alır veya ayarlar. varsayılan değer: PNG. |
| [SetImageType](./setimagetype/) | Üretilen görüntülerin formatını alır veya ayarlar. varsayılan değer: PNG. |
| [GetFitToViewPort](./getfittoviewport/) | Bu özellik true ise, üretilen svg görünüm alanına sığacaktır. |
| [SetFitToViewPort](./setfittoviewport/) | Bu özellik true ise, üretilen svg görünüm alanına sığacaktır. |
| [GetCssPrefix](./getcssprefix/) | svg içindeki css adının önekini alır veya ayarlar, varsayılan değer boş dizedir. |
| [SetCssPrefix](./setcssprefix/) | svg içindeki css adının önekini alır veya ayarlar, varsayılan değer boş dizedir. |
| [GetEmbeddedFontType](./getembeddedfonttype/) | Svg içinde gömülü olan yazı tipi türünü alır veya ayarlar. |
| [SetEmbeddedFontType](./setembeddedfonttype/) | Svg içinde gömülü olan yazı tipi türünü alır veya ayarlar. |
| [SetPrintWithStatusDialog](./setprintwithstatusdialog/) | Eğer PrintWithStatusDialog = true ise, mevcut yazdırma durumunu gösteren bir iletişim kutusu görüntülenir; aksi takdirde böyle bir iletişim kutusu gösterilmez. |
| [GetPrintWithStatusDialog](./getprintwithstatusdialog/) | Eğer PrintWithStatusDialog = true ise, mevcut yazdırma durumunu gösteren bir iletişim kutusu görüntülenir; aksi takdirde böyle bir iletişim kutusu gösterilmez. |
| [GetHorizontalResolution](./gethorizontalresolution/) | Üretilen görüntüler için yatay çözünürlüğü alır veya ayarlar, inç başına nokta (dpi) cinsinden. |
| [SetHorizontalResolution](./sethorizontalresolution/) | Üretilen görüntüler için yatay çözünürlüğü alır veya ayarlar, inç başına nokta (dpi) cinsinden. |
| [GetVerticalResolution](./getverticalresolution/) | Üretilen görüntüler için dikey çözünürlüğü alır veya ayarlar, inç başına nokta (dpi) cinsinden. |
| [SetVerticalResolution](./setverticalresolution/) | Üretilen görüntüler için dikey çözünürlüğü alır veya ayarlar, inç başına nokta (dpi) cinsinden. |
| [GetTiffCompression](./gettiffcompression/) | Sayfaları <c>Tiff</c> formatında kaydederken uygulanacak sıkıştırma türünü alır veya ayarlar. |
| [SetTiffCompression](./settiffcompression/) | Sayfaları <c>Tiff</c> formatında kaydederken uygulanacak sıkıştırma türünü alır veya ayarlar. |
| [GetTiffColorDepth](./gettiffcolordepth/) | Sayfaları <c>Tiff</c> formatında kaydederken uygulanacak bit derinliğini alır veya ayarlar. |
| [SetTiffColorDepth](./settiffcolordepth/) | Sayfaları <c>Tiff</c> formatında kaydederken uygulanacak bit derinliğini alır veya ayarlar. |
| [GetTiffBinarizationMethod](./gettiffbinarizationmethod/) | ImageType Tiff ve TiffCompression Ccitt3 veya Ccitt4 olduğunda görüntüleri 1 bpp formatına dönüştürürken kullanılan yöntemi alır veya ayarlar. |
| [SetTiffBinarizationMethod](./settiffbinarizationmethod/) | ImageType Tiff ve TiffCompression Ccitt3 veya Ccitt4 olduğunda görüntüleri 1 bpp formatına dönüştürürken kullanılan yöntemi alır veya ayarlar. |
| [GetPrintingPage](./getprintingpage/) | Hangi sayfaların yazdırılmayacağını gösterir. |
| [SetPrintingPage](./setprintingpage/) | Hangi sayfaların yazdırılmayacağını gösterir. |
| [GetQuality](./getquality/) | Sayfaları <c>Jpeg</c> formatında kaydederken uygulanacak, üretilen görüntülerin kalitesini belirleyen bir değeri alır veya ayarlar. Varsayılan değer 100'tür. |
| [SetQuality](./setquality/) | Sayfaları <c>Jpeg</c> formatında kaydederken uygulanacak, üretilen görüntülerin kalitesini belirleyen bir değeri alır veya ayarlar. Varsayılan değer 100'tür. |
| [GetOnePagePerSheet](./getonepagepersheet/) | OnePagePerSheet true ise, bir sayfanın tüm içeriği sonuçta yalnızca bir sayfaya çıktılanır. Sayfa ayarının kağıt boyutu geçersiz olur ve sayfa ayarının diğer ayarları hâlâ etkili olur. |
| [SetOnePagePerSheet](./setonepagepersheet/) | OnePagePerSheet true ise, bir sayfanın tüm içeriği sonuçta yalnızca bir sayfaya çıktılanır. Sayfa ayarının kağıt boyutu geçersiz olur ve sayfa ayarının diğer ayarları hâlâ etkili olur. |
| [GetAllColumnsInOnePagePerSheet](./getallcolumnsinonepagepersheet/) | Eğer AllColumnsInOnePagePerSheet true ise, bir sayfanın tüm sütun içeriği sonuçta yalnızca bir sayfaya çıkacaktır. pagesetup'ın kağıt boyutu genişliği geçersiz olur, ancak pagesetup'ın diğer ayarları etkili olmaya devam eder. |
| [SetAllColumnsInOnePagePerSheet](./setallcolumnsinonepagepersheet/) | Eğer AllColumnsInOnePagePerSheet true ise, bir sayfanın tüm sütun içeriği sonuçta yalnızca bir sayfaya çıkacaktır. pagesetup'ın kağıt boyutu genişliği geçersiz olur, ancak pagesetup'ın diğer ayarları etkili olmaya devam eder. |
| [GetDrawObjectEventHandler](./getdrawobjecteventhandler/) | Render ederken DrawObject ve Bound'ı elde etmek için bu arayüzü uygular. |
| [SetDrawObjectEventHandler](./setdrawobjecteventhandler/) | Render ederken DrawObject ve Bound'ı elde etmek için bu arayüzü uygular. |
| [GetOnlyArea](./getonlyarea/) | Bu özellik doğru ise, bir Area çıktılanacak ve ölçek etkili olmayacaktır. |
| [SetOnlyArea](./setonlyarea/) | Bu özellik doğru ise, bir Area çıktılanacak ve ölçek etkili olmayacaktır. |
| [GetTransparent](./gettransparent/) | Oluşturulan görüntünün arka planının şeffaf olup olmadığını gösterir. |
| [SetTransparent](./settransparent/) | Oluşturulan görüntünün arka planının şeffaf olup olmadığını gösterir. |
| [SetIsFontSubstitutionCharGranularity](./setisfontsubstitutionchargranularity/) | Hücre yazı tipi karakterle uyumlu olmadığında yalnızca karakterin yazı tipini değiştirmeyi gösterir. |
| [IsFontSubstitutionCharGranularity](./isfontsubstitutionchargranularity/) | Hücre yazı tipi karakterle uyumlu olmadığında yalnızca karakterin yazı tipini değiştirmeyi gösterir. |
| [SetPageIndex](./setpageindex/) | Kaydedilecek ilk sayfanın 0 tabanlı dizinini alır veya ayarlar. |
| [GetPageIndex](./getpageindex/) | Kaydedilecek ilk sayfanın 0 tabanlı dizinini alır veya ayarlar. |
| [SetPageCount](./setpagecount/) | Kaydedilecek sayfa sayısını alır veya ayarlar. |
| [GetPageCount](./getpagecount/) | Kaydedilecek sayfa sayısını alır veya ayarlar. |
| [SetDesiredSize](./setdesiredsize/) | Görüntünün istenen genişlik ve yüksekliğini ayarlar. |
| [IsOptimized](./isoptimized/) | Çıktı öğelerinin optimize edilip edilmeyeceğini gösterir. |
| [SetIsOptimized](./setisoptimized/) | Çıktı öğelerinin optimize edilip edilmeyeceğini gösterir. |
| [GetDefaultFont](./getdefaultfont/) | Excel'deki karakterler Unicode olduğunda ve hücre stilinde doğru yazı tipi ayarlanmamışsa, PDF ve görüntüde blok olarak görünebilirler. MingLiu veya MS Gothic gibi bir DefaultFont ayarlayarak bu karakterlerin gösterilmesini sağlayın. Bu özellik ayarlanmamışsa, Aspose.Cells bu Unicode karakterleri göstermek için sistemin varsayılan yazı tipini kullanacaktır. |
| [SetDefaultFont](./setdefaultfont/) | Excel'deki karakterler Unicode olduğunda ve hücre stilinde doğru yazı tipi ayarlanmamışsa, PDF ve görüntüde blok olarak görünebilirler. MingLiu veya MS Gothic gibi bir DefaultFont ayarlayarak bu karakterlerin gösterilmesini sağlayın. Bu özellik ayarlanmamışsa, Aspose.Cells bu Unicode karakterleri göstermek için sistemin varsayılan yazı tipini kullanacaktır. |
| [GetCheckWorkbookDefaultFont](./getcheckworkbookdefaultfont/) | Excel'deki karakterler Unicode olduğunda ve hücre stilinde doğru yazı tipi ayarlanmamışsa, PDF ve görüntüde blok olarak görünebilirler. Bu özelliği true olarak ayarlayarak önce çalışma kitabının varsayılan yazı tipini kullanıp bu karakterleri göstermeyi deneyin. |
| [SetCheckWorkbookDefaultFont](./setcheckworkbookdefaultfont/) | Excel'deki karakterler Unicode olduğunda ve hücre stilinde doğru yazı tipi ayarlanmamışsa, PDF ve görüntüde blok olarak görünebilirler. Bu özelliği true olarak ayarlayarak önce çalışma kitabının varsayılan yazı tipini kullanıp bu karakterleri göstermeyi deneyin. |
| [GetOutputBlankPageWhenNothingToPrint](./getoutputblankpagewhennothingtoprint/) | Yazdırılacak bir şey olmadığında boş bir sayfa çıktılanıp çıktılanmayacağını gösterir. |
| [SetOutputBlankPageWhenNothingToPrint](./setoutputblankpagewhennothingtoprint/) | Yazdırılacak bir şey olmadığında boş bir sayfa çıktılanıp çıktılanmayacağını gösterir. |
| [GetGridlineType](./getgridlinetype/) | Kılavuz çizgi tipini alır veya ayarlar. |
| [SetGridlineType](./setgridlinetype/) | Kılavuz çizgi tipini alır veya ayarlar. |
| [GetGridlineColor](./getgridlinecolor/) | Izgara çizgi rengini alır veya ayarlar. |
| [SetGridlineColor](./setgridlinecolor/) | Izgara çizgi rengini alır veya ayarlar. |
| [GetTextCrossType](./gettextcrosstype/) | Metin genişliği hücre genişliğinden büyük olduğunda gösterilen metin tipini alır veya ayarlar. |
| [SetTextCrossType](./settextcrosstype/) | Metin genişliği hücre genişliğinden büyük olduğunda gösterilen metin tipini alır veya ayarlar. |
| [GetDefaultEditLanguage](./getdefaulteditlanguage/) | Varsayılan düzenleme dilini alır veya ayarlar. |
| [SetDefaultEditLanguage](./setdefaulteditlanguage/) | Varsayılan düzenleme dilini alır veya ayarlar. |
| [GetSheetSet](./getsheetset/) | Renderlenecek sayfaları alır veya ayarlar. Varsayılan, çalışma kitabındaki tüm görünür sayfalardır: Aspose.Cells.Rendering.SheetSet.Visible. |
| [SetSheetSet](./setsheetset/) | Renderlenecek sayfaları alır veya ayarlar. Varsayılan, çalışma kitabındaki tüm görünür sayfalardır: Aspose.Cells.Rendering.SheetSet.Visible. |
| [GetEmfRenderSetting](./getemfrendersetting/) | Kaynak dosyada Emf metafilelerinin işlenmesi için ayar. |
| [SetEmfRenderSetting](./setemfrendersetting/) | Kaynak dosyada Emf metafilelerinin işlenmesi için ayar. |
| [GetCustomRenderSettings](./getcustomrendersettings/) | Renderleme sırasında özel ayarları alır veya ayarlar. |
| [SetCustomRenderSettings](./setcustomrendersettings/) | Renderleme sırasında özel ayarları alır veya ayarlar. |
