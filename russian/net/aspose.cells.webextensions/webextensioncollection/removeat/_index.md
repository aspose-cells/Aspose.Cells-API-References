---
title: "WebExtensionCollection.RemoveAt"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод WebExtensionCollection. Удаляет веб‑расширение по индексу"
type: docs
url: /ru/net/aspose.cells.webextensions/webextensioncollection/removeat/
---
## WebExtensionCollection.RemoveAt method

Удалить веб‑расширение по индексу.

```csharp
public void RemoveAt(int index)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| индекс | Int32 | Индекс. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.WebExtensions;
    using System;

    public class WebExtensionCollectionMethodRemoveAtWithInt32Demo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Создайте коллекцию веб‑расширений
            WebExtensionCollection webExtensions = workbook.Worksheets.WebExtensions;

            // Добавьте несколько веб-расширений в коллекцию
            int index1 = webExtensions.Add();
            int index2 = webExtensions.Add();
            int index3 = webExtensions.Add();

            Console.WriteLine($"WebExtensions count before RemoveAt: {webExtensions.Count}");

            try
            {
                // Вызовите метод RemoveAt с параметром Int32
                webExtensions.RemoveAt(index2);
                
                Console.WriteLine("Method executed successfully with parameter (Int32)");
                Console.WriteLine($"WebExtensions count after RemoveAt: {webExtensions.Count}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing RemoveAt method: {ex.Message}");
            }
            
            // Сохранить результат
            workbook.Save("WebExtensionCollectionMethodRemoveAtDemo.xlsx");
        }
    }
}
```

### См. также

* class [WebExtensionCollection](../)
* namespace [Aspose.Cells.WebExtensions](../../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../../)


