---
title: "LoadFilter.StartSheet"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод LoadFilter. Подготавливает параметры фильтра перед загрузкой указанного листа. Реализация LoadFilter пользователем может изменить LoadDataFilterOptions здесь, чтобы указать, как загружать данные для этого листа"
type: docs
url: /ru/net/aspose.cells/loadfilter/startsheet/
---
## LoadFilter.StartSheet method

Подготавливает параметры фильтра перед загрузкой указанного листа. Реализация LoadFilter пользователем может изменить LoadDataFilterOptions здесь, указывая, как загружать данные для этого листа.

```csharp
public virtual void StartSheet(Worksheet sheet)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| лист | Worksheet | Лист, который будет загружен. Здесь можно использовать только несколько свойств данного объекта листа, поскольку большинство данных и свойств ещё не загружены. Доступные свойства: Name, Index, VisibilityType |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class LoadFilterMethodStartSheetWithWorksheetDemo
    {
        // Создать пользовательский класс фильтра загрузки, наследующий LoadFilter
        class CustomLoadFilter : LoadFilter
        {
            public override void StartSheet(Worksheet sheet)
            {
                Console.WriteLine($"Processing sheet: {sheet.Name}");
                // Здесь можно добавить пользовательскую логику для обработки конкретных листов
            }
        }

        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Name = "TestSheet";

            // Создать экземпляр нашего пользовательского фильтра загрузки
            CustomLoadFilter loadFilter = new CustomLoadFilter();

            try
            {
                // Вызвать метод StartSheet с параметром worksheet
                loadFilter.StartSheet(worksheet);
                
                Console.WriteLine("StartSheet method executed successfully");
                
                // Добавьте некоторые данные, чтобы продемонстрировать доступность листа
                worksheet.Cells["A1"].PutValue("StartSheet Demo");
                worksheet.Cells["A2"].PutValue(DateTime.Now.ToString());
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing StartSheet method: {ex.Message}");
            }
            
            // Сохранить результат
            workbook.Save("LoadFilterStartSheetDemo.xlsx");
        }
    }
}
```

### См. также

* class [Worksheet](../../worksheet/)
* class [LoadFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


