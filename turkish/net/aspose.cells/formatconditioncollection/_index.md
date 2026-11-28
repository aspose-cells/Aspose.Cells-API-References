---
title: "Sınıf FormatConditionCollection"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.FormatConditionCollection sınıfı. Koşullu biçimlendirmeyi temsil eder. FormatConditions en fazla üç koşullu biçim içerebilir"
type: docs
url: /tr/net/aspose.cells/formatconditioncollection/
---
## FormatConditionCollection class

Koşullu biçimlendirmeyi temsil eder. FormatConditions üçe kadar koşullu biçimlendirme içerebilir.

```csharp
public class FormatConditionCollection
```

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [Count](../../aspose.cells/formatconditioncollection/count/) { get; } | Koşulların sayısını alır. |
| [Item](../../aspose.cells/formatconditioncollection/item/) { get; } | Biçimlendirme koşulunu dizine göre alır. |
| [RangeCount](../../aspose.cells/formatconditioncollection/rangecount/) { get; } | Koşullu biçimlendirilmiş aralıkların sayısını alır. |

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| [Add](../../aspose.cells/formatconditioncollection/add/)(CellArea, FormatConditionType, OperatorType, string, string) | Bir biçimlendirme koşulu ve etkilenen hücre aralığını FormatConditions'a ekler. FormatConditions en fazla üç koşullu biçim içerebilir. Koşullu biçimlendirme formüllerinde diğer sayfalara referans verilmesine izin verilmez. |
| [AddArea](../../aspose.cells/formatconditioncollection/addarea/)(CellArea) | Koşullu biçimlendirilmiş bir hücre aralığı ekler. |
| [AddCondition](../../aspose.cells/formatconditioncollection/addcondition/#addcondition)(FormatConditionType) | Bir biçim koşulu ekle. |
| [AddCondition](../../aspose.cells/formatconditioncollection/addcondition/#addcondition_1)(FormatConditionType, OperatorType, string, string) | Bir biçimlendirme koşulu ekler. |
| [GetCellArea](../../aspose.cells/formatconditioncollection/getcellarea/)(int) | Koşullu biçimlendirilmiş hücre aralığını dizine göre alır. |
| [RemoveArea](../../aspose.cells/formatconditioncollection/removearea/#removearea_1)(int) | Koşullu biçimlendirilmiş hücre aralığını dizine göre kaldırır. |
| [RemoveArea](../../aspose.cells/formatconditioncollection/removearea/#removearea)(int, int, int, int) | Aralıktaki koşullu biçimlendirmeyi kaldır. |
| [RemoveCondition](../../aspose.cells/formatconditioncollection/removecondition/)(int) | Biçimlendirme koşulunu dizine göre kaldırır. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class FormatConditionCollectionDemo
    {
        public static void FormatConditionCollectionExample()
        {
            // Yeni bir Workbook oluşturun
            Workbook workbook = new Workbook();

            // İlk çalışma sayfasını al
            Worksheet sheet = workbook.Worksheets[0];

            // Boş bir koşullu biçimlendirme ekler
            int index = sheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = sheet.ConditionalFormattings[index];

            // Koşullu biçimlendirme aralığını ayarlar
            CellArea ca = new CellArea { StartRow = 0, EndRow = 0, StartColumn = 0, EndColumn = 0 };
            fcs.AddArea(ca);
            ca = new CellArea { StartRow = 1, EndRow = 1, StartColumn = 1, EndColumn = 1 };
            fcs.AddArea(ca);

            // Koşullar ekler
            int conditionIndex1 = fcs.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "=A2", "100");
            int conditionIndex2 = fcs.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "50", "100");

            // Arka plan rengini ayarlar
            FormatCondition fc1 = fcs[conditionIndex1];
            fc1.Style.BackgroundColor = System.Drawing.Color.Red;

            // Excel dosyasını kaydetme
            workbook.Save("FormatConditionCollectionExample.xlsx");
            workbook.Save("FormatConditionCollectionExample.pdf");
            return;
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


