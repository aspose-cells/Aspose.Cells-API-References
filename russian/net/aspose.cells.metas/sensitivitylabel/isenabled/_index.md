---
title: "SensitivityLabel.IsEnabled"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство SensitivityLabel. Указывает, включена ли метка чувствительности"
type: docs
url: /ru/net/aspose.cells.metas/sensitivitylabel/isenabled/
---
## SensitivityLabel.IsEnabled property

Указывает, включена ли метка конфиденциальности

```csharp
public bool IsEnabled { get; set; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Metas;
    using System;

    public class SensitivityLabelPropertyIsEnabledDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            try
            {
                // Создайте экземпляр метки чувствительности
                SensitivityLabel label = (SensitivityLabel)Activator.CreateInstance(typeof(SensitivityLabel));
                
                // Установите начальные свойства
                label.Id = "CONFIDENTIAL_001";
                
                // Продемонстрируйте получение начального значения IsEnabled
                Console.WriteLine("Initial IsEnabled value: " + label.IsEnabled);
                
                // Установите IsEnabled в true и отобразите изменение
                label.IsEnabled = true;
                Console.WriteLine("After enabling: " + label.IsEnabled);
                
                // Переключите значение, чтобы продемонстрировать, что оно доступно для чтения и записи
                label.IsEnabled = false;
                Console.WriteLine("After disabling: " + label.IsEnabled);
                
                // Сохраните книгу
                workbook.Save("IsEnabledDemo.xlsx");
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


