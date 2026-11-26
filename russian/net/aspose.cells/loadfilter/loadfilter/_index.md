---
title: "LoadFilter.LoadFilter"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Конструктор LoadFilter. Создаёт один LoadFilter с параметрами фильтра по умолчанию LoadDataFilterOptions.All"
type: docs
url: /ru/net/aspose.cells/loadfilter/loadfilter/
---
## LoadFilter() {#constructor}

Создаёт один LoadFilter с параметрами фильтра по умолчанию LoadDataFilterOptions.All.

```csharp
public LoadFilter()
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class LoadFilterMethodCtorDemo
    {
        public static void Run()
        {
            // Создать новый LoadFilter с конструктором по умолчанию
            LoadFilter filter = new LoadFilter();
            
            // Создать параметры загрузки и назначить фильтр
            LoadOptions loadOptions = new LoadOptions();
            loadOptions.LoadFilter = filter;
            
            // Загрузить рабочую книгу с фильтром
            Workbook workbook = new Workbook("sample.xlsx", loadOptions);
            
            // Продемонстрировать использование, подсчитав листы
            Console.WriteLine("Number of worksheets loaded: " + workbook.Worksheets.Count);
            
            // Показать отфильтрованные данные ячеек (по умолчанию загружаются все ячейки)
            foreach (Worksheet sheet in workbook.Worksheets)
            {
                Console.WriteLine($"Worksheet '{sheet.Name}' has {sheet.Cells.Count} cells");
            }
        }
    }
}
```

### См. также

* class [LoadFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## LoadFilter(LoadDataFilterOptions) {#constructor_1}

Создаёт один LoadFilter с заданными параметрами фильтра.

```csharp
public LoadFilter(LoadDataFilterOptions opts)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| opts | LoadDataFilterOptions | опции фильтра по умолчанию |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class LoadFilterMethodCtorWithLoadDataFilterOptionsDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Подготовить данные для параметров метода (LoadDataFilterOptions)
            LoadDataFilterOptions filterOptions = LoadDataFilterOptions.CellData | LoadDataFilterOptions.Chart;

            try
            {
                // Вызвать метод #ctor с конкретными типами параметров
                LoadFilter loadFilter = new LoadFilter(filterOptions);

                // Обработать или отобразить результат
                Console.WriteLine("LoadFilter created successfully with LoadDataFilterOptions: " + filterOptions);

                // Показать эффект вызова метода
                Console.WriteLine("LoadDataFilterOptions set to: " + loadFilter.LoadDataFilterOptions);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error creating LoadFilter: {ex.Message}");
            }

            // Сохранить результат
            workbook.Save("LoadFilterCtorWithLoadDataFilterOptionsDemo.xlsx");
        }
    }
}
```

### См. также

* enum [LoadDataFilterOptions](../../loaddatafilteroptions/)
* class [LoadFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


