---
title: "Перечисление ShapePathPointValueType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Перечисление Aspose.Cells.Drawing.ShapePathPointValueType. Указывает тип значения объекта ShapePathPoint"
type: docs
url: /ru/net/aspose.cells.drawing/shapepathpointvaluetype/
---
## ShapePathPointValueType enumeration

Указывает тип значения объекта [`ShapePathPoint`](../shapepathpoint/)

```csharp
public enum ShapePathPointValueType
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| Position | `0` | Указывает, что тип объекта — координаты местоположения. Объект [`ShapePathPoint`](../shapepathpoint/) хранит координатные значения точки. |
| Angle | `1` | Указывает, что тип объекта — маркеры углов. Объект [`ShapePathPoint`](../shapepathpoint/) хранит начальный и конечный углы дуги. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class DrawingClassShapePathPointValueTypeDemo
    {
        public static void Run()
        {
            // Создать новую книгу для демонстрации
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Продемонстрировать значения перечисления ShapePathPointValueType
                ShapePathPointValueType positionType = ShapePathPointValueType.Position;
                ShapePathPointValueType angleType = ShapePathPointValueType.Angle;

                // Отобразить значения перечисления
                Console.WriteLine($"Position type value: {(int)positionType}");
                Console.WriteLine($"Angle type value: {(int)angleType}");

                // Проверьте, что значения перечисления соответствуют ожидаемым константам
                Console.WriteLine($"Position equals 0: {positionType == ShapePathPointValueType.Position}");
                Console.WriteLine($"Angle equals 1: {angleType == ShapePathPointValueType.Angle}");

                Console.WriteLine("ShapePathPointValueType enum demonstrated successfully");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with ShapePathPointValueType: {ex.Message}");
            }
        }
    }
}
```

### См. также

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


