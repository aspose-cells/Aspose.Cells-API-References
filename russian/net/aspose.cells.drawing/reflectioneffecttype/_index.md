---
title: "Перечисление ReflectionEffectType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Перечисление Aspose.Cells.Drawing.ReflectionEffectType. Представляет тип эффекта отражения"
type: docs
url: /ru/net/aspose.cells.drawing/reflectioneffecttype/
---
## ReflectionEffectType enumeration

Представляет тип эффекта отражения.

```csharp
public enum ReflectionEffectType
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| None | `0` | Без эффекта отражения. |
| Custom | `1` | Пользовательский эффект отражения. |
| TightReflectionTouching | `2` | Плотное отражение, касающееся. |
| HalfReflectionTouching | `3` | Отражение наполовину, касающееся. |
| FullReflectionTouching | `4` | Полное отражение, касающееся. |
| TightReflection4PtOffset | `5` | Плотное отражение, смещение 4 пт. |
| HalfReflection4PtOffset | `6` | Отражение наполовину, смещение 4 пт. |
| FullReflection4PtOffset | `7` | Полное отражение, смещение 4 пт. |
| TightReflection8PtOffset | `8` | Плотное отражение, смещение 8 пт. |
| HalfReflection8PtOffset | `9` | Отражение наполовину, смещение 8 пт. |
| FullReflection8PtOffset | `10` | Полное отражение, смещение 8 пт. |

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class DrawingClassReflectionEffectTypeDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавить прямоугольную фигуру
            Shape rectangle = worksheet.Shapes.AddRectangle(0, 0, 0, 0, 100, 100);
            
            // Получить эффект отражения
            ReflectionEffect reflection = rectangle.Reflection;
            
            // Установить свойства отражения
            reflection.Type = ReflectionEffectType.HalfReflectionTouching;
            reflection.Transparency = 0.5;
            reflection.Size = 55;
            reflection.Blur = 0.5;
            reflection.Distance = 0;
            
            // Сохраните книгу
            workbook.Save("DrawingClassReflectionEffectTypeDemo.xlsx");
            
            Console.WriteLine("Reflection effect demo completed successfully.");
        }
    }
}
```

### См. также

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


