---
title: "Validation.AddAreas"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Validation. Применяет проверку к указанным областям"
type: docs
url: /ru/net/aspose.cells/validation/addareas/
---
## Validation.AddAreas method

Применяет проверку к указанным областям.

```csharp
public void AddAreas(CellArea[] areas, bool checkIntersection, bool checkEdge)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| области | CellArea[] | Области. |
| checkIntersection | Boolean | Проверять пересечение заданной области с областями существующих проверок. Если одна проверка была применена в заданной области (или её части), то существующая проверка должна быть сначала удалена из заданной области. В противном случае может произойти повреждение сгенерированных проверок. Если пользователь уверен, что все добавленные области не пересекаются с любой существующей областью, этот параметр можно установить в false для повышения производительности. |
| checkEdge | Boolean | Проверять границу применённых областей этой проверки. Внутренние настройки проверки зависят от верхнего левого элемента её применённых диапазонов, поэтому если одна из заданных областей станет новым верхним левым элементом применённых диапазонов, внутренние настройки должны быть изменены и перестроены, иначе может возникнуть неожиданный результат. Если пользователь уверен, что ни одна из добавленных областей не является верхним левым, этот параметр можно установить в false для повышения производительности. |

### Примечания

В этом методе мы удалим все старые проверки в заданной области. Для верхней‑левой из применённых диапазонов Validation сначала её StartRow минимален, затем её StartColumn является наименьшим среди областей, имеющих тот же минимальный StartRow.

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ValidationMethodAddAreasWithCellAreaBooleanBooleanDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            int validationIndex = worksheet.Validations.Add();
            Validation validation = worksheet.Validations[validationIndex];
            validation.Type = ValidationType.List;
            validation.AlertStyle = ValidationAlertType.Stop;
            validation.Operator = OperatorType.None;
            validation.Formula1 = "1,2,3";
            validation.InCellDropDown = true;

            CellArea[] areas = new CellArea[2];
            areas[0] = new CellArea { StartRow = 0, StartColumn = 0, EndRow = 1, EndColumn = 1 };
            areas[1] = new CellArea { StartRow = 2, StartColumn = 2, EndRow = 3, EndColumn = 3 };

            try
            {
                validation.AddAreas(areas, true, false);
                Console.WriteLine("Added validation areas with checkIntersection=true, checkEdge=false");

                foreach (CellArea area in validation.Areas)
                {
                    Console.WriteLine($"Validation area: R{area.StartRow + 1}C{area.StartColumn + 1}:R{area.EndRow + 1}C{area.EndColumn + 1}");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error adding validation areas: {ex.Message}");
            }

            workbook.Save("ValidationAddAreasDemo.xlsx");
        }
    }
}
```

### См. также

* struct [CellArea](../../cellarea/)
* class [Validation](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


