---
title: "WebExtensionPropertyCollection.RemoveAt"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод WebExtensionPropertyCollection. Удаляет свойство по имени"
type: docs
url: /ru/net/aspose.cells.webextensions/webextensionpropertycollection/removeat/
---
## WebExtensionPropertyCollection.RemoveAt method

Удаляет свойство по имени.

```csharp
public void RemoveAt(string name)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| name | String | Имя свойства. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.WebExtensions;
    using System;

    public class WebExtensionPropertyCollectionMethodRemoveAtWithStringDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Создать коллекцию свойств веб-расширения
            WebExtensionPropertyCollection properties = new WebExtensionPropertyCollection();

            // Добавить несколько свойств в коллекцию
            properties.Add("Property1", "Value1");
            properties.Add("Property2", "Value2");
            properties.Add("Property3", "Value3");

            try
            {
                // Вызвать метод RemoveAt с параметром string
                properties.RemoveAt("Property2");

                Console.WriteLine("Property with name 'Property2' removed successfully.");
                
                // Отобразить оставшиеся свойства
                Console.WriteLine("Remaining properties:");
                for (int i = 0; i < properties.Count; i++)
                {
                    Console.WriteLine($"{properties[i].Name}: {properties[i].Value}");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing RemoveAt method: {ex.Message}");
            }
            
            // Сохраните книгу
            workbook.Save("WebExtensionPropertyCollectionDemo.xlsx");
        }
    }
}
```

### См. также

* class [WebExtensionPropertyCollection](../)
* namespace [Aspose.Cells.WebExtensions](../../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../../)


