---
title: "Validation.RemoveAreas"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Validation. Удаляет эту проверку из указанных областей"
type: docs
url: /ru/net/aspose.cells/validation/removeareas/
---
## Validation.RemoveAreas method

Удаляет эту проверку из указанных областей.

```csharp
public void RemoveAreas(CellArea[] areas)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| области | CellArea[] | области, где эти настройки проверки должны быть удалены. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ValidationMethodRemoveAreasWithCellAreaArrayDemo
    {
        public static void Run()
        {
            // Создайте новую книгу и получите доступ к первому листу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить проверку данных в лист
            int validationIndex = worksheet.Validations.Add();
            Validation validation = worksheet.Validations[validationIndex];
            
            // Настроить параметры проверки
            validation.Type = ValidationType.WholeNumber;
            validation.Operator = OperatorType.Between;
            validation.Formula1 = "1";
            validation.Formula2 = "10";

            // Создать две области ячеек для проверки
            CellArea area1 = new CellArea
            {
                StartRow = 0,
                StartColumn = 0,
                EndRow = 1,
                EndColumn = 1
            };  // A1:B2
            CellArea area2 = new CellArea
            {
                StartRow = 2,
                StartColumn = 2,
                EndRow = 3,  // Original code had (2,2,1,1) which would be invalid endRow < startRow
                EndColumn = 3
            };  // C3:D4 (corrected end coordinates)
            
            // Добавить области к проверке
            validation.AddArea(area1);
            validation.AddArea(area2);
            Console.WriteLine($"Added areas: {validation.Areas.Length}");

            try
            {
                // Создать массив с одной областью для удаления
                CellArea[] removeAreas = { area1 };
                
                // Выполнить метод RemoveAreas
                validation.RemoveAreas(removeAreas);
                Console.WriteLine($"Remaining areas after removal: {validation.Areas.Length}");
                
                // Отобразить координаты оставшихся областей
                foreach (CellArea remainingArea in validation.Areas)
                {
                    Console.WriteLine($"Area: {remainingArea.StartRow},{remainingArea.StartColumn} to {remainingArea.EndRow},{remainingArea.EndColumn}");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }

            // Сохранить изменённую книгу
            workbook.Save("ValidationRemoveAreasDemo.xlsx");
        }
    }
}
```

### См. также

* struct [CellArea](../../cellarea/)
* class [Validation](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


