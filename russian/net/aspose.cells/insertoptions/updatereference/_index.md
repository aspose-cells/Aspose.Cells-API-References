---
title: "InsertOptions.UpdateReference"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство InsertOptions. Указывает, будут ли обновляться ссылки в других листах"
type: docs
url: /ru/net/aspose.cells/insertoptions/updatereference/
---
## InsertOptions.UpdateReference property

Указывает, будут ли обновляться ссылки в других листах.

```csharp
public bool UpdateReference { get; set; }
```

### Примечания

Начиная с версии 26.7, мы устанавливаем значение по умолчанию этого свойства в true.

### Примеры

```csharp
using System;
using System.Collections.Generic;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class InsertOptionsPropertyUpdateReferenceDemo
    {
        public static void Run()
        {
            // Создать книгу
            Workbook wb = new Workbook();
            
            // Добавьте второй лист и задайте формулы, которые ссылаются на Sheet1
            Worksheet sheet2 = wb.Worksheets.Add("Sheet2");
            sheet2.Cells["A1"].Formula = "=Sheet1!A10";
            sheet2.Cells["B1"].Formula = "=Sheet1!A5";
            
            // Задайте формулы в Sheet1
            Worksheet sheet1 = wb.Worksheets[0];
            sheet1.Cells["A1"].Formula = "=A10";
            sheet1.Cells["B1"].Formula = "=A5";

            // Создайте параметры вставки с включённым UpdateReference
            InsertOptions iopts = new InsertOptions();
            iopts.UpdateReference = true;
            
            // Отслеживать изменения формул
            HashSet<string> changedCells = new HashSet<string>();
            iopts.UpdateReference = true;
            
            // Вставьте строки, которые обновят ссылки в формулах
            sheet1.Cells.InsertRows(5, 3, iopts);
            
            // Выведите количество изменённых ячеек
            Console.WriteLine("Formulas were automatically updated due to UpdateReference=true");
            
            // Отобразите обновлённые формулы
            Console.WriteLine("Sheet1 A1 formula: " + sheet1.Cells["A1"].Formula);
            Console.WriteLine("Sheet2 A1 formula: " + sheet2.Cells["A1"].Formula);
        }
    }
}
```

### См. также

* class [InsertOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


