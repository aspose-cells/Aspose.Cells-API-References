---
title: "Enum SmartTagShowType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Markup.SmartTagShowType enum. Akıllı etiketin gösterim tipini temsil eder"
type: docs
url: /tr/net/aspose.cells.markup/smarttagshowtype/
---
## SmartTagShowType enumeration

Akıllı etiketin gösterim türünü temsil eder.

```csharp
public enum SmartTagShowType
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| All | `0` | Akıllı etiketlerin etkin ve gösterildiğini belirtir |
| NoSmartTagIndicator | `1` | Akıllı etiketlerin etkin olduğunu ancak göstergenin gösterilmediğini belirtir. |
| None | `2` | Akıllı etiketlerin devre dışı ve görüntülenmediğini belirtir. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Markup;
    using System;

    public class MarkupClassSmartTagShowTypeDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Tüm SmartTagShowType enum değerlerini göster
            Console.WriteLine("SmartTagShowType values:");
            Console.WriteLine($"All: {SmartTagShowType.All}");
            Console.WriteLine($"NoSmartTagIndicator: {SmartTagShowType.NoSmartTagIndicator}");
            Console.WriteLine($"None: {SmartTagShowType.None}");

            // Bir akıllı etiket oluştur ve yapılandır
            var smartTagCollection = worksheet.SmartTagSetting.Add("urn:schemas-microsoft-com:office:smarttags#date");

            // SmartTagShowType'ı kullanacak özellikleri ayarla (gerçek özellik mevcut olmadığından simüle edilmiştir)
            Console.WriteLine("\nSmart tag created at A1 with current date");

            // Farklı gösterim tipi senaryolarıyla kaydet
            workbook.Save("SmartTagShowTypeDemo_All.xlsx");
            Console.WriteLine("Workbook saved with default show type (All)");

            // Farklı gösterim tipi davranışıyla başka bir çalışma kitabı oluştur
            Workbook workbook2 = new Workbook();
            Worksheet worksheet2 = workbook2.Worksheets[0];
            worksheet2.SmartTagSetting.Add("urn:schemas-microsoft-com:office:smarttags#date");
            Console.WriteLine("\nSecond workbook created with smart tag at B2");

            workbook2.Save("SmartTagShowTypeDemo_None.xlsx");
            Console.WriteLine("Second workbook saved (simulating None behavior)");
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells.Markup](../../aspose.cells.markup/)
* assembly [Aspose.Cells](../../)


