---
title: "ThreeDFormat.Material"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ThreeDFormat. Представляет предустановленный материал, который комбинируется со свойствами освещения, чтобы придать фигуре окончательный вид и ощущение"
type: docs
url: /ru/net/aspose.cells.drawing/threedformat/material/
---
## ThreeDFormat.Material property

Представляет предустановленный материал, который комбинируется со свойствами освещения, чтобы создать окончательный внешний вид фигуры.

```csharp
public PresetMaterialType Material { get; set; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ThreeDFormatPropertyMaterialDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте фигуру для демонстрации 3D-форматирования
            Shape shape = worksheet.Shapes.AddShape(MsoDrawingType.TextBox, 10, 10, 200, 100, 0, 0);
            shape.Text = "3D Material Demo";
            
            // Получите доступ к ThreeDFormat фигуры
            ThreeDFormat threeDFormat = shape.ThreeDFormat;

            // Отобразить текущее значение материала
            Console.WriteLine("Current Material value: " + threeDFormat.Material);

            // Установите различные типы материалов и наблюдайте за эффектами
            threeDFormat.Material = PresetMaterialType.Metal;
            Console.WriteLine("Material changed to Metal");

            threeDFormat.Material = PresetMaterialType.Plastic;
            Console.WriteLine("Material changed to Plastic");

            threeDFormat.Material = PresetMaterialType.Matte;
            Console.WriteLine("Material changed to Matte");

            // Настройте другие 3D‑свойства, чтобы лучше увидеть эффект материала
            threeDFormat.ExtrusionHeight = 20;
            threeDFormat.ContourWidth = 2;
            threeDFormat.PresetCameraType = PresetCameraType.PerspectiveFront;
            threeDFormat.RotationX = 20;
            threeDFormat.RotationY = 30;

            // Сохранить книгу с 3D‑эффектами
            workbook.Save("ThreeDFormatMaterialDemo.xlsx");
        }
    }
}
```

### См. также

* enum [PresetMaterialType](../../presetmaterialtype/)
* class [ThreeDFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


