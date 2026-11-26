---
title: "TableStyleCollection.DefaultTableStyleName"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство TableStyleCollection. Получает и задает имя стиля по умолчанию для таблицы"
type: docs
url: /ru/net/aspose.cells.tables/tablestylecollection/defaulttablestylename/
---
## TableStyleCollection.DefaultTableStyleName property

Получает и задает имя стиля таблицы по умолчанию.

```csharp
public string DefaultTableStyleName { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class TableStyleCollectionPropertyDefaultTableStyleNameDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к коллекции стилей таблицы
            TableStyleCollection tableStyles = workbook.Worksheets.TableStyles;
            
            // Отобразить имя стиля таблицы по умолчанию
            Console.WriteLine("Default Table Style: " + tableStyles.DefaultTableStyleName);
            
            // Изменить стиль таблицы по умолчанию
            tableStyles.DefaultTableStyleName = "TableStyleMedium9";
            Console.WriteLine("New Default Table Style: " + tableStyles.DefaultTableStyleName);
            
            // Сохраните книгу
            workbook.Save("output.xlsx");
        }
    }
}
```

### См. также

* class [TableStyleCollection](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


