---
title: "DocumentPropertyCollection.RemoveAt"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод DocumentPropertyCollection. Удаляет свойство по указанному индексу"
type: docs
url: /ru/net/aspose.cells.properties/documentpropertycollection/removeat/
---
## DocumentPropertyCollection.RemoveAt method

Удаляет свойство по указанному индексу.

```csharp
public void RemoveAt(int index)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| индекс | Int32 | Индекс, начинающийся с нуля. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Properties;
    using System;

    public class DocumentPropertyCollectionMethodRemoveAtWithInt32Demo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получите доступ к пользовательским свойствам документа (вместо встроенных)
            DocumentPropertyCollection properties = workbook.Worksheets.CustomDocumentProperties;
            
            // Добавьте несколько пользовательских свойств для демонстрации удаления
            ((CustomDocumentPropertyCollection)properties).Add("Property1", "Value1");
            ((CustomDocumentPropertyCollection)properties).Add("Property2", "Value2");
            ((CustomDocumentPropertyCollection)properties).Add("Property3", "Value3");

            try
            {
                // Отобразите свойства до удаления
                Console.WriteLine("Properties before removal:");
                foreach (DocumentProperty prop in properties)
                {
                    Console.WriteLine($"{prop.Name}: {prop.Value}");
                }

                // Вызовите RemoveAt с индексом 1 (второе свойство)
                properties.RemoveAt(1);

                // Отобразите свойства после удаления
                Console.WriteLine("\nProperties after removal:");
                foreach (DocumentProperty prop in properties)
                {
                    Console.WriteLine($"{prop.Name}: {prop.Value}");
                }

                Console.WriteLine("RemoveAt method executed successfully with parameter (Int32)");
            }
            catch (ArgumentOutOfRangeException ex)
            {
                Console.WriteLine($"Error: Index out of range. {ex.Message}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing RemoveAt method: {ex.Message}");
            }
            
            // Сохраните книгу
            workbook.Save("RemoveAtMethodDemo.xlsx");
        }
    }
}
```

### См. также

* class [DocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


