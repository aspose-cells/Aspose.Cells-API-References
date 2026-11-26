---
title: "CustomProperty.Value"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство CustomProperty. Возвращает или задает значение пользовательского свойства"
type: docs
url: /ru/net/aspose.cells.properties/customproperty/value/
---
## CustomProperty.Value property

Возвращает или задает значение пользовательского свойства.

```csharp
public string Value { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CustomPropertyPropertyValueDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавить пользовательское свойство с длинным строковым значением
            worksheet.CustomProperties.Add("VeryLongString", "This is a very long string value for testing custom properties");
            
            // Получить и отобразить значение пользовательского свойства
            string propertyValue = worksheet.CustomProperties["VeryLongString"].Value;
            Console.WriteLine("Custom Property Value: " + propertyValue);
            
            // Сохраните книгу
            workbook.Save("output.xlsx");
            
            // Перезагрузить книгу, чтобы проверить сохранность свойства
            Workbook loadedWorkbook = new Workbook("output.xlsx");
            Worksheet loadedWorksheet = loadedWorkbook.Worksheets[0];
            
            // Проверить, что значение осталось тем же после загрузки
            string loadedValue = loadedWorksheet.CustomProperties["VeryLongString"].Value;
            Console.WriteLine("Reloaded Custom Property Value: " + loadedValue);
        }
    }
}
```

### См. также

* class [CustomProperty](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


