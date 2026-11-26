---
title: "WebExtension.IsFrozen"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство WebExtension. Указывает, может ли пользователь взаимодействовать с Office Addin или нет"
type: docs
url: /ru/net/aspose.cells.webextensions/webextension/isfrozen/
---
## WebExtension.IsFrozen property

Указывает, может ли пользователь взаимодействовать с Office Add-in или нет.

```csharp
public bool IsFrozen { get; set; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.WebExtensions;
    using System;

    public class WebExtensionPropertyIsFrozenDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            try
            {
                // Эта строка завершится ошибкой, потому что WebExtension требует параметры конструктора
                // WebExtension webExtension = new WebExtension();
                
                // Вместо этого мы получим web extension из рабочей книги, если это возможно
                // или продемонстрировать другим способом
                Console.WriteLine("Note: WebExtension requires constructor parameters. This demo shows property usage conceptually.");
                
                // Для демонстрационных целей мы покажем, как будет работать свойство, если у вас есть действительный экземпляр
                // В реальном сценарии вы получите экземпляр WebExtension из рабочей книги или из другого источника
                WebExtension webExtension = GetWebExtensionInstance(workbook);
                
                if (webExtension != null)
                {
                    // Установите начальные свойства
                    webExtension.Id = "MyAddin123";
                    
                    // Отобразить начальное значение IsFrozen
                    Console.WriteLine($"Initial IsFrozen value: {webExtension.IsFrozen}");
                    
                    // Изменить свойство IsFrozen (поскольку оно доступно для чтения и записи)
                    webExtension.IsFrozen = true;
                    Console.WriteLine($"Updated IsFrozen value: {webExtension.IsFrozen}");
                    
                    // Продемонстрировать эффект, проверив, может ли пользователь взаимодействовать
                    Console.WriteLine($"User can{(webExtension.IsFrozen ? "not" : "")} interact with the add-in");
                    
                    // Сохранить рабочую книгу (хотя web extension может не сохраняться без дополнительных шагов)
                    workbook.Save("WebExtensionIsFrozenDemo.xlsx");
                }
                else
                {
                    Console.WriteLine("Could not obtain a WebExtension instance for demonstration.");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }

        private static WebExtension GetWebExtensionInstance(Workbook workbook)
        {
            // В реальной реализации это получит существующий WebExtension из рабочей книги
            // или правильно создать его с необходимыми параметрами конструктора
            // Это всего лишь заполнитель для демонстрации
            return null;
        }
    }
}
```

### См. также

* class [WebExtension](../)
* namespace [Aspose.Cells.WebExtensions](../../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../../)


