---
title: "DataModel.Tables"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство DataModel. Возвращает все таблицы в модели данных"
type: docs
url: /ru/net/aspose.cells.datamodels/datamodel/tables/
---
## DataModel.Tables property

Получает все таблицы в модели данных.

```csharp
public DataModelTableCollection Tables { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.DataModels;

namespace AsposeCellsExamples
{
    public class DataModelPropertyTablesDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook wb = new Workbook();
            
            // Получить доступ к модели данных
            DataModel dataModel = wb.DataModel;
            
            // Получить коллекцию таблиц и показать количество
            Console.WriteLine($"Tables count in new workbook: {dataModel.Tables.Count}");
            
            // Загрузить примерную рабочую книгу с моделью данных
            string sourceFile = "example.xlsb";
            if (System.IO.File.Exists(sourceFile))
            {
                Workbook sampleWorkbook = new Workbook(sourceFile);
                DataModel sampleDataModel = sampleWorkbook.DataModel;
                
                // Получить доступ к коллекции таблиц
                DataModelTableCollection tables = sampleDataModel.Tables;
                Console.WriteLine($"Tables count in sample file: {tables.Count}");
                
                // Перебрать таблицы
                foreach (DataModelTable table in tables)
                {
                    Console.WriteLine($"Table name: {table.Name}");
                }
            }
            else
            {
                Console.WriteLine($"Sample file '{sourceFile}' not found. Create an Excel file with data model to see tables information.");
            }
        }
    }
}
```

### См. также

* class [DataModelTableCollection](../../datamodeltablecollection/)
* class [DataModel](../)
* namespace [Aspose.Cells.DataModels](../../../aspose.cells.datamodels/)
* assembly [Aspose.Cells](../../../)


