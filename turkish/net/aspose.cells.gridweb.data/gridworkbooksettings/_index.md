---
title: "Sınıf GridWorkbookSettings"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.GridWeb.Data.GridWorkbookSettings sınıfı. Çalışma kitabının ayarlarını temsil eder"
type: docs
url: /tr/net/aspose.cells.gridweb.data/gridworkbooksettings/
---
## GridWorkbookSettings class

Çalışma kitabının ayarlarını temsil eder.

```csharp
public class GridWorkbookSettings : ISerializable
```

## Yapıcılar

| Ad | Açıklama |
| --- | --- |
| [GridWorkbookSettings](gridworkbooksettings/)() | varsayılan yapıcı |

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [Author](../../aspose.cells.gridweb.data/gridworkbooksettings/author/) { get; set; } | Dosyanın yazarını alır ve ayarlar. |
| [CheckCustomNumberFormat](../../aspose.cells.gridweb.data/gridworkbooksettings/checkcustomnumberformat/) { get; set; } | Style.Custom ayarlanırken özel sayı biçiminin kontrol edilip edilmediğini alır veya ayarlar. |
| [CreateCalcChain](../../aspose.cells.gridweb.data/gridworkbooksettings/createcalcchain/) { get; set; } | Hesaplanmış formül zincirinin oluşturulup oluşturulmayacağını alır veya ayarlar. Varsayılan değer false'tur. |
| [Date1904](../../aspose.cells.gridweb.data/gridworkbooksettings/date1904/) { get; set; } | Çalışma kitabının 1904 tarih sistemini kullanıp kullanmadığını temsil eden değeri alır veya ayarlar. |
| [EnableMacros](../../aspose.cells.gridweb.data/gridworkbooksettings/enablemacros/) { get; set; } | Makroların etkinleştirilip etkinleştirilmeyeceğini alır veya ayarlar; artık yalnızca bir çalışma kitabındaki bir çalışma sayfasını başka bir çalışma sayfasına kopyalarken çalışır. |
| [ForceFullCalculate](../../aspose.cells.gridweb.data/gridworkbooksettings/forcefullcalculate/) { get; set; } | Bir hesaplama tetiklendiğinde her seferinde tam olarak hesaplayıp hesaplamayacağını alır veya ayarlar. |
| [Iteration](../../aspose.cells.gridweb.data/gridworkbooksettings/iteration/) { get; set; } | Döngüsel referansları çözmek için yineleme kullanılıp kullanılmayacağını alır veya ayarlar. |
| [MaxIteration](../../aspose.cells.gridweb.data/gridworkbooksettings/maxiteration/) { get; set; } | Döngüsel bir referansı çözmek için azami yineleme sayısını alır veya ayarlar, varsayılan değer 100'dür. |
| [PrecisionAsDisplayed](../../aspose.cells.gridweb.data/gridworkbooksettings/precisionasdisplayed/) { get; set; } | Bu çalışma kitabındaki hesaplamalar, sayıların görüntülendiği hassasiyetle yalnızca yapılacaksa doğru. |
| [PreservePaddingSpaces](../../aspose.cells.gridweb.data/gridworkbooksettings/preservepaddingspaces/) { get; set; } | Formülleri alırken ve ayarlarken formül tokenları arasında eklenen boşluk ve satır sonlarının korunup korunmayacağını gösterir. Varsayılan değer yanlıştır. |
| [ReCalculateOnOpen](../../aspose.cells.gridweb.data/gridworkbooksettings/recalculateonopen/) { get; set; } | Dosya açıldığında tüm formüllerin yeniden hesaplanıp hesaplanmayacağını alır veya ayarlar. |

### Örnekler

```csharp
[C#]

 
GridWeb gridweb = new GridWeb();
GridWorkbookSettings gsettings = new GridWorkbookSettings();
gridweb.Settings=gsettings;

//işinizi yapın

[Visual Basic]


Dim gsettings as GridWorkbookSettings = new GridWorkbookSettings()
 gridweb.Settings=gsettings;
 
'do your business
```

### Ayrıca Bakınız

* namespace [Aspose.Cells.GridWeb.Data](../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../)


