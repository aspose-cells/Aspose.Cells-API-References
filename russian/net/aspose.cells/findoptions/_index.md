---
title: "Класс FindOptions"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.FindOptions. Представляет параметры поиска"
type: docs
url: /ru/net/aspose.cells/findoptions/
---
## FindOptions class

Представляет параметры поиска.

```csharp
public class FindOptions
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [FindOptions](findoptions/)() | Конструктор по умолчанию. |

## Свойства

| Имя | Описание |
| --- | --- |
| [CaseSensitive](../../aspose.cells/findoptions/casesensitive/) { get; set; } | Указывает, чувствителен ли искомый строк к регистру. |
| [ConvertNumericData](../../aspose.cells/findoptions/convertnumericdata/) { get; set; } | Получает или задает значение, указывающее, следует ли преобразовывать значение искомой строки в числовые данные. |
| [IsCaseSensitive](../../aspose.cells/findoptions/iscasesensitive/) { get; set; } | (**Obsolete.**) Указывает, чувствителен ли искомый строк к регистру. |
| [IsRangeSet](../../aspose.cells/findoptions/israngeset/) { get; } | Указывает, установлен ли диапазон поиска. |
| [LookAtType](../../aspose.cells/findoptions/lookattype/) { get; set; } | Посмотреть тип. |
| [LookInType](../../aspose.cells/findoptions/lookintype/) { get; set; } | Посмотреть в типе. |
| [RegexKey](../../aspose.cells/findoptions/regexkey/) { get; set; } | Указывает, является ли искомый ключ регулярным выражением. Если true, искомый ключ будет восприниматься как регулярное выражение и анализироваться. В противном случае ключ будет анализироваться согласно правилам в MS Excel. |
| [SearchBackward](../../aspose.cells/findoptions/searchbackward/) { get; set; } | Искать ли в обратном направлении ячейки. |
| [SearchNext](../../aspose.cells/findoptions/searchnext/) { get; set; } | (**Obsolete.**) Порядок поиска. True: искать следующий. False: искать предыдущий. |
| [SearchOrderByRows](../../aspose.cells/findoptions/searchorderbyrows/) { get; set; } | Указывает, осуществляется ли порядок поиска по строкам или столбцам. |
| [Style](../../aspose.cells/findoptions/style/) { get; set; } | Формат для поиска. |
| [ValueTypeSensitive](../../aspose.cells/findoptions/valuetypesensitive/) { get; set; } | Указывает, должен ли тип значения искомой ячейки совпадать с типом искомого ключа. |

## Методы

| Имя | Описание |
| --- | --- |
| [GetRange](../../aspose.cells/findoptions/getrange/)() | Получает и задает диапазон поиска. |
| [SetRange](../../aspose.cells/findoptions/setrange/)(CellArea) | Задает диапазон поиска. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class FindOptionsDemo
    {
        public static void FindOptionsExample()
        {
            // Создайте объект рабочей книги
            Workbook workbook = new Workbook("FindOptionsExample_original.xlsx");

            // Получить коллекцию Cells
            Cells cells = workbook.Worksheets[0].Cells;

            // Создайте объект FindOptions
            FindOptions findOptions = new FindOptions();

            // Создайте область Cells
            CellArea ca = new CellArea();
            ca.StartRow = 0;
            ca.StartColumn = 0;
            ca.EndRow = 5;
            ca.EndColumn = 5;

            // Установите область ячеек для параметров поиска
            findOptions.SetRange(ca);

            // Установите свойства поиска
            findOptions.SearchBackward = false;
            findOptions.SearchOrderByRows = true;
            findOptions.LookInType = LookInType.Values;

            // Найти ячейку со значением 0
            Cell cell = cells.Find(0, null, findOptions);

            if (cell != null)
            {
                Console.WriteLine("Cell found at: " + cell.Name);
            }
            else
            {
                Console.WriteLine("Cell not found.");
            }
        }
    }
}
```

### См. также

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


