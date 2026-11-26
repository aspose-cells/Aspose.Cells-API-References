---
title: "DocumentPropertyCollection.IndexOf"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод DocumentPropertyCollection. Возвращает индекс свойства по имени"
type: docs
url: /ru/net/aspose.cells.properties/documentpropertycollection/indexof/
---
## DocumentPropertyCollection.IndexOf method

Получает индекс свойства по имени.

```csharp
public int IndexOf(string name)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| name | String | Имя свойства без учёта регистра. |

### Возвращаемое значение

Индекс, начинающийся с нуля. Отрицательное значение, если не найдено.

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Properties;
    using System;

    public class DocumentPropertyCollectionMethodIndexOfWithStringDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить коллекцию встроенных свойств документа
            DocumentPropertyCollection properties = workbook.Worksheets.BuiltInDocumentProperties;

            // Для встроенных свойств можно задавать только значения существующих свойств
            // Чтобы добавить пользовательские свойства, необходимо использовать CustomDocumentPropertyCollection
            // Здесь мы просто установим несколько существующих встроенных свойств для демонстрации
            properties["Title"].Value = "Value1";
            properties["Subject"].Value = "Value2";
            properties["Author"].Value = "Value3";

            try
            {
                // Вызовите метод IndexOf со строковым параметром
                int index = properties.IndexOf("Subject");
                
                // Отобразить результат
                Console.WriteLine($"Index of 'Subject': {index}");
                
                // Показать свойство по найденному индексу
                if (index >= 0)
                {
                    DocumentProperty property = properties[index];
                    Console.WriteLine($"Property at index {index}: {property.Name} = {property.Value}");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing IndexOf method: {ex.Message}");
            }
            
            // Сохраните книгу
            workbook.Save("DocumentPropertyIndexOfDemo.xlsx");
        }
    }
}
```

### См. также

* class [DocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


