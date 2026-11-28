---
title: "FormatCondition.Type"
second_title: "Aspose.Cells için .NET API Referansı"
description: "FormatCondition özelliği. Koşullu biçimlendirme türünü alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells/formatcondition/type/
---
## FormatCondition.Type property

Koşullu biçimlendirme tipinin olup olmadığını alır ve ayarlar.

```csharp
public FormatConditionType Type { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FormatConditionPropertyTypeDemo
    {
        public static void Run()
        {
            // Bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Örnek veri ekleyin.
            sheet.Cells["A1"].PutValue(10);
            sheet.Cells["A2"].PutValue(20);
            sheet.Cells["A3"].PutValue(30);

            // Koşullu biçimlendirme oluştur
            int index = sheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = sheet.ConditionalFormattings[index];
            
            // İfade türüyle biçim koşulu ekle (düzeltilmiş parametreler)
            int conditionIndex = fcs.AddCondition(FormatConditionType.Expression, OperatorType.None, "=A1>5", null);
            FormatCondition fc = fcs[conditionIndex];
            
            // Koşul için stili ayarla
            Style style = workbook.CreateStyle();
            style.Font.Color = System.Drawing.Color.Red;
            fc.Style = style;

            // Type özelliğinin kullanımını gösterin.
            Console.WriteLine("Format Condition Type: " + fc.Type);
            
            // Çalışma kitabını kaydedin
            workbook.Save("FormatConditionPropertyTypeDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* enum [FormatConditionType](../../formatconditiontype/)
* class [FormatCondition](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


