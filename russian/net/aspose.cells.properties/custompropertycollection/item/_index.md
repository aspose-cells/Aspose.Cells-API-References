---
title: "CustomPropertyCollection.Item"
second_title: "Справочник API Aspose.Cells для .NET"
description: "CustomPropertyCollection свойство. Получает пользовательское свойство по указанному индексу"
type: docs
url: /ru/net/aspose.cells.properties/custompropertycollection/item/
---
## CustomPropertyCollection indexer (1 of 2)

Получает пользовательское свойство по указанному индексу.

```csharp
public CustomProperty this[int index] { get; }
```

| Параметр | Описание |
| --- | --- |
| индекс | Индекс. |

### Возвращаемое значение

Пользовательское свойство

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Properties;

namespace AsposeCellsExamples
{
    public class CustomPropertyCollectionPropertyItemDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            CustomPropertyCollection customProperties = sheet.CustomProperties;
            
            customProperties.Add("Author", "John Doe");
            customProperties.Add("Version", "1.0");
            customProperties.Add("DateCreated", DateTime.Now.ToString("yyyy-MM-dd"));
            
            for (int i = 0; i < customProperties.Count; i++)
            {
                CustomProperty property = customProperties[i];
                Console.WriteLine($"Property {i}: {property.Name} = {property.Value}");
            }
            
            workbook.Save("CustomPropertiesDemo.xlsx");
        }
    }
}
```

### См. также

* class [CustomProperty](../../customproperty/)
* class [CustomPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)

---

## CustomPropertyCollection indexer (2 of 2)

Получает пользовательское свойство по имени свойства.

```csharp
public CustomProperty this[string name] { get; }
```

| Параметр | Описание |
| --- | --- |
| name | Имя свойства. |

### Возвращаемое значение

Пользовательское свойство

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CustomPropertyCollectionPropertyItemDemo1
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавить пользовательские свойства
            worksheet.CustomProperties.Add("COR_Report", "Quarterly Report");
            worksheet.CustomProperties.Add("COR_ResultSet", "Sales Data");
            
            // Получить доступ и отобразить пользовательские свойства с помощью свойства Item
            Console.WriteLine("COR_Report: " + worksheet.CustomProperties["COR_Report"].Value);
            Console.WriteLine("COR_ResultSet: " + worksheet.CustomProperties["COR_ResultSet"].Value);
            
            // Изменить пользовательское свойство с помощью свойства Item
            worksheet.CustomProperties["COR_Report"].Value = "Annual Report";
            Console.WriteLine("Updated COR_Report: " + worksheet.CustomProperties["COR_Report"].Value);
        }
    }
}
```

### См. также

* class [CustomProperty](../../customproperty/)
* class [CustomPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


