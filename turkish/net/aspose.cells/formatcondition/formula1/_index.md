---
title: "FormatCondition.Formula1"
second_title: "Aspose.Cells için .NET API Referansı"
description: "FormatCondition özelliği. Koşullu biçimlendirme ile ilişkili değeri veya ifadeyi alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells/formatcondition/formula1/
---
## FormatCondition.Formula1 property

Koşullu biçimlendirme ile ilişkili değeri veya ifadeyi alır ve ayarlar.

```csharp
public string Formula1 { get; set; }
```

### Açıklamalar

Lütfen formülü ayarlamadan önce tüm alanları ekleyin. Bu koşul için formül ayarlarken, giriş değeri '=' ile başlıyorsa formül olarak kabul edilir. Aksi takdirde düz değer (metin, sayı, bool) olarak alınır. '=' ile başlayan metin değeri için kullanıcı, formülü şu formatta girebilir: \"=\\\"=...\\\"\".

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FormatConditionPropertyFormula1Demo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Örnek veri ekleyin.
            worksheet.Cells["E1"].PutValue(50);
            
            // Koşullu biçimlendirme ekle
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcc = worksheet.ConditionalFormattings[index];
            
            // Aralığı ve koşul tipini ayarla
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.StartColumn = 0;
            area.EndRow = 5;
            area.EndColumn = 5;
            fcc.AddCondition(FormatConditionType.CellValue, OperatorType.LessOrEqual, "=$E$1<=100", null);
            
            // Formula1 özelliğine eriş ve göster
            FormatCondition fc = fcc[0];
            Console.WriteLine("Formula1: " + fc.Formula1);
        }
    }
}
```

### Ayrıca Bakınız

* class [FormatCondition](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


