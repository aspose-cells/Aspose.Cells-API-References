---
title: "GroupShape.Ungroup"
second_title: "Aspose.Cells için .NET API Referansı"
description: "GroupShape yöntemi. Şekil öğelerinin grubunu çözer"
type: docs
url: /tr/net/aspose.cells.drawing/groupshape/ungroup/
---
## GroupShape.Ungroup method

Şekil öğelerinin gruplarını çöz.

```csharp
public void Ungroup()
```

### Açıklamalar

Grup şekli başka bir grup şekli tarafından gruplanmışsa, hiçbir şey yapılmaz.

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class GroupShapeMethodUngroupDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // İki dikdörtgen şekil ekle
            Shape shape1 = worksheet.Shapes.AddRectangle(0, 0, 0, 0, 100, 50);
            Shape shape2 = worksheet.Shapes.AddRectangle(0, 0, 3, 0, 100, 50);

            // Şekilleri bir GroupShape içine grupla
            GroupShape groupShape = worksheet.Shapes.Group(new Shape[] { shape1, shape2 });

            try
            {
                // Ungroup yöntemini çalıştır
                groupShape.Ungroup();
                Console.WriteLine("Shapes ungrouped successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error during ungrouping: {ex.Message}");
            }

            workbook.Save("GroupShapeUngroupDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [GroupShape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


