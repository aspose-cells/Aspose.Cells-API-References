---
title: "Класс ConditionalFormattingValueCollection"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.ConditionalFormattingValueCollection. Описывает коллекцию CFValueObject. Используется только для наборов значков"
type: docs
url: /ru/net/aspose.cells/conditionalformattingvaluecollection/
---
## ConditionalFormattingValueCollection class

Описывает коллекцию CFValueObject. Используется только для наборов иконок.

```csharp
public class ConditionalFormattingValueCollection : CollectionBase<ConditionalFormattingValue>
```

## Свойства

| Имя | Описание |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [Item](../../aspose.cells/conditionalformattingvaluecollection/item/) { get; } | Получите элемент CFValueObject по указанному индексу. |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |

## Методы

| Имя | Описание |
| --- | --- |
| [Add](../../aspose.cells/conditionalformattingvaluecollection/add/)(FormatConditionValueType, string) | Добавляет объект [`ConditionalFormattingValue`](../conditionalformattingvalue/). |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(ConditionalFormattingValue) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(ConditionalFormattingValue, IComparer&lt;ConditionalFormattingValue&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(int, int, ConditionalFormattingValue, IComparer&lt;ConditionalFormattingValue&gt;) |  |
| [Clear](../../aspose.cells/collectionbase-1/clear/)() |  |
| [Contains](../../aspose.cells/collectionbase-1/contains/)(ConditionalFormattingValue) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(ConditionalFormattingValue[]) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(ConditionalFormattingValue[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(int, ConditionalFormattingValue[], int, int) |  |
| [Exists](../../aspose.cells/collectionbase-1/exists/)(Predicate&lt;ConditionalFormattingValue&gt;) |  |
| [Find](../../aspose.cells/collectionbase-1/find/)(Predicate&lt;ConditionalFormattingValue&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase-1/findall/)(Predicate&lt;ConditionalFormattingValue&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(Predicate&lt;ConditionalFormattingValue&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, Predicate&lt;ConditionalFormattingValue&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, int, Predicate&lt;ConditionalFormattingValue&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase-1/findlast/)(Predicate&lt;ConditionalFormattingValue&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(Predicate&lt;ConditionalFormattingValue&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, Predicate&lt;ConditionalFormattingValue&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, int, Predicate&lt;ConditionalFormattingValue&gt;) |  |
| [GetEnumerator](../../aspose.cells/collectionbase-1/getenumerator/)() |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(ConditionalFormattingValue) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(ConditionalFormattingValue, int) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(ConditionalFormattingValue, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(ConditionalFormattingValue) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(ConditionalFormattingValue, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(ConditionalFormattingValue, int, int) |  |
| [RemoveAt](../../aspose.cells/collectionbase-1/removeat/)(int) |  |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ConditionalFormattingValueCollectionDemo
    {
        public static void ConditionalFormattingValueCollectionExample()
        {
            // Создание объекта Workbook
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Добавляет пустое условное форматирование
            int index = sheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = sheet.ConditionalFormattings[index];

            // Устанавливает диапазон условного форматирования
            CellArea ca = new CellArea
            {
                StartRow = 0,
                EndRow = 2,
                StartColumn = 0,
                EndColumn = 0
            };
            fcs.AddArea(ca);

            // Добавляет условие
            int conditionIndex = fcs.AddCondition(FormatConditionType.IconSet);
            FormatCondition cond = fcs[conditionIndex];

            // Получить набор значков
            IconSet iconSet = cond.IconSet;

            // Установить тип значка
            iconSet.Type = IconSetType.Arrows3;

            // Получите экземпляр CFValueObjects
            ConditionalFormattingValueCollection cfvos = iconSet.Cfvos;

            // Добавьте новый ConditionalFormattingValue в коллекцию
            int cfvIndex = cfvos.Add(FormatConditionValueType.Number, "50");

            // Получите доступ к только что добавленному ConditionalFormattingValue
            ConditionalFormattingValue cfv = cfvos[cfvIndex];

            // Измените свойства ConditionalFormattingValue
            cfv.Value = 75;
            cfv.Type = FormatConditionValueType.Percent;
            cfv.IsGTE = true;

            // Задать значения ячеек
            sheet.Cells["A1"].PutValue(10);
            sheet.Cells["A2"].PutValue(120);
            sheet.Cells["A3"].PutValue(260);

            // Сохранение файла Excel
            workbook.Save("ConditionalFormattingValueCollectionExample.xlsx");
            workbook.Save("ConditionalFormattingValueCollectionExample.pdf");
        }
    }
}
```

### См. также

* class [CollectionBase&lt;T&gt;](../collectionbase-1/)
* class [ConditionalFormattingValue](../conditionalformattingvalue/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


