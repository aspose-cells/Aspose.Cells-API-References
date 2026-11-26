---
title: "SensitivityLabel.AssignmentType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство SensitivityLabel. Получает и задает метод назначения для метки чувствительности"
type: docs
url: /ru/net/aspose.cells.metas/sensitivitylabel/assignmenttype/
---
## SensitivityLabel.AssignmentType property

Получает и задает метод назначения метки конфиденциальности.

```csharp
public SensitivityLabelAssignmentType AssignmentType { get; set; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Metas;
    using System;

    public class SensitivityLabelPropertyAssignmentTypeDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            try
            {
                // Создайте экземпляр метки чувствительности
                SensitivityLabel label = (SensitivityLabel)Activator.CreateInstance(typeof(SensitivityLabel));
                
                // Установите базовые свойства
                label.Id = "CONFIDENTIAL_001";
                label.IsEnabled = true;
                
                // Продемонстрируйте получение начального значения AssignmentType
                Console.WriteLine("Initial AssignmentType: " + label.AssignmentType);
                
                // Установите AssignmentType в Privileged и отобразите изменение
                label.AssignmentType = SensitivityLabelAssignmentType.Privileged;
                Console.WriteLine("After setting Privileged: " + label.AssignmentType);
                
                // Верните значение обратно в Standard, чтобы продемонстрировать, что оно читаемо‑записываемо
                label.AssignmentType = SensitivityLabelAssignmentType.Standard;
                Console.WriteLine("After setting Standard: " + label.AssignmentType);
                
                // Сохраните книгу
                workbook.Save("AssignmentTypeDemo.xlsx");
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

* enum [SensitivityLabelAssignmentType](../../sensitivitylabelassignmenttype/)
* class [SensitivityLabel](../)
* namespace [Aspose.Cells.Metas](../../../aspose.cells.metas/)
* assembly [Aspose.Cells](../../../)


