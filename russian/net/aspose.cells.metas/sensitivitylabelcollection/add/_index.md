---
title: "SensitivityLabelCollection.Add"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод SensitivityLabelCollection. Добавляет метку чувствительности"
type: docs
url: /ru/net/aspose.cells.metas/sensitivitylabelcollection/add/
---
## SensitivityLabelCollection.Add method

Добавляет метку конфиденциальности.

```csharp
public int Add(string id, bool isEnabled, SensitivityLabelAssignmentType methodType, string siteId, 
    SensitivityLabelMarkType markType)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| id | String | Идентификатор метки. |
| isEnabled | Boolean | Указывает, включена ли эта метка чувствительности. |
| methodType | SensitivityLabelAssignmentType | Тип метода назначения. |
| siteId | String | Идентификатор сайта. |
| markType | SensitivityLabelMarkType | Тип метки. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Metas;
    using System;

    public class SensitivityLabelCollectionMethodAddWithStringBooleanSensitivityLabelADemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Создайте новую SensitivityLabelCollection
            var sensitivityLabels = new SensitivityLabelCollection();
            
            try
            {
                // Вызовите метод Add с конкретными параметрами
                int index = sensitivityLabels.Add(
                    id: "Confidential",
                    isEnabled: true,
                    methodType: SensitivityLabelAssignmentType.Privileged,
                    siteId: "Contoso",
                    markType: SensitivityLabelMarkType.Watermark);
                
                Console.WriteLine($"Sensitivity label added at index: {index}");
                
                // Добавьте некоторые данные, чтобы продемонстрировать эффект
                worksheet.Cells["A1"].Value = "Confidential Data";
                worksheet.Cells["A2"].Value = "This document contains sensitive information";
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Add method: {ex.Message}");
            }
            
            // Сохранить результат
            workbook.Save("SensitivityLabelAddDemo.xlsx");
        }
    }
}
```

### См. также

* enum [SensitivityLabelAssignmentType](../../sensitivitylabelassignmenttype/)
* enum [SensitivityLabelMarkType](../../sensitivitylabelmarktype/)
* class [SensitivityLabelCollection](../)
* namespace [Aspose.Cells.Metas](../../../aspose.cells.metas/)
* assembly [Aspose.Cells](../../../)


