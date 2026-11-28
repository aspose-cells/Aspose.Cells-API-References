---
title: "Range.GetEnumerator"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Range yöntemi. Bu Range içindeki hücreler için yineleyiciyi alır"
type: docs
url: /tr/net/aspose.cells/range/getenumerator/
---
## Range.GetEnumerator method

Bu Range içindeki hücreler için yineleyiciyi alır.

```csharp
public IEnumerator GetEnumerator()
```

### Dönüş Değeri

Hücre sayacı

### Açıklamalar

Dönen Enumerator ile öğeler dolaşılırken, hücre koleksiyonu değiştirilmemelidir (örneğin yeni Hücre/Row oluşturulmasına veya mevcut Hücre/Row silinmesine neden olacak işlemler). Aksi takdirde enumerator tüm hücreleri doğru şekilde dolaşamayabilir (bazı öğeler tekrar tekrar dolaşılabilir veya atlanabilir).

### Örnekler

```csharp
using System;
using System.Collections;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangeMethodGetEnumeratorDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Biraz örnek veri doldurun
            worksheet.Cells["B2"].PutValue("Apple");
            worksheet.Cells["B3"].PutValue("Banana");
            worksheet.Cells["C2"].PutValue("Cherry");
            worksheet.Cells["C3"].PutValue("Date");

            // Aralığı al ve hücreler arasında yinele
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("B2:C3");
            IEnumerator enumerator = range.GetEnumerator();
            
            while (enumerator.MoveNext())
            {
                Cell cell = (Cell)enumerator.Current;
                Console.WriteLine($"{cell.Name}: {cell.Value}");
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


