---
title: "WorkbookDesigner.SetJsonDataSource"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод WorkbookDesigner. Устанавливает значение строки json в качестве источника данных для smart markers"
type: docs
url: /ru/net/aspose.cells/workbookdesigner/setjsondatasource/
---
## WorkbookDesigner.SetJsonDataSource method

Устанавливает значение строки JSON в качестве источника данных смарт‑маркировок.

```csharp
public void SetJsonDataSource(string name, string json)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| name | String | Имя таблицы. Если значение JSON представляет объект, оно может быть null. |
| json | String | Значение строки Json. |

### Примеры

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookDesignerMethodSetJsonDataSourceWithStringStringDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавьте пример маркера в ячейку A1
            worksheet.Cells["A1"].PutValue("&=$DataSource.Name");
            
            // Создать дизайнер рабочей книги
            WorkbookDesigner designer = new WorkbookDesigner();
            designer.Workbook = workbook;
            
            // Пример JSON-данных
            string jsonData = "{\"Name\":\"John Doe\",\"Age\":30,\"City\":\"New York\"}";
            
            // Установите источник данных JSON
            designer.SetJsonDataSource("DataSource", jsonData);
            
            // Обработайте маркеры
            designer.Process();
            
            // Сохраните книгу
            workbook.Save("output.xlsx");
        }
    }
}
```

### См. также

* class [WorkbookDesigner](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


