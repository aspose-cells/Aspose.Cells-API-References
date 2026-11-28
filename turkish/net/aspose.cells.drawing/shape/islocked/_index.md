---
title: "Shape.IsLocked"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Shape özelliği. True değeri, sayfa korunduğunda nesnenin değiştirilemeyeceği anlamına gelir. Bu değerin yalnızca çalışma sayfası veya çalışma sayfasındaki nesneler korunduğunda anlamlı olduğunu unutmayın."
type: docs
url: /tr/net/aspose.cells.drawing/shape/islocked/
---
## Shape.IsLocked property

True, sayfa korunduğunda nesnenin değiştirilemeyeceği anlamına gelir. Bu değerin yalnızca çalışma sayfası veya içindeki nesneler korunduğunda anlamlı olduğunu unutmayın.

```csharp
public bool IsLocked { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyIsLockedDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Çalışma sayfasına bir şekil ekle
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 100, 100, 100);

            // Çalışma sayfasını koru
            worksheet.Protect(ProtectionType.All);

            // Şeklin kilitlenmesini/kilitlenmesinin kaldırılmasını gösterin
            Console.WriteLine("Original IsLocked state: " + shape.IsLocked);

            // Şeklin kilidini açın
            shape.IsLocked = false;
            Console.WriteLine("After unlocking, IsLocked state: " + shape.IsLocked);

            // Şekli kilitleyin
            shape.IsLocked = true;
            Console.WriteLine("After locking, IsLocked state: " + shape.IsLocked);
        }
    }
}
```

### Ayrıca Bakınız

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


