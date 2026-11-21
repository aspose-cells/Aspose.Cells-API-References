---
title: "SvgImageOptions"
second_title: "Aspose.Cells for Java API Referansı"
description: "Svg görüntüsü oluşturma seçenekleri."
type: docs
url: /tr/java/com.aspose.cells/svgimageoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.ImageOrPrintOptions](../../com.aspose.cells/imageorprintoptions)
```
public class SvgImageOptions extends ImageOrPrintOptions
```

Svg görüntüsü oluşturma seçenekleri.
## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [SvgImageOptions()](#SvgImageOptions--) | Yapıcı. |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAllColumnsInOnePagePerSheet()](#getAllColumnsInOnePagePerSheet--) | AllColumnsInOnePagePerSheet true ise, bir sayfadaki tüm sütun içeriği sonuçta yalnızca bir sayfaya çıktılanır. |
| [getChartImageType()](#getChartImageType--) | Dönüştürürken grafik görüntü türünü belirtin. |
| [getCheckWorkbookDefaultFont()](#getCheckWorkbookDefaultFont--) | Excel'deki karakterler Unicode olduğunda ve hücre stilinde doğru yazı tipi ayarlanmamışsa, PDF ve görüntüde blok olarak görünebilirler. |
| [getClass()](#getClass--) |  |
| [getCssPrefix()](#getCssPrefix--) | Svg içinde css adının önekini alır, varsayılan değer boş dizedir. |
| [getCustomRenderSettings()](#getCustomRenderSettings--) | Renderleme sırasında özel ayarları alır. |
| [getDefaultEditLanguage()](#getDefaultEditLanguage--) | Varsayılan düzenleme dilini alır. |
| [getDefaultFont()](#getDefaultFont--) | Excel'deki karakterler Unicode olduğunda ve hücre stilinde doğru yazı tipi ayarlanmamışsa, PDF ve görüntüde blok olarak görünebilirler. |
| [getDrawObjectEventHandler()](#getDrawObjectEventHandler--) | Render işlemi sırasında DrawObject ve Bound elde etmek için bu arayüzü uygular. |
| [getEmbeddedFontType()](#getEmbeddedFontType--) | Svg içinde gömülü olan yazı tipinin türünü alır. |
| [getEmbededImageNameInSvg()](#getEmbededImageNameInSvg--) | Svg içinde gömülü görüntünün dosya adını belirtin. |
| [getEmfRenderSetting()](#getEmfRenderSetting--) | Kaynak dosyada Emf meta dosyalarını işleme ayarı. |
| [getFitToViewPort()](#getFitToViewPort--) | Bu özellik doğruysa, oluşturulan svg görünüm alanına sığar. |
| [getGridlineColor()](#getGridlineColor--) | Izgara çizgi rengini alır. |
| [getGridlineType()](#getGridlineType--) | Izgara çizgisi tipini alır. |
| [getHorizontalResolution()](#getHorizontalResolution--) | Oluşturulan görüntüler için yatay çözünürlüğü, inç başına nokta cinsinden alır. |
| [getImageType()](#getImageType--) | Oluşturulan görüntülerin biçimini alır. |
| [getOnePagePerSheet()](#getOnePagePerSheet--) | OnePagePerSheet true ise, bir sayfanın tüm içeriği sonuçta yalnızca bir sayfaya çıktılanır. |
| [getOnlyArea()](#getOnlyArea--) | Bu özellik doğruysa, bir Alan çıktılanır ve ölçek etkili olmaz. |
| [getOutputBlankPageWhenNothingToPrint()](#getOutputBlankPageWhenNothingToPrint--) | Yazdırılacak bir şey olmadığında boş sayfa çıktısı verilip verilmeyeceğini gösterir. |
| [getPageCount()](#getPageCount--) | Kaydedilecek sayfa sayısını alır. |
| [getPageIndex()](#getPageIndex--) | Kaydedilecek ilk sayfanın 0 tabanlı indeksini alır. |
| [getPageSavingCallback()](#getPageSavingCallback--) | Sayfa kaydetme sürecinin ilerlemesini kontrol/indike eder. |
| [getPrintWithStatusDialog()](#getPrintWithStatusDialog--) | PrintWithStatusDialog = true ise, mevcut yazdırma durumunu gösteren bir iletişim kutusu görüntülenir. |
| [getPrintingPage()](#getPrintingPage--) | Hangi sayfaların yazdırılmayacağını gösterir. |
| [getQuality()](#getQuality--) | Sayfaları `Jpeg` biçiminde kaydederken yalnızca uygulanacak, oluşturulan görüntülerin kalitesini belirleyen bir değeri alır. |
| [getSVGFitToViewPort()](#getSVGFitToViewPort--) | Bu özellik doğruysa, oluşturulan svg görünüm alanına sığar. |
| [getSaveFormat()](#getSaveFormat--) | Çıktı dosya biçimi türünü alır, Tiff/XPS desteklenir. |
| [getSheetSet()](#getSheetSet--) | Render edilecek sayfaları alır. |
| [getSvgCssPrefix()](#getSvgCssPrefix--) | Svg içinde css adının önekini alır, varsayılan değer boş dizedir. |
| [getTextCrossType()](#getTextCrossType--) | Metin genişliği hücre genişliğinden büyük olduğunda görüntüleme metin türünü alır. |
| [getTiffColorDepth()](#getTiffColorDepth--) | `Tiff` biçiminde sayfaları kaydederken yalnızca uygulanacak bit derinliğini alır. |
| [getTiffCompression()](#getTiffCompression--) | `Tiff` biçiminde sayfaları kaydederken yalnızca uygulanacak sıkıştırma türünü alır. |
| [getTiffPhotometricInterpretation()](#getTiffPhotometricInterpretation--) | `Tiff` biçiminde sayfaları kaydederken yalnızca uygulanacak FotometrikYorumlama türünü alır. |
| [getTransparent()](#getTransparent--) | Oluşturulan görüntünün arka planının şeffaf olup olmadığını belirtir. |
| [getVerticalResolution()](#getVerticalResolution--) | Oluşturulan görüntüler için dikey çözünürlüğü, inç başına nokta cinsinden alır. |
| [getWarningCallback()](#getWarningCallback--) | Uyarı geri çağrısını alır. |
| [hashCode()](#hashCode--) |  |
| [isCellAutoFit()](#isCellAutoFit--) | Hücrelerin genişlik ve yüksekliğinin hücre değeriyle otomatik olarak ayarlanıp ayarlanmayacağını belirtir. |
| [isFontSubstitutionCharGranularity()](#isFontSubstitutionCharGranularity--) | Hücre yazı tipi uyumlu olmadığında yalnızca karakterin yazı tipinin değiştirilip değiştirilmeyeceğini gösterir. |
| [isOptimized()](#isOptimized--) | Çıktı öğelerinin optimize edilip edilmeyeceğini belirtir. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAllColumnsInOnePagePerSheet(boolean value)](#setAllColumnsInOnePagePerSheet-boolean-) | AllColumnsInOnePagePerSheet true ise, bir sayfadaki tüm sütun içeriği sonuçta yalnızca bir sayfaya çıktılanır. |
| [setCellAutoFit(boolean value)](#setCellAutoFit-boolean-) | Hücrelerin genişlik ve yüksekliğinin hücre değeriyle otomatik olarak ayarlanıp ayarlanmayacağını belirtir. |
| [setChartImageType(ImageFormat value)](#setChartImageType-com.aspose.cells.ImageFormat-) | Dönüştürürken grafik görüntü türünü belirtin. |
| [setCheckWorkbookDefaultFont(boolean value)](#setCheckWorkbookDefaultFont-boolean-) | Excel'deki karakterler Unicode olduğunda ve hücre stilinde doğru yazı tipi ayarlanmamışsa, PDF ve görüntüde blok olarak görünebilirler. |
| [setCssPrefix(String value)](#setCssPrefix-java.lang.String-) | Svg içinde css adının önekini ayarlar, varsayılan değer boş dizedir. |
| [setCustomRenderSettings(CustomRenderSettings value)](#setCustomRenderSettings-com.aspose.cells.CustomRenderSettings-) | Renderleme sırasında özel ayarları belirler. |
| [setDefaultEditLanguage(int value)](#setDefaultEditLanguage-int-) | Varsayılan düzenleme dilini ayarlar. |
| [setDefaultFont(String value)](#setDefaultFont-java.lang.String-) | Excel'deki karakterler Unicode olduğunda ve hücre stilinde doğru yazı tipi ayarlanmamışsa, PDF ve görüntüde blok olarak görünebilirler. |
| [setDesiredSize(int desiredWidth, int desiredHeight)](#setDesiredSize-int-int-) | Görüntünün istenen genişlik ve yüksekliğini ayarlar. |
| [setDesiredSize(int desiredWidth, int desiredHeight, boolean keepAspectRatio)](#setDesiredSize-int-int-boolean-) | Görüntünün istenen genişlik ve yüksekliğini ayarlar. |
| [setDrawObjectEventHandler(DrawObjectEventHandler value)](#setDrawObjectEventHandler-com.aspose.cells.DrawObjectEventHandler-) | Render işlemi sırasında DrawObject ve Bound elde etmek için bu arayüzü uygular. |
| [setEmbeddedFontType(int value)](#setEmbeddedFontType-int-) | Svg içinde gömülü olan yazı tipinin türünü ayarlar. |
| [setEmbededImageNameInSvg(String value)](#setEmbededImageNameInSvg-java.lang.String-) | Svg içinde gömülü görüntünün dosya adını belirtin. |
| [setEmfRenderSetting(int value)](#setEmfRenderSetting-int-) | Kaynak dosyada Emf meta dosyalarını işleme ayarı. |
| [setFitToViewPort(boolean value)](#setFitToViewPort-boolean-) | Bu özellik doğruysa, oluşturulan svg görünüm alanına sığar. |
| [setFontSubstitutionCharGranularity(boolean value)](#setFontSubstitutionCharGranularity-boolean-) | Hücre yazı tipi uyumlu olmadığında yalnızca karakterin yazı tipinin değiştirilip değiştirilmeyeceğini gösterir. |
| [setGridlineColor(Color value)](#setGridlineColor-com.aspose.cells.Color-) | Izgara çizgi rengini ayarlar. |
| [setGridlineType(int value)](#setGridlineType-int-) | Kılavuz çizgi tipini ayarlar. |
| [setHorizontalResolution(int value)](#setHorizontalResolution-int-) | Oluşturulan görüntüler için yatay çözünürlüğü nokta başına düşen inç cinsinden ayarlar. |
| [setImageType(int value)](#setImageType-int-) | Oluşturulan görüntülerin formatını ayarlar. |
| [setOnePagePerSheet(boolean value)](#setOnePagePerSheet-boolean-) | OnePagePerSheet true ise, bir sayfanın tüm içeriği sonuçta yalnızca bir sayfaya çıktılanır. |
| [setOnlyArea(boolean value)](#setOnlyArea-boolean-) | Bu özellik doğruysa, bir Alan çıktılanır ve ölçek etkili olmaz. |
| [setOptimized(boolean value)](#setOptimized-boolean-) | Çıktı öğelerinin optimize edilip edilmeyeceğini belirtir. |
| [setOutputBlankPageWhenNothingToPrint(boolean value)](#setOutputBlankPageWhenNothingToPrint-boolean-) | Yazdırılacak bir şey olmadığında boş sayfa çıktısı verilip verilmeyeceğini gösterir. |
| [setPageCount(int value)](#setPageCount-int-) | Kaydedilecek sayfa sayısını ayarlar. |
| [setPageIndex(int value)](#setPageIndex-int-) | Kaydedilecek ilk sayfanın 0 tabanlı indeksini ayarlar. |
| [setPageSavingCallback(IPageSavingCallback value)](#setPageSavingCallback-com.aspose.cells.IPageSavingCallback-) | Sayfa kaydetme sürecinin ilerlemesini kontrol/indike eder. |
| [setPrintWithStatusDialog(boolean value)](#setPrintWithStatusDialog-boolean-) | PrintWithStatusDialog = true ise, mevcut yazdırma durumunu gösteren bir iletişim kutusu görüntülenir. |
| [setPrintingPage(int value)](#setPrintingPage-int-) | Hangi sayfaların yazdırılmayacağını gösterir. |
| [setQuality(int value)](#setQuality-int-) | Sayfaları `Jpeg` formatında kaydederken uygulanacak, oluşturulan görüntülerin kalitesini belirleyen bir değeri ayarlar. |
| [setRenderingHint(RenderingHints.Key key, Object value)](#setRenderingHint-java.awt.RenderingHints.Key-java.lang.Object-) | Renderleme algoritmaları için tek bir tercihin değerini ayarlar. |
| [setSVGFitToViewPort(boolean value)](#setSVGFitToViewPort-boolean-) | Bu özellik doğruysa, oluşturulan svg görünüm alanına sığar. |
| [setSaveFormat(int value)](#setSaveFormat-int-) | Çıktı dosya formatı türünü ayarlar. Destek: Tiff/XPS |
| [setSheetSet(SheetSet value)](#setSheetSet-com.aspose.cells.SheetSet-) | Render edilecek sayfaları ayarlar. |
| [setSvgCssPrefix(String value)](#setSvgCssPrefix-java.lang.String-) | Svg içinde css adının önekini ayarlar, varsayılan değer boş dizedir. |
| [setTextCrossType(int value)](#setTextCrossType-int-) | Metin genişliği hücre genişliğinden büyük olduğunda görüntüleme metin türünü ayarlar. |
| [setTiffColorDepth(int value)](#setTiffColorDepth-int-) | Sayfaları `Tiff` formatında kaydederken uygulanacak bit derinliğini ayarlar. |
| [setTiffCompression(int value)](#setTiffCompression-int-) | Sayfaları `Tiff` formatında kaydederken uygulanacak sıkıştırma türünü ayarlar. |
| [setTiffPhotometricInterpretation(int value)](#setTiffPhotometricInterpretation-int-) | Sayfaları `Tiff` formatında kaydederken uygulanacak PhotometricInterpretation türünü ayarlar. |
| [setTransparent(boolean value)](#setTransparent-boolean-) | Oluşturulan görüntünün arka planının şeffaf olup olmadığını belirtir. |
| [setVerticalResolution(int value)](#setVerticalResolution-int-) | Oluşturulan görüntüler için dikey çözünürlüğü nokta başına düşen inç cinsinden ayarlar. |
| [setWarningCallback(IWarningCallback value)](#setWarningCallback-com.aspose.cells.IWarningCallback-) | Uyarı geri çağrısını ayarlar. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### SvgImageOptions() {#SvgImageOptions--}
```
public SvgImageOptions()
```


Yapıcı.

### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| arg0 | java.lang.Object |  |

**Returns:**
boolean
### getAllColumnsInOnePagePerSheet() {#getAllColumnsInOnePagePerSheet--}
```
public boolean getAllColumnsInOnePagePerSheet()
```


AllColumnsInOnePagePerSheet true ise, bir sayfanın tüm sütun içeriği tek bir sayfaya çıktılanır. pagesetup'ın kağıt boyutu genişliği geçersiz olur, ancak pagesetup'ın diğer ayarları etkili olmaya devam eder.

**Returns:**
boolean
### getChartImageType() {#getChartImageType--}
```
public ImageFormat getChartImageType()
```


Dönüştürürken grafik görüntü tipini belirtin. varsayılan değer: PNG.

**Remarks**

NOT: Bu üye artık kullanımdan kaldırılmıştır. Bunun yerine, Chart ve Shape her zaman vektör öğeleri (ör. nokta, çizgi) olarak işlenir, böylece render kalitesi artar. Bu özellik, Haziran 2022'den itibaren 12 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

**Returns:**
[ImageFormat](../../com.aspose.cells/imageformat)
### getCheckWorkbookDefaultFont() {#getCheckWorkbookDefaultFont--}
```
public boolean getCheckWorkbookDefaultFont()
```


Excel'deki karakterler Unicode olduğunda ve hücre stilinde doğru yazı tipi ayarlanmamışsa, pdf ve görüntüde blok olarak görünebilirler. Bunu true olarak ayarlayın, böylece önce çalışma kitabının varsayılan yazı tipi kullanılarak bu karakterler gösterilmeye çalışılır.

**Remarks**

Varsayılan true'dur.

**Returns:**
boolean
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getCssPrefix() {#getCssPrefix--}
```
public String getCssPrefix()
```


Svg içinde css adının önekini alır, varsayılan değer boş dizedir.

**Returns:**
java.lang.String
### getCustomRenderSettings() {#getCustomRenderSettings--}
```
public CustomRenderSettings getCustomRenderSettings()
```


Renderleme sırasında özel ayarları alır.

**Returns:**
[CustomRenderSettings](../../com.aspose.cells/customrendersettings)
### getDefaultEditLanguage() {#getDefaultEditLanguage--}
```
public int getDefaultEditLanguage()
```


Varsayılan düzenleme dilini alır.

Bakınız [DefaultEditLanguage](../../com.aspose.cells/defaulteditlanguage).

**Remarks**

Farklı düzenleme dilleri ayarlandığında metin paragrafı için farklı düzenler görüntülenebilir/renderlanabilir. Varsayılan [DefaultEditLanguage.AUTO](../../com.aspose.cells/defaulteditlanguage\#AUTO) 'dır.

**Returns:**
int
### getDefaultFont() {#getDefaultFont--}
```
public String getDefaultFont()
```


Excel'deki karakterler Unicode olduğunda ve hücre stilinde doğru yazı tipi ayarlanmamışsa, pdf ve görüntüde blok olarak görünebilirler. Bu karakterleri göstermek için MingLiu veya MS Gothic gibi DefaultFont'u ayarlayın. Bu özellik ayarlanmamışsa, Aspose.Cells bu Unicode karakterleri göstermek için sistemin varsayılan yazı tipini kullanacaktır.

**Returns:**
java.lang.String
### getDrawObjectEventHandler() {#getDrawObjectEventHandler--}
```
public DrawObjectEventHandler getDrawObjectEventHandler()
```


Render işlemi sırasında DrawObject ve Bound elde etmek için bu arayüzü uygular.

**Returns:**
[DrawObjectEventHandler](../../com.aspose.cells/drawobjecteventhandler)
### getEmbeddedFontType() {#getEmbeddedFontType--}
```
public int getEmbeddedFontType()
```


Svg içinde gömülü olan yazı tipinin türünü alır.

Bakınız [SvgEmbeddedFontType](../../com.aspose.cells/svgembeddedfonttype).

**Remarks**

Varsayılan değer, [SvgEmbeddedFontType.NONE](../../com.aspose.cells/svgembeddedfonttype\#NONE) olup, Svg içinde font gömülmeyeceğini gösterir.

**Returns:**
int
### getEmbededImageNameInSvg() {#getEmbededImageNameInSvg--}
```
public String getEmbededImageNameInSvg()
```


Svg içinde gömülü görüntünün dosya adını belirtin. Bu, "c:\\\\xpsEmbedded" gibi bir dizin içeren tam yol olmalıdır.

**Remarks**

NOT: Bu üye artık kullanımdan kaldırılmıştır. Bunun yerine, lütfen bu özelliği kaldırın çünkü görüntüler artık Svg içinde base64 formatında her zaman gömülür. Bu özellik, Nisan 2025'ten itibaren 12 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

**Returns:**
java.lang.String
### getEmfRenderSetting() {#getEmfRenderSetting--}
```
public int getEmfRenderSetting()
```


Kaynak dosyada Emf meta dosyalarını işleme ayarı.

Bakınız [EmfRenderSetting](../../com.aspose.cells/emfrendersetting).

**Remarks**

"EMF+ Dual" olarak tanımlanan EMF metafileleri hem EMF+ kayıtları hem de EMF kayıtları içerebilir. Görüntüyü oluşturmak için her iki kayıt türü de, yalnızca EMF+ kayıtları ya da yalnızca EMF kayıtları kullanılabilir. [EmfRenderSetting.EMF\_PLUS\_PREFER](../../com.aspose.cells/emfrendersetting\#EMF-PLUS-PREFER) ayarlandığında, görüntüye render edilirken EMF+ kayıtları ayrıştırılır, aksi takdirde yalnızca EMF kayıtları ayrıştırılır. Varsayılan değer [EmfRenderSetting.EMF\_ONLY](../../com.aspose.cells/emfrendersetting\#EMF-ONLY)'dir. .NET System.Drawing.Common'a bağımlı çerçeveler için bu ayar yok sayılır.

**Returns:**
int
### getFitToViewPort() {#getFitToViewPort--}
```
public boolean getFitToViewPort()
```


Bu özellik doğruysa, oluşturulan svg görünüm alanına sığar.

**Returns:**
boolean
### getGridlineColor() {#getGridlineColor--}
```
public Color getGridlineColor()
```


Izgara çizgi rengini alır.

**Remarks**

Kaynak dosyadaki kılavuz çizgi renk ayarlarını yok sayacaktır.

**Returns:**
[Color](../../com.aspose.cells/color)
### getGridlineType() {#getGridlineType--}
```
public int getGridlineType()
```


Izgara çizgisi tipini alır.

Bakınız [GridlineType](../../com.aspose.cells/gridlinetype).

**Remarks**

Varsayılan Dotted tipidir.

**Returns:**
int
### getHorizontalResolution() {#getHorizontalResolution--}
```
public int getHorizontalResolution()
```


Oluşturulan görüntüler için yatay çözünürlüğü, inç başına nokta cinsinden alır.

**Remarks**

Varsayılan değer 96'dır. Ayarlama  ve  çıkış görüntüsünün piksel cinsinden genişlik ve yüksekliğini etkiler.

**Example**

Aşağıdaki kod çözünürlüğü 192 olarak ayarlar, oluşturulan görüntünün genişlik ve yüksekliği, çözünürlük varsayılan değer 96 iken olanın iki katıdır.

```
         Workbook wb = new Workbook("Book1.xlsx");
 
         ImageOrPrintOptions opts = new ImageOrPrintOptions();
 
         //Set output image type: png.
         opts.setImageType(ImageType.PNG);
 
         //Set resolution to 192.
         opts.setHorizontalResolution(192);
         opts.setVerticalResolution(192);
 
         //Render worksheet page to image.
         SheetRender sr = new SheetRender(wb.getWorksheets().get(0), opts);
         sr.toImage(0, "Sheet_Page1.png");
```

**Returns:**
int
### getImageType() {#getImageType--}
```
public int getImageType()
```


Oluşturulan görüntülerin formatını alır. varsayılan değer: PNG.

Bakınız [ImageType](../../com.aspose.cells/imagetype).

**Returns:**
int
### getOnePagePerSheet() {#getOnePagePerSheet--}
```
public boolean getOnePagePerSheet()
```


OnePagePerSheet true ise, bir sayfanın tüm içeriği sonuçta yalnızca bir sayfaya çıkacaktır. pagesetup'ın kağıt boyutu geçersiz olacak, ancak pagesetup'ın diğer ayarları hâlâ etkili olacaktır.

**Returns:**
boolean
### getOnlyArea() {#getOnlyArea--}
```
public boolean getOnlyArea()
```


Bu özellik doğruysa, bir Alan çıktılanır ve ölçek etkili olmaz.

**Returns:**
boolean
### getOutputBlankPageWhenNothingToPrint() {#getOutputBlankPageWhenNothingToPrint--}
```
public boolean getOutputBlankPageWhenNothingToPrint()
```


Yazdırılacak bir şey olmadığında boş sayfa çıktısı verilip verilmeyeceğini gösterir.

**Remarks**

Varsayılan false'tur.

**Returns:**
boolean
### getPageCount() {#getPageCount--}
```
public int getPageCount()
```


Kaydedilecek sayfa sayısını alır.

**Remarks**

Varsayılan System.Int32.MaxValue'dur, bu da tüm sayfaların render edileceği anlamına gelir.

**Returns:**
int
### getPageIndex() {#getPageIndex--}
```
public int getPageIndex()
```


Kaydedilecek ilk sayfanın 0 tabanlı indeksini alır.

**Remarks**

Varsayılan 0'dır.

**Returns:**
int
### getPageSavingCallback() {#getPageSavingCallback--}
```
public IPageSavingCallback getPageSavingCallback()
```


Sayfa kaydetme sürecinin ilerlemesini kontrol/indike eder.

**Returns:**
[IPageSavingCallback](../../com.aspose.cells/ipagesavingcallback)
### getPrintWithStatusDialog() {#getPrintWithStatusDialog--}
```
public boolean getPrintWithStatusDialog()
```


PrintWithStatusDialog = true ise, mevcut yazdırma durumunu gösteren bir iletişim kutusu görüntülenir; aksi takdirde böyle bir iletişim kutusu gösterilmez.

**Returns:**
boolean
### getPrintingPage() {#getPrintingPage--}
```
public int getPrintingPage()
```


Hangi sayfaların yazdırılmayacağını gösterir.

Bakınız [PrintingPageType](../../com.aspose.cells/printingpagetype).

**Returns:**
int
### getQuality() {#getQuality--}
```
public int getQuality()
```


Sayfaları `Jpeg` formatında kaydederken uygulanacak, oluşturulan görüntülerin kalitesini belirleyen bir değer alır. Varsayılan değer 100'tür.

**Remarks**

Yalnızca JPEG olarak kaydederken etkili olur. Değer 0 ile 100 arasında olmalıdır. Varsayılan değer 100'dür.

**Returns:**
int
### getSVGFitToViewPort() {#getSVGFitToViewPort--}
```
public boolean getSVGFitToViewPort()
```


Bu özellik doğruysa, oluşturulan svg görünüm alanına sığar.

**Remarks**

NOT: Bu üye artık kullanımdan kaldırılmıştır. Bunun yerine lütfen [SvgImageOptions.getFitToViewPort()](../../com.aspose.cells/svgimageoptions\#getFitToViewPort--) kullanın. Bu özellik, Nisan 2025'ten itibaren 12 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

**Returns:**
boolean
### getSaveFormat() {#getSaveFormat--}
```
public int getSaveFormat()
```


Çıktı dosya biçimi türünü alır, Tiff/XPS desteklenir.

Bakınız [SaveFormat](../../com.aspose.cells/saveformat).

**Remarks**

NOT: Bu üye artık kullanımdan kaldırılmıştır. Bunun yerine, Tiff/Svg için [getImageType()](../../com.aspose.cells/imageorprintoptions\#getImageType--) kullanın; Xps için ise [Workbook.save(String,SaveOptions)](../../com.aspose.cells/workbook\#save-String-SaveOptions-) ile [XpsSaveOptions](../../com.aspose.cells/xpssaveoptions) kullanın. Bu özellik, Ağustos 2022'den itibaren 12 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

**Returns:**
int
### getSheetSet() {#getSheetSet--}
```
public SheetSet getSheetSet()
```


Render edilecek sayfaları alır. Varsayılan, çalışma kitabındaki tüm görünür sayfalardır: [SheetSet.getVisible()](../../com.aspose.cells/sheetset\#getVisible--).

**Remarks**

Bu ayar, [SheetRender](../../com.aspose.cells/sheetrender) içinde kullanıldığında yok sayılır.

**Returns:**
[SheetSet](../../com.aspose.cells/sheetset)
### getSvgCssPrefix() {#getSvgCssPrefix--}
```
public String getSvgCssPrefix()
```


Svg içinde css adının önekini alır, varsayılan değer boş dizedir.

**Remarks**

NOT: Bu üye artık kullanımdan kaldırılmıştır. Bunun yerine lütfen [SvgImageOptions.getCssPrefix()](../../com.aspose.cells/svgimageoptions\#getCssPrefix--) kullanın. Bu özellik, Nisan 2025'ten itibaren 12 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

**Returns:**
java.lang.String
### getTextCrossType() {#getTextCrossType--}
```
public int getTextCrossType()
```


Metin genişliği hücre genişliğinden büyük olduğunda görüntüleme metin türünü alır.

Bakınız [TextCrossType](../../com.aspose.cells/textcrosstype).

**Returns:**
int
### getTiffColorDepth() {#getTiffColorDepth--}
```
public int getTiffColorDepth()
```


`Tiff` biçiminde sayfaları kaydederken yalnızca uygulanacak bit derinliğini alır.

[ColorDepth](../../com.aspose.cells/colordepth) sayfasına bakın.

**Remarks**

Yalnızca TIFF olarak kaydederken etkili olur. TiffCompression CCITT3 veya CCITT4 olarak ayarlanmışsa bu etkili olmaz, oluşturulan tiff görüntüsünün bit derinliği her zaman 1 olur.

**Returns:**
int
### getTiffCompression() {#getTiffCompression--}
```
public int getTiffCompression()
```


`Tiff` biçiminde sayfaları kaydederken yalnızca uygulanacak sıkıştırma türünü alır.

[TiffCompression](../../com.aspose.cells/tiffcompression) sayfasına bakın.

**Remarks**

Yalnızca TIFF olarak kaydederken etkili olur. Varsayılan değer Lzw'dir.

**Returns:**
int
### getTiffPhotometricInterpretation() {#getTiffPhotometricInterpretation--}
```
public int getTiffPhotometricInterpretation()
```


`Tiff` biçiminde sayfaları kaydederken yalnızca uygulanacak FotometrikYorumlama türünü alır.

**Remarks**

Yalnızca TIFF olarak kaydederken etkili olur. Varsayılan değer -1'dir, bu PhotometricInterpretation uygulanmadığını gösterir.

**Returns:**
int
### getTransparent() {#getTransparent--}
```
public boolean getTransparent()
```


Oluşturulan görüntünün arka planının şeffaf olup olmadığını belirtir.

**Remarks**

Varsayılan değer false'tur. Bu, oluşturulan görüntülerin arka planının beyaz olduğu anlamına gelir.

**Returns:**
boolean
### getVerticalResolution() {#getVerticalResolution--}
```
public int getVerticalResolution()
```


Oluşturulan görüntüler için dikey çözünürlüğü, inç başına nokta cinsinden alır.

**Remarks**

Varsayılan değer 96'dır. Ayarlama  ve  çıkış görüntüsünün piksel cinsinden genişlik ve yüksekliğini etkiler.

**Example**

Aşağıdaki kod çözünürlüğü 192 olarak ayarlar, oluşturulan görüntünün genişlik ve yüksekliği, çözünürlük varsayılan değer 96 iken olanın iki katıdır.

```
         Workbook wb = new Workbook("Book1.xlsx");
 
         ImageOrPrintOptions opts = new ImageOrPrintOptions();
 
         //Set output image type: png.
         opts.setImageType(ImageType.PNG);
 
         //Set resolution to 192.
         opts.setHorizontalResolution(192);
         opts.setVerticalResolution(192);
 
         //Render Chart to image.
         wb.getWorksheets().get(0).getCharts().get(0).toImage("Chart.png", opts);
```

**Returns:**
int
### getWarningCallback() {#getWarningCallback--}
```
public IWarningCallback getWarningCallback()
```


Uyarı geri çağrısını alır.

**Returns:**
[IWarningCallback](../../com.aspose.cells/iwarningcallback)
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isCellAutoFit() {#isCellAutoFit--}
```
public boolean isCellAutoFit()
```


Hücrelerin genişlik ve yüksekliğinin hücre değeriyle otomatik olarak ayarlanıp ayarlanmadığını gösterir. Varsayılan değer false'tur.

**Remarks**

NOT: Bu üye artık kullanımdan kaldırılmıştır. Bunun yerine bu özellik kullanılmaz, lütfen bu özelliği kaldırın. Bu özellik, Ağustos 2022'den itibaren 12 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

**Returns:**
boolean
### isFontSubstitutionCharGranularity() {#isFontSubstitutionCharGranularity--}
```
public boolean isFontSubstitutionCharGranularity()
```


Hücre yazı tipi uyumlu olmadığında yalnızca karakterin yazı tipinin değiştirilip değiştirilmeyeceğini gösterir.

**Remarks**

Varsayılan false'tur. Önce hücre yazı tipi için Workbook ve PdfSaveOption/sistem'in varsayılan yazı tipini deneyeceğiz.

**Returns:**
boolean
### isOptimized() {#isOptimized--}
```
public boolean isOptimized()
```


Çıktı öğelerinin optimize edilip edilmeyeceğini belirtir.

**Remarks**

Varsayılan değer false'tur. Şu anda bu özellik true olarak ayarlandığında aşağıdaki iyileştirmeler yapılır: 1. kenar çizgileri optimize edilir. 2. Svg görüntüsü oluşturulurken dosya boyutu optimize edilir.

**Returns:**
boolean
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### setAllColumnsInOnePagePerSheet(boolean value) {#setAllColumnsInOnePagePerSheet-boolean-}
```
public void setAllColumnsInOnePagePerSheet(boolean value)
```


AllColumnsInOnePagePerSheet true ise, bir sayfanın tüm sütun içeriği tek bir sayfaya çıktılanır. pagesetup'ın kağıt boyutu genişliği geçersiz olur, ancak pagesetup'ın diğer ayarları etkili olmaya devam eder.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setCellAutoFit(boolean value) {#setCellAutoFit-boolean-}
```
public void setCellAutoFit(boolean value)
```


Hücrelerin genişlik ve yüksekliğinin hücre değeriyle otomatik olarak ayarlanıp ayarlanmadığını gösterir. Varsayılan değer false'tur.

**Remarks**

NOT: Bu üye artık kullanımdan kaldırılmıştır. Bunun yerine bu özellik kullanılmaz, lütfen bu özelliği kaldırın. Bu özellik, Ağustos 2022'den itibaren 12 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setChartImageType(ImageFormat value) {#setChartImageType-com.aspose.cells.ImageFormat-}
```
public void setChartImageType(ImageFormat value)
```


Dönüştürürken grafik görüntü tipini belirtin. varsayılan değer: PNG.

**Remarks**

NOT: Bu üye artık kullanımdan kaldırılmıştır. Bunun yerine, Chart ve Shape her zaman vektör öğeleri (ör. nokta, çizgi) olarak işlenir, böylece render kalitesi artar. Bu özellik, Haziran 2022'den itibaren 12 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | [ImageFormat](../../com.aspose.cells/imageformat) |  |

### setCheckWorkbookDefaultFont(boolean value) {#setCheckWorkbookDefaultFont-boolean-}
```
public void setCheckWorkbookDefaultFont(boolean value)
```


Excel'deki karakterler Unicode olduğunda ve hücre stilinde doğru yazı tipi ayarlanmamışsa, pdf ve görüntüde blok olarak görünebilirler. Bunu true olarak ayarlayın, böylece önce çalışma kitabının varsayılan yazı tipi kullanılarak bu karakterler gösterilmeye çalışılır.

**Remarks**

Varsayılan true'dur.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setCssPrefix(String value) {#setCssPrefix-java.lang.String-}
```
public void setCssPrefix(String value)
```


Svg içinde css adının önekini ayarlar, varsayılan değer boş dizedir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String |  |

### setCustomRenderSettings(CustomRenderSettings value) {#setCustomRenderSettings-com.aspose.cells.CustomRenderSettings-}
```
public void setCustomRenderSettings(CustomRenderSettings value)
```


Renderleme sırasında özel ayarları belirler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | [CustomRenderSettings](../../com.aspose.cells/customrendersettings) |  |

### setDefaultEditLanguage(int value) {#setDefaultEditLanguage-int-}
```
public void setDefaultEditLanguage(int value)
```


Varsayılan düzenleme dilini ayarlar.

Bakınız [DefaultEditLanguage](../../com.aspose.cells/defaulteditlanguage).

**Remarks**

Farklı düzenleme dilleri ayarlandığında metin paragrafı için farklı düzenler görüntülenebilir/renderlanabilir. Varsayılan [DefaultEditLanguage.AUTO](../../com.aspose.cells/defaulteditlanguage\#AUTO) 'dır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setDefaultFont(String value) {#setDefaultFont-java.lang.String-}
```
public void setDefaultFont(String value)
```


Excel'deki karakterler Unicode olduğunda ve hücre stilinde doğru yazı tipi ayarlanmamışsa, pdf ve görüntüde blok olarak görünebilirler. Bu karakterleri göstermek için MingLiu veya MS Gothic gibi DefaultFont'u ayarlayın. Bu özellik ayarlanmamışsa, Aspose.Cells bu Unicode karakterleri göstermek için sistemin varsayılan yazı tipini kullanacaktır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String |  |

### setDesiredSize(int desiredWidth, int desiredHeight) {#setDesiredSize-int-int-}
```
public void setDesiredSize(int desiredWidth, int desiredHeight)
```


Görüntünün istenen genişlik ve yüksekliğini ayarlar.

**Remarks**

NOT: Bu üye artık kullanımdan kaldırılmıştır. Bunun yerine, keepAspectRatio parametresini false olarak ayarlayarak [setDesiredSize(int,int,boolean)](../../com.aspose.cells/imageorprintoptions\#setDesiredSize-int-int-boolean-) kullanın. Bu özellik, Mayıs 2023'ten itibaren 12 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| desiredWidth | int | piksellerde istenen genişlik |
| desiredHeight | int | piksellerde istenen yükseklik |

### setDesiredSize(int desiredWidth, int desiredHeight, boolean keepAspectRatio) {#setDesiredSize-int-int-boolean-}
```
public void setDesiredSize(int desiredWidth, int desiredHeight, boolean keepAspectRatio)
```


Görüntünün istenen genişlik ve yüksekliğini ayarlar.

**Remarks**

Çıktı görüntüsünün piksel cinsinden genişlik ve yüksekliği yalnızca ayarlanan istenen genişlik ve yüksekliğe dayanacaktır. Bu durumda  ve  çıkış görüntüsünün genişlik ve yüksekliğini etkilemeyecektir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| desiredWidth | int | piksellerde istenen genişlik |
| desiredHeight | int | piksellerde istenen yükseklik |
| keepAspectRatio | boolean | orijinal görüntünün en-boy oranını koruyup korumayacağını belirler |

### setDrawObjectEventHandler(DrawObjectEventHandler value) {#setDrawObjectEventHandler-com.aspose.cells.DrawObjectEventHandler-}
```
public void setDrawObjectEventHandler(DrawObjectEventHandler value)
```


Render işlemi sırasında DrawObject ve Bound elde etmek için bu arayüzü uygular.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | [DrawObjectEventHandler](../../com.aspose.cells/drawobjecteventhandler) |  |

### setEmbeddedFontType(int value) {#setEmbeddedFontType-int-}
```
public void setEmbeddedFontType(int value)
```


Svg içinde gömülü olan yazı tipinin türünü ayarlar.

Bakınız [SvgEmbeddedFontType](../../com.aspose.cells/svgembeddedfonttype).

**Remarks**

Varsayılan değer, [SvgEmbeddedFontType.NONE](../../com.aspose.cells/svgembeddedfonttype\#NONE) olup, Svg içinde font gömülmeyeceğini gösterir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setEmbededImageNameInSvg(String value) {#setEmbededImageNameInSvg-java.lang.String-}
```
public void setEmbededImageNameInSvg(String value)
```


Svg içinde gömülü görüntünün dosya adını belirtin. Bu, "c:\\\\xpsEmbedded" gibi bir dizin içeren tam yol olmalıdır.

**Remarks**

NOT: Bu üye artık kullanımdan kaldırılmıştır. Bunun yerine, lütfen bu özelliği kaldırın çünkü görüntüler artık Svg içinde base64 formatında her zaman gömülür. Bu özellik, Nisan 2025'ten itibaren 12 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String |  |

### setEmfRenderSetting(int value) {#setEmfRenderSetting-int-}
```
public void setEmfRenderSetting(int value)
```


Kaynak dosyada Emf meta dosyalarını işleme ayarı.

Bakınız [EmfRenderSetting](../../com.aspose.cells/emfrendersetting).

**Remarks**

"EMF+ Dual" olarak tanımlanan EMF metafileleri hem EMF+ kayıtları hem de EMF kayıtları içerebilir. Görüntüyü oluşturmak için her iki kayıt türü de, yalnızca EMF+ kayıtları ya da yalnızca EMF kayıtları kullanılabilir. [EmfRenderSetting.EMF\_PLUS\_PREFER](../../com.aspose.cells/emfrendersetting\#EMF-PLUS-PREFER) ayarlandığında, görüntüye render edilirken EMF+ kayıtları ayrıştırılır, aksi takdirde yalnızca EMF kayıtları ayrıştırılır. Varsayılan değer [EmfRenderSetting.EMF\_ONLY](../../com.aspose.cells/emfrendersetting\#EMF-ONLY)'dir. .NET System.Drawing.Common'a bağımlı çerçeveler için bu ayar yok sayılır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setFitToViewPort(boolean value) {#setFitToViewPort-boolean-}
```
public void setFitToViewPort(boolean value)
```


Bu özellik doğruysa, oluşturulan svg görünüm alanına sığar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setFontSubstitutionCharGranularity(boolean value) {#setFontSubstitutionCharGranularity-boolean-}
```
public void setFontSubstitutionCharGranularity(boolean value)
```


Hücre yazı tipi uyumlu olmadığında yalnızca karakterin yazı tipinin değiştirilip değiştirilmeyeceğini gösterir.

**Remarks**

Varsayılan false'tur. Önce hücre yazı tipi için Workbook ve PdfSaveOption/sistem'in varsayılan yazı tipini deneyeceğiz.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setGridlineColor(Color value) {#setGridlineColor-com.aspose.cells.Color-}
```
public void setGridlineColor(Color value)
```


Izgara çizgi rengini ayarlar.

**Remarks**

Kaynak dosyadaki kılavuz çizgi renk ayarlarını yok sayacaktır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | [Color](../../com.aspose.cells/color) |  |

### setGridlineType(int value) {#setGridlineType-int-}
```
public void setGridlineType(int value)
```


Kılavuz çizgi tipini ayarlar.

Bakınız [GridlineType](../../com.aspose.cells/gridlinetype).

**Remarks**

Varsayılan Dotted tipidir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setHorizontalResolution(int value) {#setHorizontalResolution-int-}
```
public void setHorizontalResolution(int value)
```


Oluşturulan görüntüler için yatay çözünürlüğü nokta başına düşen inç cinsinden ayarlar.

**Remarks**

Varsayılan değer 96'dır. Ayarlama  ve  çıkış görüntüsünün piksel cinsinden genişlik ve yüksekliğini etkiler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setImageType(int value) {#setImageType-int-}
```
public void setImageType(int value)
```


Oluşturulan görüntülerin formatını ayarlar. Varsayılan değer: PNG.

Bakınız [ImageType](../../com.aspose.cells/imagetype).

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setOnePagePerSheet(boolean value) {#setOnePagePerSheet-boolean-}
```
public void setOnePagePerSheet(boolean value)
```


OnePagePerSheet true ise, bir sayfanın tüm içeriği sonuçta yalnızca bir sayfaya çıkacaktır. pagesetup'ın kağıt boyutu geçersiz olacak, ancak pagesetup'ın diğer ayarları hâlâ etkili olacaktır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setOnlyArea(boolean value) {#setOnlyArea-boolean-}
```
public void setOnlyArea(boolean value)
```


Bu özellik doğruysa, bir Alan çıktılanır ve ölçek etkili olmaz.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setOptimized(boolean value) {#setOptimized-boolean-}
```
public void setOptimized(boolean value)
```


Çıktı öğelerinin optimize edilip edilmeyeceğini belirtir.

**Remarks**

Varsayılan değer false'tur. Şu anda bu özellik true olarak ayarlandığında aşağıdaki iyileştirmeler yapılır: 1. kenar çizgileri optimize edilir. 2. Svg görüntüsü oluşturulurken dosya boyutu optimize edilir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setOutputBlankPageWhenNothingToPrint(boolean value) {#setOutputBlankPageWhenNothingToPrint-boolean-}
```
public void setOutputBlankPageWhenNothingToPrint(boolean value)
```


Yazdırılacak bir şey olmadığında boş sayfa çıktısı verilip verilmeyeceğini gösterir.

**Remarks**

Varsayılan false'tur.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setPageCount(int value) {#setPageCount-int-}
```
public void setPageCount(int value)
```


Kaydedilecek sayfa sayısını ayarlar.

**Remarks**

Varsayılan System.Int32.MaxValue'dur, bu da tüm sayfaların render edileceği anlamına gelir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setPageIndex(int value) {#setPageIndex-int-}
```
public void setPageIndex(int value)
```


Kaydedilecek ilk sayfanın 0 tabanlı indeksini ayarlar.

**Remarks**

Varsayılan 0'dır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setPageSavingCallback(IPageSavingCallback value) {#setPageSavingCallback-com.aspose.cells.IPageSavingCallback-}
```
public void setPageSavingCallback(IPageSavingCallback value)
```


Sayfa kaydetme sürecinin ilerlemesini kontrol/indike eder.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | [IPageSavingCallback](../../com.aspose.cells/ipagesavingcallback) |  |

### setPrintWithStatusDialog(boolean value) {#setPrintWithStatusDialog-boolean-}
```
public void setPrintWithStatusDialog(boolean value)
```


PrintWithStatusDialog = true ise, mevcut yazdırma durumunu gösteren bir iletişim kutusu görüntülenir; aksi takdirde böyle bir iletişim kutusu gösterilmez.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setPrintingPage(int value) {#setPrintingPage-int-}
```
public void setPrintingPage(int value)
```


Hangi sayfaların yazdırılmayacağını gösterir.

Bakınız [PrintingPageType](../../com.aspose.cells/printingpagetype).

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setQuality(int value) {#setQuality-int-}
```
public void setQuality(int value)
```


Sayfaları `Jpeg` formatında kaydederken uygulanacak, oluşturulan görüntülerin kalitesini belirleyen bir değeri ayarlar. Varsayılan değer 100'tür.

**Remarks**

Yalnızca JPEG olarak kaydederken etkili olur. Değer 0 ile 100 arasında olmalıdır. Varsayılan değer 100'dür.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setRenderingHint(RenderingHints.Key key, Object value) {#setRenderingHint-java.awt.RenderingHints.Key-java.lang.Object-}
```
public void setRenderingHint(RenderingHints.Key key, Object value)
```


Renderleme algoritmaları için tek bir tercihin değerini ayarlar. İpucu kategorileri, renderleme kalitesi ve renderleme sürecindeki genel zaman/kalite dengesini kontrol eder. Bazı ortak anahtarlar ve değerlerin tanımları için RenderingHints sınıfına bakın.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| anahtar | java.awt.RenderingHints.Key | ayarlanacak ipucunun anahtarı. |
| değer | java.lang.Object | belirtilen ipucu kategorisi için tercihleri gösteren değer. |

### setSVGFitToViewPort(boolean value) {#setSVGFitToViewPort-boolean-}
```
public void setSVGFitToViewPort(boolean value)
```


Bu özellik doğruysa, oluşturulan svg görünüm alanına sığar.

**Remarks**

NOT: Bu üye artık kullanımdan kaldırılmıştır. Bunun yerine lütfen [SvgImageOptions.getFitToViewPort()](../../com.aspose.cells/svgimageoptions\#getFitToViewPort--) kullanın. Bu özellik, Nisan 2025'ten itibaren 12 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setSaveFormat(int value) {#setSaveFormat-int-}
```
public void setSaveFormat(int value)
```


Çıktı dosya formatı türünü ayarlar. Destek: Tiff/XPS

Bakınız [SaveFormat](../../com.aspose.cells/saveformat).

**Remarks**

NOT: Bu üye artık kullanımdan kaldırılmıştır. Bunun yerine, Tiff/Svg için [getImageType()](../../com.aspose.cells/imageorprintoptions\#getImageType--) kullanın; Xps için ise [Workbook.save(String,SaveOptions)](../../com.aspose.cells/workbook\#save-String-SaveOptions-) ile [XpsSaveOptions](../../com.aspose.cells/xpssaveoptions) kullanın. Bu özellik, Ağustos 2022'den itibaren 12 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setSheetSet(SheetSet value) {#setSheetSet-com.aspose.cells.SheetSet-}
```
public void setSheetSet(SheetSet value)
```


Render edilecek sayfaları ayarlar. Varsayılan, çalışma kitabındaki tüm görünür sayfalardır: [SheetSet.getVisible()](../../com.aspose.cells/sheetset\#getVisible--).

**Remarks**

Bu ayar, [SheetRender](../../com.aspose.cells/sheetrender) içinde kullanıldığında yok sayılır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | [SheetSet](../../com.aspose.cells/sheetset) |  |

### setSvgCssPrefix(String value) {#setSvgCssPrefix-java.lang.String-}
```
public void setSvgCssPrefix(String value)
```


Svg içinde css adının önekini ayarlar, varsayılan değer boş dizedir.

**Remarks**

NOT: Bu üye artık kullanımdan kaldırılmıştır. Bunun yerine lütfen [SvgImageOptions.getCssPrefix()](../../com.aspose.cells/svgimageoptions\#getCssPrefix--) kullanın. Bu özellik, Nisan 2025'ten itibaren 12 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String |  |

### setTextCrossType(int value) {#setTextCrossType-int-}
```
public void setTextCrossType(int value)
```


Metin genişliği hücre genişliğinden büyük olduğunda görüntüleme metin türünü ayarlar.

Bakınız [TextCrossType](../../com.aspose.cells/textcrosstype).

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setTiffColorDepth(int value) {#setTiffColorDepth-int-}
```
public void setTiffColorDepth(int value)
```


Sayfaları `Tiff` formatında kaydederken uygulanacak bit derinliğini ayarlar.

[ColorDepth](../../com.aspose.cells/colordepth) sayfasına bakın.

**Remarks**

Yalnızca TIFF olarak kaydederken etkili olur. TiffCompression CCITT3 veya CCITT4 olarak ayarlanmışsa bu etkili olmaz, oluşturulan tiff görüntüsünün bit derinliği her zaman 1 olur.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setTiffCompression(int value) {#setTiffCompression-int-}
```
public void setTiffCompression(int value)
```


Sayfaları `Tiff` formatında kaydederken uygulanacak sıkıştırma türünü ayarlar.

[TiffCompression](../../com.aspose.cells/tiffcompression) sayfasına bakın.

**Remarks**

Yalnızca TIFF olarak kaydederken etkili olur. Varsayılan değer Lzw'dir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setTiffPhotometricInterpretation(int value) {#setTiffPhotometricInterpretation-int-}
```
public void setTiffPhotometricInterpretation(int value)
```


Sayfaları `Tiff` formatında kaydederken uygulanacak PhotometricInterpretation türünü ayarlar.

**Remarks**

Yalnızca TIFF olarak kaydederken etkili olur. Varsayılan değer -1'dir, bu PhotometricInterpretation uygulanmadığını gösterir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setTransparent(boolean value) {#setTransparent-boolean-}
```
public void setTransparent(boolean value)
```


Oluşturulan görüntünün arka planının şeffaf olup olmadığını belirtir.

**Remarks**

Varsayılan değer false'tur. Bu, oluşturulan görüntülerin arka planının beyaz olduğu anlamına gelir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setVerticalResolution(int value) {#setVerticalResolution-int-}
```
public void setVerticalResolution(int value)
```


Oluşturulan görüntüler için dikey çözünürlüğü nokta başına düşen inç cinsinden ayarlar.

**Remarks**

Varsayılan değer 96'dır. Ayarlama  ve  çıkış görüntüsünün piksel cinsinden genişlik ve yüksekliğini etkiler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setWarningCallback(IWarningCallback value) {#setWarningCallback-com.aspose.cells.IWarningCallback-}
```
public void setWarningCallback(IWarningCallback value)
```


Uyarı geri çağrısını ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | [IWarningCallback](../../com.aspose.cells/iwarningcallback) |  |

### toString() {#toString--}
```
public String toString()
```




**Returns:**
java.lang.String
### wait() {#wait--}
```
public final void wait()
```




### wait(long arg0) {#wait-long-}
```
public final native void wait(long arg0)
```




**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

