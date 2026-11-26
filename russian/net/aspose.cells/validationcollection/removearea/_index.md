---
title: "ValidationCollection.RemoveArea"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод ValidationCollection. Удаляет все настройки проверок в диапазоне"
type: docs
url: /ru/net/aspose.cells/validationcollection/removearea/
---
## ValidationCollection.RemoveArea method

Удаляет все настройки проверок в диапазоне..

```csharp
public void RemoveArea(CellArea ca)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| ca | CellArea | Диапазон, содержащий настройки проверок. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ValidationCollectionMethodRemoveAreaDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Создать проверку в конкретной области
            ValidationCollection validations = worksheet.Validations;
            CellArea validationArea = CellArea.CreateCellArea(0, 0, 5, 5);
            int validationIndex = validations.Add(validationArea);
            
            // Создайте область для удаления из проверки
            CellArea removeArea = CellArea.CreateCellArea(2, 2, 4, 4);
            
            try
            {
                // Вызовите метод RemoveArea с параметром CellArea
                validations.RemoveArea(removeArea);
                
                Console.WriteLine("Validation area removed successfully.");
                
                // Отобразите оставшиеся области проверок
                foreach (Validation validation in validations)
                {
                    if (validation.Areas.Length > 0)
                    {
                        Console.WriteLine($"Remaining validation area: {validation.Areas[0]}");
                    }
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing RemoveArea method: {ex.Message}");
            }
            
            // Сохранить результат
            workbook.Save("ValidationRemoveAreaDemo.xlsx");
        }
    }
}
```

### См. также

* struct [CellArea](../../cellarea/)
* class [ValidationCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


