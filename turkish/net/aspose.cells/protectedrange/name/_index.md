---
title: "ProtectedRange.Name"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ProtectedRange özelliği. Aralık başlığını alır. Bu, adlandırılmış bir aralık tanımı olarak değil, bir tanımlayıcı olarak kullanılır."
type: docs
url: /tr/net/aspose.cells/protectedrange/name/
---
## ProtectedRange.Name property

Aralık başlığını alır. Bu, adlandırılmış bir aralık tanımı yerine bir tanımlayıcı olarak kullanılır.

```csharp
public string Name { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ProtectedRangePropertyNameDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Korunan aralık koleksiyonu oluştur
            ProtectedRangeCollection allowRanges = worksheet.AllowEditRanges;

            // Adı "MyRange" olan bir korunan aralık ekle
            int index = allowRanges.Add("MyRange", 0, 0, 2, 2);
            ProtectedRange protectedRange = allowRanges[index];
            protectedRange.Password = "123";

            // Name özelliğine eriş ve göster
            Console.WriteLine("Protected range name: " + protectedRange.Name);
            Console.WriteLine("Cell area: {0},{1} to {2},{3}", 
                protectedRange.CellArea.StartRow,
                protectedRange.CellArea.StartColumn,
                protectedRange.CellArea.EndRow,
                protectedRange.CellArea.EndColumn);

            // Başka bir adlandırılmış aralık ekle
            index = allowRanges.Add("SecondRange", 3, 3, 5, 5);
            ProtectedRange secondRange = allowRanges[index];
            Console.WriteLine("Second protected range name: " + secondRange.Name);

            // Çalışma kitabını kaydedin
            workbook.Save("ProtectedRangeDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [ProtectedRange](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


