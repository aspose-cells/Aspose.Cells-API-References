---
title: "UnionRange.GetEnumerator"
second_title: "Aspose.Cells için .NET API Referansı"
description: "UnionRange yöntemi. Bu aralıktaki hücreler için yineleyiciyi alır"
type: docs
url: /tr/net/aspose.cells/unionrange/getenumerator/
---
## UnionRange.GetEnumerator method

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
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Collections;

    public class UnionRangeMethodGetEnumeratorDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluşturun ve ilk çalışma sayfasını alın.
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // İlk aralığı (A1:B2) oluşturun ve verilerle doldurun
            Aspose.Cells.Range range1 = worksheet.Cells.CreateRange("A1", "B2");
            range1[0, 0].PutValue("R1C1");
            range1[0, 1].PutValue("R1C2");
            range1[1, 0].PutValue("R2C1");
            range1[1, 1].PutValue("R2C2");

            // İkinci aralığı (C1:D2) oluşturun ve verilerle doldurun
            Aspose.Cells.Range range2 = worksheet.Cells.CreateRange("C1", "D2");
            range2[0, 0].PutValue("R1C3");
            range2[0, 1].PutValue("R1C4");
            range2[1, 0].PutValue("R2C3");
            range2[1, 1].PutValue("R2C4");

            try
            {
                // İlk aralıktan bir UnionRange oluşturun
                UnionRange unionRange = worksheet.Cells
                    .CreateRange("A1:B2")
                    .UnionRanges(new Aspose.Cells.Range[] { range1 });

                // İkinci aralığı birliğe ekleyin
                unionRange = unionRange.Union("C1:D2");

                // Enumerator'ı elde edin ve birliğin içindeki tüm hücrelerde yineleyin
                IEnumerator enumerator = unionRange.GetEnumerator();
                Console.WriteLine("Enumerating cells in the UnionRange:");
                while (enumerator.MoveNext())
                {
                    Cell cell = enumerator.Current as Cell;
                    if (cell != null)
                    {
                        Console.WriteLine($"{cell.Name}: {cell.Value}");
                    }
                }

                // Çalışma kitabını kaydedin (isteğe bağlı, sadece verilerin kalıcı olduğunu göstermek için)
                workbook.Save("UnionRangeGetEnumeratorDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling GetEnumerator: {ex.Message}");
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [UnionRange](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


