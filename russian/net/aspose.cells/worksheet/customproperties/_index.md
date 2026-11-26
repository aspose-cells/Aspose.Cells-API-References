---
title: "Worksheet.CustomProperties"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство листа. Возвращает объект, представляющий идентификационную информацию, связанную с листом."
type: docs
url: /ru/net/aspose.cells/worksheet/customproperties/
---
## Worksheet.CustomProperties property

Получает объект, представляющий информацию об идентификаторе, связанную с рабочим листом.

```csharp
public CustomPropertyCollection CustomProperties { get; }
```

### Примечания

Worksheet.CustomProperties предоставляет предпочтительный механизм для хранения произвольных данных. Он поддерживает устаревшие сторонние компоненты документов, а также ситуации, требующие строгой работы с бинарными частями.

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyCustomPropertiesDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавить пользовательские свойства к листу
            worksheet.CustomProperties.Add("Property1", "Value1");
            worksheet.CustomProperties.Add("Property2", "12345");
            worksheet.CustomProperties.Add("Property3", DateTime.Now.ToString());
            
            // Отобразить количество пользовательских свойств
            Console.WriteLine("Custom Properties Count: " + worksheet.CustomProperties.Count);
            
            // Получить доступ и отобразить значения свойств
            foreach (var prop in worksheet.CustomProperties)
            {
                Console.WriteLine($"Name: {prop.Name}, Value: {prop.Value}");
            }
            
            // Сохраните книгу
            workbook.Save("WorksheetCustomPropertiesDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### См. также

* class [CustomPropertyCollection](../../../aspose.cells.properties/custompropertycollection/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


