---
title: "Validation.InCellDropDown"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Validation. Указывает, отображает ли проверка данных выпадающий список, содержащий допустимые значения"
type: docs
url: /ru/net/aspose.cells/validation/incelldropdown/
---
## Validation.InCellDropDown property

Указывает, отображает ли проверка данных выпадающий список с допустимыми значениями.

```csharp
public bool InCellDropDown { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ValidationPropertyInCellDropDownDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Создать проверку для ячейки A1
            Validation validation = worksheet.Cells["A1"].GetValidation();
            
            // Установить тип проверки в список со значениями
            validation.Type = ValidationType.List;
            validation.Formula1 = "Option1,Option2,Option3";
            
            // Включить выпадающий список в ячейке
            validation.InCellDropDown = true;

            // Создать другую проверку для ячейки B1 без выпадающего списка
            Validation validation2 = worksheet.Cells["B1"].GetValidation();
            validation2.Type = ValidationType.List;
            validation2.Formula1 = "Choice1,Choice2,Choice3";
            validation2.InCellDropDown = false;

            // Сохраните книгу
            workbook.Save("InCellDropDownDemo.xlsx");
        }
    }
}
```

### См. также

* class [Validation](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


