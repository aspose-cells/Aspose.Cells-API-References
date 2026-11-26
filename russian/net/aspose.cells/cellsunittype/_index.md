---
title: "Перечисление CellsUnitType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Перечисление Aspose.Cells.CellsUnitType. Указывает единицу измерения"
type: docs
url: /ru/net/aspose.cells/cellsunittype/
---
## CellsUnitType enumeration

Указывает единицу измерения.

```csharp
public enum CellsUnitType
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| Pixel | `1` | Измерение в пикселях. |
| Point | `2` | Измерение в пунктах. Один пункт равен 1/72 дюйма. |
| Inch | `4` | Измерение в дюймах. |
| Cm | `6` | Измерение в сантиметрах. |
| Character | `7` | В единицах символов. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsClassCellsUnitTypeDemo
    {
        public static void Run()
        {
            // Создать новую книгу для демонстрации
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Продемонстрировать использование разных значений перечисления CellsUnitType
                Console.WriteLine("Available CellsUnitType values:");

                // Отобразить все значения перечисления
                Console.WriteLine("Pixel: " + CellsUnitType.Pixel);
                Console.WriteLine("Point: " + CellsUnitType.Point);
                Console.WriteLine("Inch: " + CellsUnitType.Inch);
                Console.WriteLine("Cm: " + CellsUnitType.Cm);
                Console.WriteLine("Character: " + CellsUnitType.Character);

                // Пример использования: установить ширину столбца, используя разные единицы
                worksheet.Cells.SetColumnWidthPixel(0, 100); // Using Pixel unit
                worksheet.Cells.SetColumnWidthInch(1, 2.0);  // Using Inch unit

                // Сохраните рабочую книгу, чтобы продемонстрировать полный процесс
                workbook.Save("CellsUnitTypeDemo.xlsx");
                Console.WriteLine("Workbook saved successfully with different unit types applied.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with CellsUnitType: {ex.Message}");
            }
        }
    }
}
```

### См. также

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


