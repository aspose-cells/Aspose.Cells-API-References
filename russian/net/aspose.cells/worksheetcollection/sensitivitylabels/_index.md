---
title: "WorksheetCollection.SensitivityLabels"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство WorksheetCollection. Представляет все метки чувствительности"
type: docs
url: /ru/net/aspose.cells/worksheetcollection/sensitivitylabels/
---
## WorksheetCollection.SensitivityLabels property

Представляет все метки чувствительности.

```csharp
public SensitivityLabelCollection SensitivityLabels { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Metas;

namespace AsposeCellsExamples
{
    public class WorksheetCollectionPropertySensitivityLabelsDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к коллекции листов
            WorksheetCollection worksheets = workbook.Worksheets;
            
            // Добавить метку чувствительности
            int index = worksheets.SensitivityLabels.Add(
                "{7e848398-70bd-400c-b8cf-2ab6f30d1b60}", // ID
                true,                                       // IsEnabled
                SensitivityLabelAssignmentType.Standard,     // AssignmentType
                "contoso-site",                             // SiteId
                SensitivityLabelMarkType.Header              // MarkType
            );
            
            // Проверить добавленную метку
            SensitivityLabel label = worksheets.SensitivityLabels[index];
            Console.WriteLine($"Label added - ID: {label.Id}, SiteID: {label.SiteId}");
            
            // Сохраните книгу
            workbook.Save("SensitivityLabelsDemo.xlsx");
        }
    }
}
```

### См. также

* class [SensitivityLabelCollection](../../../aspose.cells.metas/sensitivitylabelcollection/)
* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


