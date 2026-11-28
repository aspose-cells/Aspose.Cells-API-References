---
title: "Enum OperatorType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.OperatorType enum. Koşullu biçimlendirme ve veri doğrulama için operatör tipini temsil eder"
type: docs
url: /tr/net/aspose.cells/operatortype/
---
## OperatorType enumeration

Koşullu biçimlendirme ve veri doğrulamanın operatör türünü temsil eder.

```csharp
public enum OperatorType
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| Between | `0` | Koşullu biçimlendirme ve veri doğrulama için Between operatörünü temsil eder. |
| Equal | `1` | Koşullu biçimlendirme ve veri doğrulama için Equal operatörünü temsil eder. |
| GreaterThan | `2` | Koşullu biçimlendirme ve veri doğrulama için GreaterThan operatörünü temsil eder. |
| GreaterOrEqual | `3` | Koşullu biçimlendirme ve veri doğrulama için GreaterOrEqual operatörünü temsil eder. |
| LessThan | `4` | Koşullu biçimlendirme ve veri doğrulama için LessThan operatörünü temsil eder. |
| LessOrEqual | `5` | Koşullu biçimlendirme ve veri doğrulama için LessOrEqual operatörünü temsil eder. |
| None | `6` | Karşılaştırma yoktur. |
| NotBetween | `7` | Koşullu biçimlendirme ve veri doğrulama için NotBetween operatörünü temsil eder. |
| NotEqual | `8` | Koşullu biçimlendirme ve veri doğrulama için NotEqual operatörünü temsil eder. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class OperatorTypeDemo
    {
        public static void OperatorTypeExample()
        {
            // Yeni bir Workbook oluşturun
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Boş bir koşullu biçimlendirme ekle
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = worksheet.ConditionalFormattings[index];

            // Koşullu biçimlendirme aralığını ayarla
            CellArea ca = new CellArea { StartRow = 0, EndRow = 10, StartColumn = 0, EndColumn = 10 };
            fcs.AddArea(ca);

            // OperatorType.Between ile bir koşul ekle
            int conditionIndex = fcs.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "=A1", "100");
            FormatCondition fc = fcs[conditionIndex];
            fc.Style.BackgroundColor = System.Drawing.Color.Yellow;

            // OperatorType.GreaterThan ile bir başka koşul ekle
            int conditionIndex2 = fcs.AddCondition(FormatConditionType.CellValue, OperatorType.GreaterThan, "50", null);
            FormatCondition fc2 = fcs[conditionIndex2];
            fc2.Style.BackgroundColor = System.Drawing.Color.Green;

            // Çalışma kitabını kaydedin
            workbook.Save("OperatorTypeExample.xlsx");

            return;
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


