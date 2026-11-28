---
title: "Sınıf GridWorkbookSettings"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.GridJs.GridWorkbookSettings sınıfı. Çalışma kitabının ayarlarını temsil eder"
type: docs
url: /tr/net/aspose.cells.gridjs/gridworkbooksettings/
---
## GridWorkbookSettings class

Çalışma kitabının ayarlarını temsil eder.

```csharp
public class GridWorkbookSettings
```

## Yapıcılar

| Ad | Açıklama |
| --- | --- |
| [GridWorkbookSettings](gridworkbooksettings/)() | Varsayılan yapıcı. |

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [Author](../../aspose.cells.gridjs/gridworkbooksettings/author/) { get; set; } | Dosyanın yazarını alır/ayarlar. |
| [CheckCustomNumberFormat](../../aspose.cells.gridjs/gridworkbooksettings/checkcustomnumberformat/) { get; set; } | Style.Custom ayarlanırken özel sayı biçiminin kontrol edilip edilmeyeceğini gösterir, varsayılan değer false'tur. |
| [CheckExcelRestriction](../../aspose.cells.gridjs/gridworkbooksettings/checkexcelrestriction/) { get; set; } | Kullanıcı hücreyle ilgili nesneleri değiştirdiğinde Excel dosyasının kısıtlamalarının kontrol edilip edilmeyeceği. Örneğin, Excel 32K'dan uzun bir dize değerinin girilmesine izin vermez. Cell.PutValue(string) gibi 32K'dan uzun bir değer girerseniz ve bu özellik true ise bir İstisna alırsınız. Özellik false ise, girdiğiniz dize değerini hücrenin değeri olarak kabul ederiz, böylece daha sonra CSV gibi diğer dosya formatları için tam dize değerini dışa aktarabilirsiniz. Ancak, Excel dosya formatı için geçersiz bir değer ayarladıysanız, çalışma kitabını daha sonra Excel dosya formatında kaydetmemelisiniz. Aksi takdirde oluşturulan Excel dosyasında beklenmeyen hatalar ortaya çıkabilir. Varsayılan değer false'tur. |
| [CreateCalcChain](../../aspose.cells.gridjs/gridworkbooksettings/createcalcchain/) { get; set; } | Hesaplanmış formül zincirinin oluşturulup oluşturulmayacağını gösterir. Varsayılan değer false'tur. |
| [Date1904](../../aspose.cells.gridjs/gridworkbooksettings/date1904/) { get; set; } | Çalışma kitabının 1904 tarih sistemini kullanıp kullanmadığını temsil eden bir değeri alır veya ayarlar. |
| [EnableMacros](../../aspose.cells.gridjs/gridworkbooksettings/enablemacros/) { get; set; } | Makroları etkinleştir; Şu anda yalnızca bir çalışma kitabında bir çalışma sayfasını başka bir çalışma sayfasına kopyalarken çalışır. |
| [ForceFullCalculate](../../aspose.cells.gridjs/gridworkbooksettings/forcefullcalculate/) { get; set; } | Bir hesaplama tetiklendiğinde her seferinde tam olarak hesaplanıp hesaplanmayacağını gösterir. |
| [Iteration](../../aspose.cells.gridjs/gridworkbooksettings/iteration/) { get; set; } | Döngüsel referansları çözmek için yineleme kullanılıp kullanılmayacağını gösterir. |
| [MaxIteration](../../aspose.cells.gridjs/gridworkbooksettings/maxiteration/) { get; set; } | Döngüsel bir referansı çözmek için azami yineleme sayısını alır veya ayarlar, varsayılan değer 100'dür. |
| [PrecisionAsDisplayed](../../aspose.cells.gridjs/gridworkbooksettings/precisionasdisplayed/) { get; set; } | Bu çalışma kitabındaki hesaplamalar, sayıların görüntülendiği hassasiyetle yalnızca yapılacaksa doğru. |
| [ReCalculateOnOpen](../../aspose.cells.gridjs/gridworkbooksettings/recalculateonopen/) { get; set; } | Dosya açıldığında tüm formüllerin yeniden hesaplanıp hesaplanmayacağını gösterir. Varsayılan değer true'tur. |

### Örnekler

```csharp
[C#]

GridJsWorkbook g = new GridJsWorkbook();

GridWorkbookSettings gsettings = new GridWorkbookSettings();
g.Settings=gsettings;

//işinizi yapın

[Visual Basic]
Dim g as GridJsWorkbook = new GridJsWorkbook()

Dim gsettings as GridWorkbookSettings = new GridWorkbookSettings()
 g.Settings=gsettings;
 
'do your business
```

### Ayrıca Bakınız

* namespace [Aspose.Cells.GridJs](../../aspose.cells.gridjs/)
* assembly [Aspose.Cells.GridJs](../../)


