---
title: "DataSorterKey.Type"
second_title: "Aspose.Cells için .NET API Referansı"
description: "DataSorterKey özelliği. Sıralama türünü temsil eder"
type: docs
url: /tr/net/aspose.cells/datasorterkey/type/
---
## DataSorterKey.Type property

Sıralama türünü temsil eder.

```csharp
public SortOnType Type { get; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DataSorterKeyPropertyTypeDemo
    {
        public static void Run()
        {
            // Bir çalışma kitabı nesnesi oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Örnek veri ekleyin.
            worksheet.Cells["A1"].PutValue("USA");
            worksheet.Cells["A2"].PutValue("China");
            worksheet.Cells["A3"].PutValue("Brazil");
            worksheet.Cells["A4"].PutValue("Russia");
            worksheet.Cells["A5"].PutValue("Canada");

            // Veri sıralayıcı oluştur ve anahtar ekle
            DataSorter sorter = workbook.DataSorter;
            sorter.AddKey(0, SortOrder.Ascending);

            // Verileri sırala
            CellArea ca = CellArea.CreateCellArea("A1", "A5");
            sorter.Sort(worksheet.Cells, ca);

            // Type özelliğinin kullanımını gösterin.
            foreach (DataSorterKey key in sorter.Keys)
            {
                Console.WriteLine($"Key Type: {key.Type}");
            }
        }
    }
}
```

### Ayrıca Bakınız

* enum [SortOnType](../../sortontype/)
* class [DataSorterKey](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


