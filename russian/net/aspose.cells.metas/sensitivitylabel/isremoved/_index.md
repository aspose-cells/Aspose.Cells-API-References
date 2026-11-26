---
title: "SensitivityLabel.IsRemoved"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство SensitivityLabel. Указывает, был ли удалён метка чувствительности"
type: docs
url: /ru/net/aspose.cells.metas/sensitivitylabel/isremoved/
---
## SensitivityLabel.IsRemoved property

Указывает, была ли метка конфиденциальности удалена.

```csharp
public bool IsRemoved { get; set; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Metas;
    using System;

    public class SensitivityLabelPropertyIsRemovedDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            try
            {
                // Создайте экземпляр метки чувствительности с помощью рефлексии
                // поскольку прямое создание недоступно
                Type labelType = typeof(SensitivityLabel);
                SensitivityLabel label = (SensitivityLabel)Activator.CreateInstance(labelType);
                
                // Установите необходимые свойства
                label.Id = "SENSITIVE_DATA";
                label.IsEnabled = true;
                label.IsRemoved = false;
                
                // Отобразите начальное значение IsRemoved
                Console.WriteLine("Initial IsRemoved value: " + label.IsRemoved);
                
                // Продемонстрируйте установку свойства IsRemoved (поскольку оно доступно для чтения и записи)
                label.IsRemoved = true;
                Console.WriteLine("After setting IsRemoved: " + label.IsRemoved);
                
                // Переключите значение обратно, чтобы показать, что его можно изменить
                label.IsRemoved = false;
                Console.WriteLine("Final IsRemoved value: " + label.IsRemoved);
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


