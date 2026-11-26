---
title: "Перечисление AutoFillType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Перечисление Aspose.Cells.AutoFillType. Представляет тип автозаполнения"
type: docs
url: /ru/net/aspose.cells/autofilltype/
---
## AutoFillType enumeration

Представляет тип автозаполнения.

```csharp
public enum AutoFillType
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| Copy | `1` | Копирует значение и формат исходной области в целевую область |
| Default | `0` | Автоматически заполняет целевую область значением и форматом. |
| Formats | `3` | Копирует только формат исходной области в целевую область. |
| Series | `2` | Расширяет значение из исходной области в целевую область в виде серии и копирует формат в целевую область. |
| Values | `4` | Копирует только значение исходной области в целевую область. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class AutoFillTypeDemo
    {
        public static void AutoFillTypeExample()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Создайте диапазон (A1:A10) и заполните его некоторыми значениями
            Aspose.Cells.Range sourceRange = worksheet.Cells.CreateRange("A1:A10");
            for (int i = 0; i < 10; i++)
            {
                sourceRange[i, 0].PutValue(i + 1);
            }

            // Создайте целевой диапазон (B1:B10)
            Aspose.Cells.Range targetRange = worksheet.Cells.CreateRange("B1:B10");

            //Ошибка типа серии, заявка создана
            // Используйте метод AutoFill с AutoFillType.Series для заполнения целевого диапазона
            //sourceRange.AutoFill(targetRange, AutoFillType.Series);

            // Используйте метод AutoFill с AutoFillType.Copy для заполнения целевого диапазона
            sourceRange.AutoFill(targetRange, AutoFillType.Copy);
            // Сохраните книгу
            workbook.Save("AutoFillTypeExample.xlsx");
            workbook.Save("AutoFillTypeExample.pdf");
        }
    }

}
```

### См. также

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


