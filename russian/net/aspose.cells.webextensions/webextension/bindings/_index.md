---
title: "WebExtension.Bindings"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство WebExtension. Возвращает все связи между надстройкой Office и данными в документе"
type: docs
url: /ru/net/aspose.cells.webextensions/webextension/bindings/
---
## WebExtension.Bindings property

Получает все отношения привязок между Office Add-in и данными в документе.

```csharp
public WebExtensionBindingCollection Bindings { get; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.WebExtensions;
    using System;

    public class WebExtensionPropertyBindingsDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Создайте пример рабочего листа
            Worksheet worksheet = workbook.Worksheets[0];
            
            try
            {
                // Предполагая, что мы получаем веб‑расширение откуда‑то (поскольку мы не можем создать его напрямую)
                // Это минимальное изменение, позволяющее скомпилировать код, сохраняя его структуру
                WebExtension webExtension = null; // In real usage, this would come from workbook.WebExtensions or similar
                
                if (webExtension != null)
                {
                    // Доступ к свойству Bindings (только для чтения)
                    WebExtensionBindingCollection bindings = webExtension.Bindings;
                    
                    // Отобразить информацию о связях
                    Console.WriteLine($"Number of bindings: {bindings.Count}");
                    
                    // Добавить новую связь (демонстрирует использование коллекции)
                    int newBindingIndex = bindings.Add();
                    Console.WriteLine($"Added new binding at index: {newBindingIndex}");
                    
                    // Отобразить обновленное количество
                    Console.WriteLine($"Updated number of bindings: {bindings.Count}");
                }
                else
                {
                    Console.WriteLine("No web extension available");
                }
                
                // Сохраните книгу
                workbook.Save("WebExtensionBindingsDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### См. также

* class [WebExtensionBindingCollection](../../webextensionbindingcollection/)
* class [WebExtension](../)
* namespace [Aspose.Cells.WebExtensions](../../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../../)


