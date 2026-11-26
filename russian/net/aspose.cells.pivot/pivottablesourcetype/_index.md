---
title: "Перечисление PivotTableSourceType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Перечисление Aspose.Cells.Pivot.PivotTableSourceType. Представляет тип источника данных сводной таблицы"
type: docs
url: /ru/net/aspose.cells.pivot/pivottablesourcetype/
---
## PivotTableSourceType enumeration

Представляет тип источника данных сводной таблицы.

```csharp
public enum PivotTableSourceType : byte
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| Sheet | `1` | Указывает, что исходные данные представляют собой диапазон. |
| External | `2` | Указывает, что используются внешние исходные данные. |
| Consolidation | `4` | Указывает, что в качестве исходных данных используются несколько диапазонов консолидации. |
| Scenario | `8` | Исходные данные заполняются из временной внутренней структуры. |
| Unknown | `9` | Неизвестный источник данных. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotClassPivotTableSourceTypeDemo
    {
        public static void Run()
        {
            // Создать новую книгу для демонстрации
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Добавить примерные данные в лист
                worksheet.Cells["A1"].PutValue("Category");
                worksheet.Cells["B1"].PutValue("Value");
                worksheet.Cells["A2"].PutValue("A");
                worksheet.Cells["B2"].PutValue(10);
                worksheet.Cells["A3"].PutValue("B");
                worksheet.Cells["B3"].PutValue(20);
                worksheet.Cells["A4"].PutValue("C");
                worksheet.Cells["B4"].PutValue(30);

                // Создать коллекцию сводных таблиц
                PivotTableCollection pivotTables = worksheet.PivotTables;

                // Добавить сводную таблицу, используя лист в качестве типа источника
                int index = pivotTables.Add("=A1:B4", "D3", "SheetPivotTable");
                PivotTable pivotTable = pivotTables[index];

                // Отобразить тип источника
                Console.WriteLine("Pivot Table Source Type: " + pivotTable.SourceType);

                // Продемонстрировать различные типы источников
                Console.WriteLine("Available PivotTableSourceType values:");
                Console.WriteLine("Sheet: " + PivotTableSourceType.Sheet);
                Console.WriteLine("External: " + PivotTableSourceType.External);
                Console.WriteLine("Consolidation: " + PivotTableSourceType.Consolidation);
                Console.WriteLine("Scenario: " + PivotTableSourceType.Scenario);
                Console.WriteLine("Unknown: " + PivotTableSourceType.Unknown);

                // Сохраните книгу
                workbook.Save("PivotTableSourceTypeDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with PivotTableSourceType: {ex.Message}");
            }
        }
    }
}
```

### См. также

* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)


