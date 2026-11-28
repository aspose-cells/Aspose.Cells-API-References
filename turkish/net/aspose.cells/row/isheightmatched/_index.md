---
title: "Row.IsHeightMatched"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Satır özelliği. Satır yüksekliğinin çalışma kitabının mevcut varsayılan yazı tipi ayarına uygun olup olmadığını gösterir. Bu özelliğin doğru olması aynı zamanda satır yüksekliğinin kullanıcı tarafından özel bir değer ayarlanmadan otomatik olduğunu gösterir."
type: docs
url: /tr/net/aspose.cells/row/isheightmatched/
---
## Row.IsHeightMatched property

Satır yüksekliğinin çalışma kitabının mevcut varsayılan yazı tipi ayarına uyup uymadığını gösterir. Bu özelliğin true olması ayrıca satır yüksekliğinin kullanıcı tarafından özel bir değer ayarlanmamış "otomatik" olduğunu gösterir.

```csharp
public bool IsHeightMatched { get; set; }
```

### Açıklamalar

Bu özellik doğru olduğunda, bu satırdaki içerik değişirse, genellikle satır yüksekliğinin yeniden hesaplanması gerekir (örneğin [`AutoFitRows`](../../worksheet/autofitrows/) ile) çalışma kitabını MS Excel'de açtığınızda gösterilen sonuçla aynı sonucu elde etmek için.

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RowPropertyIsHeightMatchedDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Satır yüksekliğinin eşleşmesini göstermek için örnek veri ve stil ayarlayın
            worksheet.Cells["A1"].PutValue("This is a test string to demonstrate row height matching");
            worksheet.Cells["B1"].PutValue("Another cell in the same row");
            
            // Yükseklik ayarlamasını zorlamak için kelime kaydırmayı uygulayın
            Style style = worksheet.Cells["A1"].GetStyle();
            style.IsTextWrapped = true;
            worksheet.Cells["A1"].SetStyle(style);
            
            // Satırı içeriğin yüksekliğine uyacak şekilde otomatik sığdırın
            worksheet.AutoFitRow(0);
            
            // Satır yüksekliğinin içeriğiyle eşleşip eşleşmediğini kontrol edin
            Console.WriteLine("Is row height matched: " + worksheet.Cells.Rows[0].IsHeightMatched);
        }
    }
}
```

### Ayrıca Bakınız

* class [Row](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


