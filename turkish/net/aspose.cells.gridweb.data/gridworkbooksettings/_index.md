---
title: GridWorkbookSettings
second_title: Aspose.Cells for .NET API Referansı
description: Çalışma kitabının ayarlarını temsil eder.
type: docs
weight: 560
url: /tr/net/aspose.cells.gridweb.data/gridworkbooksettings/
---
## GridWorkbookSettings class

Çalışma kitabının ayarlarını temsil eder.

```csharp
public class GridWorkbookSettings
```

## yapıcılar

| İsim | Tanım |
| --- | --- |
| [GridWorkbookSettings](gridworkbooksettings)() | Default_Constructor |

## Özellikleri

| İsim | Tanım |
| --- | --- |
| [Author](../../aspose.cells.gridweb.data/gridworkbooksettings/author) { get; set; } | Dosyanın yazarını alır ve ayarlar. |
| [CheckCustomNumberFormat](../../aspose.cells.gridweb.data/gridworkbooksettings/checkcustomnumberformat) { get; set; } | Style.Custom. ayarlanırken özel sayı biçiminin kontrol edilip edilmeyeceğini alır veya ayarlar |
| [CreateCalcChain](../../aspose.cells.gridweb.data/gridworkbooksettings/createcalcchain) { get; set; } | Hesaplanmış formüller zinciri oluşturup oluşturmayacağını alır veya ayarlar. Varsayılan yanlıştır. |
| [Date1904](../../aspose.cells.gridweb.data/gridworkbooksettings/date1904) { get; set; } | Çalışma kitabının 1904 tarih sistemini kullanıp kullanmadığını gösteren değeri alır veya ayarlar. |
| [EnableMacros](../../aspose.cells.gridweb.data/gridworkbooksettings/enablemacros) { get; set; } | Makroların etkinleştirilip etkinleştirilmeyeceğini alır veya ayarlar; Artık yalnızca çalışma kitabındaki bir çalışma sayfasını başka bir çalışma sayfasına kopyalarken çalışıyor. |
| [ForceFullCalculate](../../aspose.cells.gridweb.data/gridworkbooksettings/forcefullcalculate) { get; set; } | Bir hesaplama her tetiklendiğinde tam olarak hesaplanıp hesaplanmayacağını alır veya ayarlar. |
| [Iteration](../../aspose.cells.gridweb.data/gridworkbooksettings/iteration) { get; set; } | Döngüsel başvuruları çözümlemek için yineleme kullanılıp kullanılmayacağını alır veya ayarlar. |
| [MaxIteration](../../aspose.cells.gridweb.data/gridworkbooksettings/maxiteration) { get; set; } | Döngüsel bir başvuruyu çözmek için maksimum yineleme sayısını alır veya ayarlar, varsayılan değer 100'dür. |
| [PrecisionAsDisplayed](../../aspose.cells.gridweb.data/gridworkbooksettings/precisionasdisplayed) { get; set; } | Bu çalışma kitabındaki hesaplamalar yalnızca sayıların gösterildiği gibi kesinliği kullanılarak yapılacaksa doğrudur |
| [ReCalculateOnOpen](../../aspose.cells.gridweb.data/gridworkbooksettings/recalculateonopen) { get; set; } | Dosya açılırken tüm formüllerin yeniden hesaplanıp hesaplanmayacağını alır veya ayarlar. |

### Örnekler

```csharp
[C#]

 

GridWorkbookSettings gsettings = new GridWorkbookSettings();
gridweb.Settings=gsettings;

//işini yap

[Visual Basic]


Dim gsettings as GridWorkbookSettings = new GridWorkbookSettings()
 gridweb..Settings=gsettings;
 
'işini yap
```

### Ayrıca bakınız

* ad alanı [Aspose.Cells.GridWeb.Data](../../aspose.cells.gridweb.data)
* toplantı [Aspose.Cells.GridWeb](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.GridWeb.dll -->
