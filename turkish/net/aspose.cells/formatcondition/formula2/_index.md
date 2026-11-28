---
title: "FormatCondition.Formula2"
second_title: "Aspose.Cells için .NET API Referansı"
description: "FormatCondition özelliği. Koşullu biçimlendirme ile ilişkili değeri veya ifadeyi alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells/formatcondition/formula2/
---
## FormatCondition.Formula2 property

Koşullu biçimlendirme ile ilişkili değeri veya ifadeyi alır ve ayarlar.

```csharp
public string Formula2 { get; set; }
```

### Açıklamalar

Lütfen formülü ayarlamadan önce tüm alanları ekleyin. Bu koşul için formül ayarlarken, giriş değeri '=' ile başlıyorsa formül olarak kabul edilir. Aksi takdirde düz değer (metin, sayı, bool) olarak alınır. '=' ile başlayan metin değeri için kullanıcı, formülü şu formatta girebilir: \"=\\\"=...\\\"\".

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FormatConditionPropertyFormula2Demo
    {
        public static void Run()
        {
            // Bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Koşullu biçimlendirme ekle
            ConditionalFormattingCollection conditionalFormattings = worksheet.ConditionalFormattings;
            int index = conditionalFormattings.Add();
            FormatConditionCollection formatConditions = conditionalFormattings[index];
            
            // Hücre aralığını tanımla
            CellArea area = CellArea.CreateCellArea(0, 0, 1, 1);
            
            // Formula2 ile biçim koşulu ekle
            formatConditions.Add(area, 
                FormatConditionType.CellValue, 
                OperatorType.Between, 
                "=\"abc def\"", 
                "=\"a\"&\"b\"");

            // Biçim koşulunu al
            FormatCondition formatCondition = formatConditions[0];

            // Formülleri çıktı olarak ver
            Console.WriteLine("Formula1: " + formatCondition.Formula1);
            Console.WriteLine("Formula2: " + formatCondition.Formula2);

            // Çalışma kitabını kaydedin
            workbook.Save("FormatConditionFormula2Demo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Ayrıca Bakınız

* class [FormatCondition](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


