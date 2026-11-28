---
title: "Enum LookAtType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.LookAtType enum. Arama türünü temsil eder"
type: docs
url: /tr/net/aspose.cells/lookattype/
---
## LookAtType enumeration

Bakma türünü temsil eder.

```csharp
public enum LookAtType
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| Contains | `0` | Hücre değeri arama nesnesini içerir. |
| StartWith | `1` | Hücre değeri arama nesnesiyle başlar. |
| EndWith | `2` | Hücre değeri arama nesnesiyle biter. |
| EntireContent | `3` | Hücre değeri arama nesnesiyle aynıdır. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class LookAtTypeDemo
    {
        public static void LookAtTypeExample()
        {
            // Çalışma kitabı nesnesini örnekle
            Workbook workbook = new Workbook("LookAtTypeExample_original.xlsx");

            // Hücreler koleksiyonunu al
            Cells cells = workbook.Worksheets[0].Cells;

            // FindOptions nesnesini örnekle
            FindOptions findOptions = new FindOptions();

            // Bir Hücre Alanı oluştur
            CellArea ca = new CellArea();
            ca.StartRow = 8;
            ca.StartColumn = 2;
            ca.EndRow = 17;
            ca.EndColumn = 13;

            // FindOptions için hücre alanını ayarla
            findOptions.SetRange(ca);

            // Arama özelliklerini ayarla
            findOptions.SearchBackward = false;
            findOptions.SearchOrderByRows = true;
            findOptions.LookInType = LookInType.Values;

            // LookAtType'ı Contains olarak ayarla
            findOptions.LookAtType = LookAtType.Contains;

            // Belirli bir değere sahip hücreyi bul
            Cell cell = cells.Find("searchValue", null, findOptions);

            if (cell != null)
            {
                Console.WriteLine($"Cell found at row {cell.Row}, column {cell.Column}");
            }
            else
            {
                Console.WriteLine("Cell not found.");
            }
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


