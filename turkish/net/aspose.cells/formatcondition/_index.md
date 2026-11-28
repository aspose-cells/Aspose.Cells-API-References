---
title: "FormatCondition sınıfı"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.FormatCondition sınıfı. Koşullu biçimlendirme koşulunu temsil eder"
type: docs
url: /tr/net/aspose.cells/formatcondition/
---
## FormatCondition class

Koşullu biçimlendirme koşulunu temsil eder.

```csharp
public class FormatCondition
```

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [AboveAverage](../../aspose.cells/formatcondition/aboveaverage/) { get; } | Koşullu biçimlendirme'nin "AboveAverage" örneğini al. Varsayılan örneğin kuralı, aralıktaki tüm değerlerin ortalamasının üzerindeki hücreleri vurgular. Yalnızca type = AboveAverage için geçerlidir. |
| [ColorScale](../../aspose.cells/formatcondition/colorscale/) { get; } | Koşullu biçimlendirme'nin "ColorScale" örneğini al. Varsayılan örnek, "yeşil-sarı-kırmızı" 3ColorScale'dir. Yalnızca type = ColorScale için geçerlidir. |
| [DataBar](../../aspose.cells/formatcondition/databar/) { get; } | Koşullu biçimlendirme'nin "DataBar" örneğini al. Varsayılan örneğin rengi mavidir. Yalnızca type = DataBar için geçerlidir. |
| [Formula1](../../aspose.cells/formatcondition/formula1/) { get; set; } | Koşullu biçimlendirme ile ilişkili değeri veya ifadeyi alır ve ayarlar. |
| [Formula2](../../aspose.cells/formatcondition/formula2/) { get; set; } | Koşullu biçimlendirme ile ilişkili değeri veya ifadeyi alır ve ayarlar. |
| [IconSet](../../aspose.cells/formatcondition/iconset/) { get; } | Koşullu biçimlendirme'nin "IconSet" örneğini al. Varsayılan örneğin IconSetType'ı TrafficLights31'dir. Yalnızca type = IconSet için geçerlidir. |
| [Operator](../../aspose.cells/formatcondition/operator/) { get; set; } | Koşullu biçimlendirme operatör tipini alır ve ayarlar. |
| [Priority](../../aspose.cells/formatcondition/priority/) { get; set; } | Bu koşullu biçimlendirme kuralının önceliği. Bu değer, hangi biçimin değerlendirileceğini ve işleneceğini belirlemek için kullanılır. Daha düşük sayısal değerler, daha yüksek sayısal değerlerden daha yüksek önceliğe sahiptir; '1' en yüksek önceliği temsil eder. |
| [StopIfTrue](../../aspose.cells/formatcondition/stopiftrue/) { get; set; } | Doğru, bu kural doğru değerlendirildiğinde, daha düşük öncelikli kurallar bu kuralın üzerine uygulanamaz. Yalnızca Excel 2007 için geçerlidir; |
| [Style](../../aspose.cells/formatcondition/style/) { get; set; } | Koşullu biçimlendirilmiş hücre aralıklarının stilini alır veya ayarlar. |
| [Text](../../aspose.cells/formatcondition/text/) { get; set; } | "text contains" koşullu biçimlendirme kuralındaki metin değeridir. Yalnızca type = containsText, notContainsText, beginsWith ve endsWith için geçerlidir. Varsayılan değer null'dur. |
| [TimePeriod](../../aspose.cells/formatcondition/timeperiod/) { get; set; } | "date occurrin" koşullu biçimlendirme kuralındaki uygulanabilir zaman dilimidir. Yalnızca type = timePeriod için geçerlidir. Varsayılan değer TimePeriodType.Today'dir. |
| [Top10](../../aspose.cells/formatcondition/top10/) { get; } | Koşullu biçimlendirme'nin "Top10" örneğini al. Varsayılan örneğin kuralı, değerleri en üst 10 dilimine düşen hücreleri vurgular. Yalnızca type = Top10 için geçerlidir. |
| [Type](../../aspose.cells/formatcondition/type/) { get; set; } | Koşullu biçimlendirme tipinin olup olmadığını alır ve ayarlar. |

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| [GetFormula1](../../aspose.cells/formatcondition/getformula1/#getformula1)(bool, bool) | Bu biçim koşuluyla ilişkili değeri veya ifadeyi alır. |
| [GetFormula1](../../aspose.cells/formatcondition/getformula1/#getformula1_2)(int, int) | Hücrenin koşullu biçimlendirme formülünü alır. |
| [GetFormula1](../../aspose.cells/formatcondition/getformula1/#getformula1_1)(bool, bool, int, int) | Hücrenin koşullu biçimlendirme değerini veya ifadesini alır. |
| [GetFormula2](../../aspose.cells/formatcondition/getformula2/#getformula2)(bool, bool) | Bu biçim koşuluyla ilişkili değeri veya ifadeyi alır. |
| [GetFormula2](../../aspose.cells/formatcondition/getformula2/#getformula2_2)(int, int) | Hücrenin koşullu biçimlendirme formülünü alır. |
| [GetFormula2](../../aspose.cells/formatcondition/getformula2/#getformula2_1)(bool, bool, int, int) | Hücrenin koşullu biçimlendirme değerini veya ifadesini alır. |
| [SetFormula1](../../aspose.cells/formatcondition/setformula1/)(string, bool, bool) | Bu biçim koşuluyla ilişkili değeri veya ifadeyi ayarlar. |
| [SetFormula2](../../aspose.cells/formatcondition/setformula2/)(string, bool, bool) | Bu biçim koşuluyla ilişkili değeri veya ifadeyi ayarlar. |
| [SetFormulas](../../aspose.cells/formatcondition/setformulas/)(string, string, bool, bool) | Bu biçim koşuluyla ilişkili değeri veya ifadeyi ayarlar. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class FormatConditionDemo
    {
        public static void FormatConditionExample()
        {
            // Yeni bir Workbook oluştur.
            Workbook workbook = new Workbook();

            // İlk çalışma sayfasını al.
            Worksheet sheet = workbook.Worksheets[0];

            // Boş bir koşullu biçimlendirme ekler
            int index = sheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = sheet.ConditionalFormattings[index];

            // Koşullu biçimlendirme aralığını ayarlar.
            CellArea ca = new CellArea
            {
                StartRow = 0,
                EndRow = 10,
                StartColumn = 0,
                EndColumn = 10
            };
            fcs.AddArea(ca);

            // Koşul ekler.
            int conditionIndex = fcs.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "=A2", "100");
            FormatCondition fc = fcs[conditionIndex];

            // Özellikleri ayarlama
            fc.Formula1 = "=A2";
            fc.Formula2 = "100";
            fc.Operator = OperatorType.Between;
            fc.StopIfTrue = true;
            fc.Priority = 1;
            fc.Style.BackgroundColor = Color.Red;
            fc.Type = FormatConditionType.CellValue;

            // Diğer özellikleri gösterme
            fc.Text = "Sample Text";
            fc.TimePeriod = TimePeriodType.Today;

            // Excel dosyasını kaydetme
            workbook.Save("FormatConditionExample.xlsx");
            workbook.Save("FormatConditionExample.pdf");
            return;
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


