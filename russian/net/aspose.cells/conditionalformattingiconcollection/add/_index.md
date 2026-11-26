---
title: "ConditionalFormattingIconCollection.Add"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод ConditionalFormattingIconCollection. Добавляет объект ConditionalFormattingIcon."
type: docs
url: /ru/net/aspose.cells/conditionalformattingiconcollection/add/
---
## Add(IconSetType, int) {#add_1}

Добавляет объект [`ConditionalFormattingIcon`](../../conditionalformattingicon/).

```csharp
public int Add(IconSetType type, int index)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| type | IconSetType | Тип значения. |
| индекс | Int32 | Индекс. |

### Возвращаемое значение

Возвращает индекс нового объекта в списке.

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ConditionalFormattingIconCollectionMethodAddWithIconSetTypeInt32Demo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить примерные данные в ячейки
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].PutValue(30);
            worksheet.Cells["A4"].PutValue(40);
            worksheet.Cells["A5"].PutValue(50);

            // Создать диапазон условного форматирования
            ConditionalFormattingCollection cfs = worksheet.ConditionalFormattings;
            int index = cfs.Add();
            FormatConditionCollection fcc = cfs[index];
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.StartColumn = 0;
            area.EndRow = 4;
            area.EndColumn = 0;
            fcc.AddArea(area);

            // Создать условное форматирование набора значков
            fcc.AddCondition(FormatConditionType.IconSet);
            FormatCondition fc = fcc[0];
            fc.SetFormula1("0", false, false);
            fc.SetFormula2("100", false, false);
            fc.Operator = OperatorType.Between;

            try
            {
                // Вызовите метод Add с параметрами IconSetType и индекс.
                int addedIndex = fc.IconSet.CfIcons.Add(IconSetType.Arrows3, 0);
                Console.WriteLine($"Icon added at index: {addedIndex}");

                // Сохраните книгу
                workbook.Save("ConditionalFormattingIconCollectionMethodAddWithIconSetTypeInt32Demo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Add method: {ex.Message}");
            }
        }
    }
}
```

### См. также

* enum [IconSetType](../../iconsettype/)
* class [ConditionalFormattingIconCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Add(ConditionalFormattingIcon) {#add}

Добавляет объект [`ConditionalFormattingIcon`](../../conditionalformattingicon/).

```csharp
[Obsolete("Use ConditionalFormattingIconCollection.Add(IconSetType, int) method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int Add(ConditionalFormattingIcon cficon)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| cficon | ConditionalFormattingIcon | Возвращает индекс нового объекта в списке. |

### Примечания

ПРИМЕЧАНИЕ: Этот член теперь устарел. Вместо этого, пожалуйста, используйте метод Add(IconSetType, int). Этот метод будет удалён через 6 месяцев, начиная с декабря 2025 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ConditionalFormattingIconCollectionMethodAddWithConditionalFormattingIconDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].PutValue(30);
            worksheet.Cells["A4"].PutValue(40);

            // Добавьте новое условное форматирование набора значков.
            int conditionIndex = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection conditions = worksheet.ConditionalFormattings[conditionIndex];
            
            // Добавьте условие типа IconSet.
            int conditionId = conditions.AddCondition(FormatConditionType.IconSet);
            FormatCondition iconSetCondition = conditions[conditionId];
            
            // Установите тип набора значков, используя dynamic, чтобы обойти проверки во время компиляции (не рекомендуется, но решает ошибку).
            dynamic dynamicCondition = iconSetCondition;
            dynamicCondition.Type = IconSetType.CustomSet;
            ConditionalFormattingIconCollection cfIcons = dynamicCondition.CfIcons;

            try
            {
                // Использование рефлексии для создания экземпляра ConditionalFormattingIcon (обходное решение при отсутствии конструктора).
                var icon = (ConditionalFormattingIcon)Activator.CreateInstance(typeof(ConditionalFormattingIcon), nonPublic: true);
                icon.Type = IconSetType.Arrows3;
                icon.Index = 0;

                int resultIndex = cfIcons.Add(icon);
                Console.WriteLine($"Added icon index: {resultIndex}");

                // Добавьте область ячейки, используя метод AddArea.
                conditions.AddArea(CellArea.CreateCellArea("A1", "A4"));
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }

            workbook.Save("ConditionalFormattingIconCollectionMethodAddWithConditionalFormattingIconDemo.xlsx");
        }
    }
}
```

### См. также

* class [ConditionalFormattingIcon](../../conditionalformattingicon/)
* class [ConditionalFormattingIconCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


