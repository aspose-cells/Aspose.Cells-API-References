---
title: "Sınıf FormulaSettings"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.FormulaSettings sınıfı. Formüllerin ve hesaplamanın ayarları"
type: docs
url: /tr/net/aspose.cells/formulasettings/
---
## FormulaSettings class

Formüllerin ve hesaplamanın ayarları.

```csharp
public class FormulaSettings
```

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [CalculateOnOpen](../../aspose.cells/formulasettings/calculateonopen/) { get; set; } | Uygulamanın çalışma kitabı açıldığında tam bir hesaplama yapması gerekip gerekmediğini gösterir. |
| [CalculateOnSave](../../aspose.cells/formulasettings/calculateonsave/) { get; set; } | Manuel hesaplama modundayken belgeyi kaydetmeden önce çalışma kitabının yeniden hesaplanıp hesaplanmayacağını gösterir. |
| [CalculationId](../../aspose.cells/formulasettings/calculationid/) { get; set; } | Çalışma kitabındaki değerleri hesaplamak için kullanılan hesaplama motorunun sürümünü belirtir. |
| [CalculationMode](../../aspose.cells/formulasettings/calculationmode/) { get; set; } | MS Excel'de çalışma kitabı hesaplama modunu alır veya ayarlar. |
| [EnableCalculationChain](../../aspose.cells/formulasettings/enablecalculationchain/) { get; set; } | Formüller için hesaplama zincirinin etkinleştirilip etkinleştirilmeyeceğini gösterir. Varsayılan değer false'tur. |
| [EnableIterativeCalculation](../../aspose.cells/formulasettings/enableiterativecalculation/) { get; set; } | Döngüsel referansları çözmek için yinelemeli hesaplamanın etkinleştirilip etkinleştirilmeyeceğini gösterir. |
| [ForceFullCalculation](../../aspose.cells/formulasettings/forcefullcalculation/) { get; set; } | Bir hesaplama tetiklendiğinde tüm formüllerin her seferinde hesaplanıp hesaplanmayacağını gösterir. |
| [MaxChange](../../aspose.cells/formulasettings/maxchange/) { get; set; } | Döngüsel bir referansı çözmek için azami değişim. |
| [MaxIteration](../../aspose.cells/formulasettings/maxiteration/) { get; set; } | Döngüsel bir referansı çözmek için azami yineleme sayısı. |
| [PrecisionAsDisplayed](../../aspose.cells/formulasettings/precisionasdisplayed/) { get; set; } | Formüller hesaplanırken hesaplanan sonucun hassasiyetinin gösterildiği gibi ayarlanıp ayarlanmayacağını gösterir. |
| [PreservePaddingSpaces](../../aspose.cells/formulasettings/preservepaddingspaces/) { get; set; } | Formülleri alırken ve ayarlarken formül tokenları arasında doldurulan boşlukları ve satır sonlarını koruyup korumayacağını gösterir. Varsayılan değer false'tur. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class FormulaSettingsDemo
    {
        public static void FormulaSettingsExample()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // Çalışma kitabının formül ayarlarına erişin
            FormulaSettings formulaSettings = workbook.Settings.FormulaSettings;

            // Özellikleri ayarlama
            formulaSettings.CalculateOnOpen = true;
            formulaSettings.CalculateOnSave = true;
            formulaSettings.ForceFullCalculation = false;
            formulaSettings.CalculationMode = CalcModeType.Automatic;
            formulaSettings.CalculationId = "0";
            formulaSettings.EnableIterativeCalculation = true;
            formulaSettings.MaxIteration = 100;
            formulaSettings.MaxChange = 0.001;
            formulaSettings.PrecisionAsDisplayed = false;
            formulaSettings.EnableCalculationChain = true;
            formulaSettings.PreservePaddingSpaces = false;

            // Çalışma kitabını kaydedin
            workbook.Save("FormulaSettingsExample.xlsx");
            workbook.Save("FormulaSettingsExample.pdf");
            return;
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


