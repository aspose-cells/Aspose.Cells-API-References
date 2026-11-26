---
title: "ConditionalFormattingCollection.RemoveArea"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод ConditionalFormattingCollection. Удалить все условное форматирование в диапазоне"
type: docs
url: /ru/net/aspose.cells/conditionalformattingcollection/removearea/
---
## ConditionalFormattingCollection.RemoveArea method

Удалить всё условное форматирование в диапазоне.

```csharp
public void RemoveArea(int startRow, int startColumn, int totalRows, int totalColumns)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| startRow | Int32 | Начальная строка диапазона. |
| startColumn | Int32 | Начальный столбец диапазона. |
| totalRows | Int32 | Количество строк в диапазоне. |
| totalColumns | Int32 | Количество столбцов в диапазоне. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ConditionalFormattingCollectionMethodRemoveAreaWithInt32Int32Int32Int32Demo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Получить коллекцию условного форматирования
            ConditionalFormattingCollection cfc = worksheet.ConditionalFormattings;

            // Добавить несколько правил условного форматирования
            int index = cfc.Add();
            FormatConditionCollection fcc = cfc[index];
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.StartColumn = 0;
            area.EndRow = 5;
            area.EndColumn = 5;
            fcc.AddArea(area);

            try
            {
                // Вызвать RemoveArea с параметрами (Int32, Int32, Int32, Int32)
                cfc.RemoveArea(0, 0, 3, 3);

                Console.WriteLine("Conditional formatting removed from area (0,0,3,3)");
                
                // Проверьте эффект, проверив количество (это будет 0, если всё форматирование было удалено)
                Console.WriteLine($"Remaining conditional formatting areas: {fcc.RangeCount}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing RemoveArea method: {ex.Message}");
            }
            
            // Сохранить результат
            workbook.Save("RemoveAreaWithInt32Demo.xlsx");
        }
    }
}
```

### См. также

* class [ConditionalFormattingCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


