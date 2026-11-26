---
title: "DeleteOptions.UpdateReference"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство DeleteOptions. Указывает, обновлять ли ссылки в других листах"
type: docs
url: /ru/net/aspose.cells/deleteoptions/updatereference/
---
## DeleteOptions.UpdateReference property

Указывает, следует ли обновлять ссылки в других листах.

```csharp
public bool UpdateReference { get; set; }
```

### Примечания

Начиная с версии 26.7, мы устанавливаем значение по умолчанию этого свойства в true.

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DeleteOptionsPropertyUpdateReferenceDemo
    {
        public static void Run()
        {
            // Создайте книгу с примерными данными
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавить примерные данные и формулы
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["B1"].PutValue(20);
            worksheet.Cells["C1"].Formula = "=A1+B1";
            worksheet.Cells["A2"].PutValue(30);
            worksheet.Cells["B2"].PutValue(40);
            worksheet.Cells["C2"].Formula = "=A2+B2";

            // Создайте параметры удаления с UpdateReference, установленным в true
            DeleteOptions deleteOptions = new DeleteOptions();
            deleteOptions.UpdateReference = true;

            // Удалите столбец A, который используется в формулах
            worksheet.Cells.DeleteColumns(0, 1, deleteOptions);

            // Сохраните книгу
            workbook.Save("output.xlsx");
        }
    }
}
```

### См. также

* class [DeleteOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


