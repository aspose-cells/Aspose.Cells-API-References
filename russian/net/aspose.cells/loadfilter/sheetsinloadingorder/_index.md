---
title: "LoadFilter.SheetsInLoadingOrder"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство LoadFilter. Указывает индексы листов и порядок их загрузки. По умолчанию null, что означает загрузку всех листов в порядке по умолчанию в файле шаблона. Если не null и некоторый индекс листа отсутствует в возвращаемом массиве, то лист не будет загружен."
type: docs
url: /ru/net/aspose.cells/loadfilter/sheetsinloadingorder/
---
## LoadFilter.SheetsInLoadingOrder property

Указывает листы (индексы) и порядок их загрузки. По умолчанию null, что означает загрузку всех листов в порядке по умолчанию из файла шаблона. Если не null и индекс некоторого листа отсутствует в возвращённом массиве, лист не будет загружен.

```csharp
public virtual int[] SheetsInLoadingOrder { get; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class LoadFilterPropertySheetsInLoadingOrderDemo
    {
        public static void Run()
        {
            // Создайте новую книгу с несколькими листами.
            Workbook workbook = new Workbook();
            workbook.Worksheets.Add("Sheet2");
            workbook.Worksheets.Add("Sheet3");
            
            // Создать пользовательский фильтр загрузки
            LoadFilter loadFilter = new LoadFilter(LoadDataFilterOptions.All);
            
            // Отобразить значение по умолчанию SheetsInLoadingOrder (null означает загрузку всех листов)
            Console.WriteLine("Initial SheetsInLoadingOrder is null: " + (loadFilter.SheetsInLoadingOrder == null));
            
            // Создать файл шаблона для демонстрации загрузки с пользовательским порядком листов
            workbook.Save("Template.xlsx");
            
            // Создать параметры загрузки с нашим пользовательским фильтром
            LoadOptions loadOptions = new LoadOptions();
            loadOptions.LoadFilter = loadFilter;
            
            // Загрузить книгу с настройками по умолчанию (все листы)
            Workbook loadedWorkbook1 = new Workbook("Template.xlsx", loadOptions);
            Console.WriteLine("Sheets loaded with default filter: " + loadedWorkbook1.Worksheets.Count);
            
            // Создать новый фильтр с определённым порядком загрузки листов
            LoadFilter orderedFilter = new LoadFilter(LoadDataFilterOptions.All)
            {
                // Примечание: SheetsInLoadingOrder доступен только для чтения, поэтому нам нужно создать новый фильтр
                // с желаемым порядком в конструкторе или другими способами
                // Это демонстрирует ограничение свойства, которое доступно только для чтения
            };
            
            // Поскольку SheetsInLoadingOrder доступен только для чтения, нам придётся создать подкласс LoadFilter
            // для демонстрации пользовательского порядка загрузки листов
            CustomLoadFilter customFilter = new CustomLoadFilter(new int[] { 2, 0 }); // Load Sheet3 first, then Sheet1
            
            LoadOptions customLoadOptions = new LoadOptions();
            customLoadOptions.LoadFilter = customFilter;
            
            // Загрузить книгу с пользовательским порядком листов
            Workbook loadedWorkbook2 = new Workbook("Template.xlsx", customLoadOptions);
            Console.WriteLine("Sheets loaded with custom filter: " + loadedWorkbook2.Worksheets.Count);
            Console.WriteLine("First sheet in custom order: " + loadedWorkbook2.Worksheets[0].Name);
        }
    }

    // Пользовательская реализация LoadFilter для демонстрации функциональности SheetsInLoadingOrder
    public class CustomLoadFilter : LoadFilter
    {
        private readonly int[] _sheetsOrder;
        
        public CustomLoadFilter(int[] sheetsOrder) : base(LoadDataFilterOptions.All)
        {
            _sheetsOrder = sheetsOrder;
        }
        
        public override int[] SheetsInLoadingOrder => _sheetsOrder;
    }
}
```

### См. также

* class [LoadFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


