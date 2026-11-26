---
title: "Класс LoadFilter"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.LoadFilter. Представляет фильтр, который предоставляет параметры загрузки данных при загрузке книги из шаблона"
type: docs
url: /ru/net/aspose.cells/loadfilter/
---
## LoadFilter class

Представляет фильтр, который предоставляет параметры загрузки данных при загрузке рабочей книги из шаблона.

```csharp
public class LoadFilter
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [LoadFilter](loadfilter/#constructor)() | Создаёт один LoadFilter с параметрами фильтра по умолчанию LoadDataFilterOptions.All. |
| [LoadFilter](loadfilter/#constructor_1)(LoadDataFilterOptions) | Создаёт один LoadFilter с заданными параметрами фильтра. |

## Свойства

| Имя | Описание |
| --- | --- |
| [LoadDataFilterOptions](../../aspose.cells/loadfilter/loaddatafilteroptions/) { get; set; } | Параметры фильтра, указывающие, какие данные следует загрузить. |
| virtual [SheetsInLoadingOrder](../../aspose.cells/loadfilter/sheetsinloadingorder/) { get; } | Указывает листы (индексы) и порядок их загрузки. По умолчанию null, что означает загрузку всех листов в порядке по умолчанию из файла шаблона. Если не null и индекс некоторого листа отсутствует в возвращённом массиве, лист не будет загружен. |

## Методы

| Имя | Описание |
| --- | --- |
| virtual [StartSheet](../../aspose.cells/loadfilter/startsheet/)(Worksheet) | Подготавливает параметры фильтра перед загрузкой указанного листа. Реализация LoadFilter пользователем может изменить LoadDataFilterOptions здесь, указывая, как загружать данные для этого листа. |

### Примечания

Пользователь может указать параметры фильтра или реализовать собственный LoadFilter, чтобы задать способ загрузки данных.

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class LoadFilterDemo
    {
        public static void LoadFilterExample()
        {
            // Создайте LoadOptions и задайте LoadFilter
            LoadOptions opts = new LoadOptions();
            opts.LoadFilter = new CustomLoadFilter();

            // Загрузите книгу с указанными LoadOptions
            Workbook wb = new Workbook("LoadFilterExample_original.xlsx", opts);

            // Сохраните книгу, чтобы увидеть эффект LoadFilter
            wb.Save("LoadFilterExample.xlsx");
        }

        // Пользовательская реализация LoadFilter
        public class CustomLoadFilter : LoadFilter
        {
            public override void StartSheet(Worksheet sheet)
            {
                if (sheet.Name == "Sheet1")
                {
                    LoadDataFilterOptions = LoadDataFilterOptions.All;
                }
                else
                {
                    LoadDataFilterOptions = LoadDataFilterOptions.Structure;
                }
            }
        }
    }
}
```

### См. также

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


