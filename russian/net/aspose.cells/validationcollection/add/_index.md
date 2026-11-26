---
title: "ValidationCollection.Add"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод ValidationCollection. Добавляет проверку данных в коллекцию"
type: docs
url: /ru/net/aspose.cells/validationcollection/add/
---
## Add() {#add}

Добавляет проверку данных в коллекцию.

```csharp
[Obsolete("Use ValidationCollection.Add(CellArea) method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int Add()
```

### Возвращаемое значение

[`Validation`](../../validation/) object index.

### Примечания

ПРИМЕЧАНИЕ: Этот метод теперь устарел. Вместо него, пожалуйста, используйте метод ValidationCollection.Add(CellArea). Этот метод будет удалён через 12 месяцев, начиная с ЯНВАРЯ 2015. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

### См. также

* class [ValidationCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Add(CellArea) {#add_1}

Добавляет проверку данных в коллекцию.

```csharp
public int Add(CellArea ca)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| ca | CellArea | Область содержит эту проверку. |

### Возвращаемое значение

[`Validation`](../../validation/) object index.

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ValidationCollectionMethodAddWithCellAreaDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Создайте область ячеек для проверки
            CellArea cellarea = new CellArea();
            cellarea.StartRow = 0;
            cellarea.StartColumn = 0;
            cellarea.EndRow = 1;
            cellarea.EndColumn = 1;
            
            // Добавьте проверку в коллекцию
            int index = sheet.Validations.Add(cellarea);
            Validation validation = sheet.Validations[index];
            
            // Настроить параметры проверки
            validation.Type = ValidationType.List;
            validation.Formula1 = "Yes,No";
            validation.AlertStyle = ValidationAlertType.Information;
            
            // Сохраните книгу
            workbook.Save("ValidationCollectionMethodAddWithCellAreaDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### См. также

* struct [CellArea](../../cellarea/)
* class [ValidationCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


