---
title: "CellArea.CompareTo"
second_title: "Aspose.Cells için .NET API Referansı"
description: "CellArea yöntemi. İki CellArea nesnesini sol üst köşelerine göre karşılaştırır"
type: docs
url: /tr/net/aspose.cells/cellarea/compareto/
---
## CellArea.CompareTo method

İki CellArea nesnesini sol üst köşelerine göre karşılaştırın.

```csharp
public int CompareTo(object obj)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| obj | Object |  |

### Dönüş Değeri

İki köşe farklı satırlarda ise satır indekslerini karşılaştırın. Aksi takdirde sütun indekslerini karşılaştırın. Köşeler aynıysa 0 döndürülür.

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellAreaMethodCompareToWithObjectDemo
    {
        public static void Run()
        {
            // Karşılaştırma için iki CellArea nesnesi oluştur
            CellArea ca1 = new CellArea { StartRow = 0, EndRow = 10, StartColumn = 0, EndColumn = 10 };
            object ca2 = new CellArea { StartRow = 0, EndRow = 5, StartColumn = 0, EndColumn = 5 };

            // Object parametresiyle CompareTo yöntemini göster
            int comparisonResult = ca1.CompareTo(ca2);
            Console.WriteLine($"Comparison result: {comparisonResult}");

            // Eşit alanlarla başka bir karşılaştırma oluştur
            object ca3 = new CellArea { StartRow = 0, EndRow = 10, StartColumn = 0, EndColumn = 10 };
            comparisonResult = ca1.CompareTo(ca3);
            Console.WriteLine($"Comparison result with equal areas: {comparisonResult}");
        }
    }
}
```

### Ayrıca Bakınız

* struct [CellArea](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


