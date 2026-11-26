---
title: "Validation.AddArea"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Validation. Применяет проверку к области"
type: docs
url: /ru/net/aspose.cells/validation/addarea/
---
## AddArea(CellArea) {#addarea}

Применяет проверку к области.

```csharp
public void AddArea(CellArea cellArea)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| cellArea | CellArea | Область. |

### Примечания

Это эквивалентно использованию `AddArea` с проверкой пересечения и границы.

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ValidationMethodAddAreaWithCellAreaDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];

            // Создать проверку
            ValidationCollection vc = sheet.Validations;
            Validation validation = vc[vc.Add(CellArea.CreateCellArea(0, 0, 0, 0))];
            validation.Type = ValidationType.List;
            validation.Formula1 = "=A1:A10";

            // Добавить больше областей к проверке
            for (int i = 1; i < 5; i++)
            {
                validation.AddArea(CellArea.CreateCellArea(i, 0, i, 0));
            }

            // Сохраните книгу
            wb.Save("ValidationMethodAddAreaWithCellAreaDemo.xlsx", SaveFormat.Xlsx);

            Console.WriteLine("Validation with multiple areas created successfully.");
        }
    }
}
```

### См. также

* struct [CellArea](../../cellarea/)
* class [Validation](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## AddArea(CellArea, bool, bool) {#addarea_1}

Применяет проверку к области.

```csharp
public void AddArea(CellArea cellArea, bool checkIntersection, bool checkEdge)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| cellArea | CellArea | Область. |
| checkIntersection | Boolean | Определяет, проверять ли пересечение заданной области с областями существующих проверок. Если в заданной области (или её части) уже применена проверка, то существующая проверка должна сначала быть удалена из этой области. В противном случае может произойти повреждение сгенерированных проверок. Если пользователь уверен, что добавляемая область не пересекается ни с одной существующей областью, этот параметр можно установить в false для повышения производительности. |
| checkEdge | Boolean | Определяет, проверять ли границу применённых областей этой проверки. Внутренние настройки Validation зависят от верхней‑левой области её применённых диапазонов, поэтому если заданная область станет новой верхней‑левой областью применённых диапазонов, внутренние настройки должны быть изменены и перестроены, иначе могут возникнуть неожиданные результаты. Если пользователь уверен, что добавляемая область не является верхней‑левой, этот параметр можно установить в false для повышения производительности. |

### Примечания

В этом методе мы удалим все старые проверки в заданной области. Для верхней‑левой из применённых диапазонов Validation сначала её StartRow минимален, затем её StartColumn является наименьшим среди областей, имеющих тот же минимальный StartRow.

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ValidationMethodAddAreaWithCellAreaBooleanBooleanDemo
    {
        public static void Run()
        {
            // Создать книгу и получить первый лист
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Создать проверку в конкретной области
            Validation validation = worksheet.Validations[worksheet.Validations.Add(CellArea.CreateCellArea(5, 3, 6, 3))];
            validation.Operator = OperatorType.GreaterThan;
            validation.Formula1 = "F3";

            // Продемонстрировать AddArea с CellArea и двумя булевыми параметрами
            validation.AddArea(CellArea.CreateCellArea(3, 3, 3, 4), false, true);
            Console.WriteLine("Area count after AddArea: " + validation.Areas.Length);
            Console.WriteLine("Formula1 after AddArea: " + validation.Formula1);

            // Удалить добавленную область
            validation.RemoveArea(CellArea.CreateCellArea(3, 3, 3, 4));
            Console.WriteLine("Area count after RemoveArea: " + validation.Areas.Length);

            // Добавить несколько областей с массовой операцией
            CellArea[] areas = new CellArea[10];
            for (int i = 0; i < areas.Length; i++)
            {
                areas[i] = CellArea.CreateCellArea(6 + i, 3, 6 + i, 4);
            }
            validation.AddAreas(areas, true, true);
            Console.WriteLine("Area count after bulk AddAreas: " + validation.Areas.Length);

            // Сохраните книгу
            workbook.Save("ValidationMethodAddAreaDemo.xlsx");
        }
    }
}
```

### См. также

* struct [CellArea](../../cellarea/)
* class [Validation](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


