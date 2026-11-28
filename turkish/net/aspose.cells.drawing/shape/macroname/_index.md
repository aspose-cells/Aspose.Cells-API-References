---
title: "Shape.MacroName"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Shape özelliği. Makro adını alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells.drawing/shape/macroname/
---
## Shape.MacroName property

Makronun adını alır ve ayarlar.

```csharp
public string MacroName { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyMacroNameDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Çalışma sayfasına bir şekil ekle
            Shape shape = worksheet.Shapes.AddRectangle(1, 1, 100, 100, 0, 0);

            // Şekil için makro adını ayarla
            shape.MacroName = "DoWork()";

            // Çıktı onayı
            Console.WriteLine("Shape macro name set to: " + shape.MacroName);
        }
    }
}
```

### Ayrıca Bakınız

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


