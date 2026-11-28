---
title: "Cells.GetEnumerator"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Cells yöntemi. Hücre enumeratörünü alır"
type: docs
url: /tr/net/aspose.cells/cells/getenumerator/
---
## Cells.GetEnumerator method

Hücre enumeratörünü alır.

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
    public class CellsMethodGetEnumeratorDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Hücrelere örnek veri ekle
            worksheet.Cells["A1"].PutValue("Hello");
            worksheet.Cells["B1"].PutValue(123);
            worksheet.Cells["A2"].PutValue(DateTime.Now);
            
            // Enumerator'ı al ve hücreler arasında yinele
            IEnumerator enumerator = worksheet.Cells.GetEnumerator();
            while (enumerator.MoveNext())
            {
                Cell cell = (Cell)enumerator.Current;
                if (cell.Value != null)
                {
                    Console.WriteLine($"{cell.Name}: {cell.Value}");
                }
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


