---
title: "GroupShape.Item"
second_title: "Aspose.Cells için .NET API Referansı"
description: "GroupShape özelliği. Çocuk şekli indeksine göre alır"
type: docs
url: /tr/net/aspose.cells.drawing/groupshape/item/
---
## GroupShape indexer

Çocuk şekli indeksine göre alır.

```csharp
public Shape this[int index] { get; }
```

| Parametre | Açıklama |
| --- | --- |
| indeks | çocuk şeklinin indeksi. |

### Dönüş Değeri

çocuk şekli döndürür.

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class GroupShapePropertyItemDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // İki dikdörtgen şekil oluştur
            Shape shape1 = worksheet.Shapes.AddRectangle(0, 0, 100, 100, 0, 0);
            Shape shape2 = worksheet.Shapes.AddRectangle(50, 50, 100, 100, 0, 0);

            // Şekilleri grupla
            Shape[] shapesToGroup = new Shape[] { shape1, shape2 };
            GroupShape groupShape = worksheet.Shapes.Group(shapesToGroup);

            // İlk şeklin özelliklerine eriş ve göster
            Shape firstShape = groupShape[0];
            Console.WriteLine($"First shape initial name: {firstShape.Name}");
            Console.WriteLine($"First shape initial text: {firstShape.Text}");

            // Item erişimiyle ilk şeklin özelliklerini değiştir
            firstShape.Name = "ModifiedRectangle1";
            firstShape.Text = "First Grouped Shape";

            // İkinci şekle doğrudan indeksleyiciyle eriş ve değiştir
            groupShape[1].Text = "Second Grouped Shape";

            // Değişiklikleri doğrula
            Console.WriteLine($"\nFirst shape updated name: {groupShape[0].Name}");
            Console.WriteLine($"First shape updated text: {groupShape[0].Text}");
            Console.WriteLine($"Second shape updated text: {groupShape[1].Text}");

            // Değiştirilmiş çalışma kitabını kaydet
            workbook.Save("GroupShapePropertyItemDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Shape](../../shape/)
* class [GroupShape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


