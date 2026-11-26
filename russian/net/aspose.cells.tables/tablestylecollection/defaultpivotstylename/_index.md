---
title: "TableStyleCollection.DefaultPivotStyleName"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство TableStyleCollection. Получает и задает имя стиля по умолчанию для сводной таблицы"
type: docs
url: /ru/net/aspose.cells.tables/tablestylecollection/defaultpivotstylename/
---
## TableStyleCollection.DefaultPivotStyleName property

Получает и задает имя стиля по умолчанию сводной таблицы.

```csharp
public string DefaultPivotStyleName { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class TableStyleCollectionPropertyDefaultPivotStyleNameDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к коллекции стилей таблицы
            TableStyleCollection tableStyles = workbook.Worksheets.TableStyles;
            
            // Отобразить имя стиля сводной таблицы по умолчанию
            Console.WriteLine("Default Pivot Style: " + tableStyles.DefaultPivotStyleName);
            
            // Изменить стиль сводной таблицы по умолчанию
            tableStyles.DefaultPivotStyleName = "PivotStyleDark2";
            
            // Проверьте изменение
            Console.WriteLine("Updated Default Pivot Style: " + tableStyles.DefaultPivotStyleName);
            
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


