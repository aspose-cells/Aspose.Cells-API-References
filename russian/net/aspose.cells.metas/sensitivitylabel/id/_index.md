---
title: "SensitivityLabel.Id"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство SensitivityLabel. Получает и задаёт идентификатор метки чувствительности"
type: docs
url: /ru/net/aspose.cells.metas/sensitivitylabel/id/
---
## SensitivityLabel.Id property

Получает и задает идентификатор метки конфиденциальности.

```csharp
public string Id { get; set; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Metas;
    using System;

    public class SensitivityLabelPropertyIdDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            try
            {
                // Создайте экземпляр метки чувствительности
                Type labelType = typeof(SensitivityLabel);
                SensitivityLabel label = (SensitivityLabel)Activator.CreateInstance(labelType);
                
                // Продемонстрировать установку и получение свойства Id
                string testId = "CONFIDENTIAL_001";
                label.Id = testId;
                
                // Отобразить значение Id
                Console.WriteLine("Sensitivity Label Id: " + label.Id);
                
                // Измените значение Id, чтобы продемонстрировать, что оно доступно для чтения и записи
                label.Id = "INTERNAL_USE_ONLY";
                Console.WriteLine("Updated Sensitivity Label Id: " + label.Id);
                
                // Показать, как свойство влияет на другие операции
                label.IsEnabled = true;
                Console.WriteLine($"Label {label.Id} is enabled: {label.IsEnabled}");
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

* class [SensitivityLabel](../)
* namespace [Aspose.Cells.Metas](../../../aspose.cells.metas/)
* assembly [Aspose.Cells](../../../)


