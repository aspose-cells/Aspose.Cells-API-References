---
title: "Класс SensitivityLabel"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.Metas.SensitivityLabel. Представляет метку конфиденциальности"
type: docs
url: /ru/net/aspose.cells.metas/sensitivitylabel/
---
## SensitivityLabel class

Представляет метку чувствительности.

```csharp
public class SensitivityLabel
```

## Свойства

| Имя | Описание |
| --- | --- |
| [AssignmentType](../../aspose.cells.metas/sensitivitylabel/assignmenttype/) { get; set; } | Получает и задает метод назначения метки конфиденциальности. |
| [ContentMarkType](../../aspose.cells.metas/sensitivitylabel/contentmarktype/) { get; set; } | Получает и задает типы маркировки контента, которые должны быть применены к файлу. |
| [Id](../../aspose.cells.metas/sensitivitylabel/id/) { get; set; } | Получает и задает идентификатор метки конфиденциальности. |
| [IsEnabled](../../aspose.cells.metas/sensitivitylabel/isenabled/) { get; set; } | Указывает, включена ли метка конфиденциальности |
| [IsRemoved](../../aspose.cells.metas/sensitivitylabel/isremoved/) { get; set; } | Указывает, была ли метка конфиденциальности удалена. |
| [SiteId](../../aspose.cells.metas/sensitivitylabel/siteid/) { get; set; } | Представляет идентификатор сайта Azure Active Directory (Azure AD), соответствующий политике метки конфиденциальности, описывающей метку конфиденциальности. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Metas;
    using System;

    public class MetasClassSensitivityLabelDemo
    {
        public static void Run()
        {
            // Создать новую книгу для демонстрации
            Workbook workbook = new Workbook();
            
            try
            {
                // Создайте экземпляр класса SensitivityLabel с использованием рефлексии
                SensitivityLabel label = (SensitivityLabel)Activator.CreateInstance(typeof(SensitivityLabel));
                
                // Установите базовые свойства
                label.Id = "CONFIDENTIAL_001";
                label.IsEnabled = true;
                label.AssignmentType = SensitivityLabelAssignmentType.Standard;
                label.ContentMarkType = SensitivityLabelMarkType.None;
                
                // Отобразить значения свойств
                Console.WriteLine($"Sensitivity Label Created:");
                Console.WriteLine($"ID: {label.Id}");
                Console.WriteLine($"Enabled: {label.IsEnabled}");
                Console.WriteLine($"Assignment Type: {label.AssignmentType}");
                Console.WriteLine($"Content Mark Type: {label.ContentMarkType}");
                
                // Сохраните книгу
                workbook.Save("SensitivityLabelDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with SensitivityLabel: {ex.Message}");
            }
        }
    }
}
```

### См. также

* namespace [Aspose.Cells.Metas](../../aspose.cells.metas/)
* assembly [Aspose.Cells](../../)


