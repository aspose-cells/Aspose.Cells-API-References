---
title: "CopyOptions.CopyInvalidFormulasAsValues"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство CopyOptions. Если формула недействительна для целевого листа, копировать только значения"
type: docs
url: /ru/net/aspose.cells/copyoptions/copyinvalidformulasasvalues/
---
## CopyOptions.CopyInvalidFormulasAsValues property

Если формула недействительна для целевого назначения, копировать только значения.

```csharp
public bool CopyInvalidFormulasAsValues { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CopyOptionsPropertyCopyInvalidFormulasAsValuesDemo
    {
        public static void Run()
        {
            // Создайте исходную книгу с образцовым листом
            Workbook srcWorkbook = new Workbook();
            Worksheet srcSheet = srcWorkbook.Worksheets[0];
            
            // Добавьте формулу, которая может быть недействительной в некоторых контекстах
            srcSheet.Cells["A1"].Formula = "=1/0"; // Division by zero - invalid formula
            srcSheet.Cells["A2"].Value = "Valid Data";

            // Создайте целевую книгу
            Workbook destWorkbook = new Workbook();
            
            // Установите параметры копирования для преобразования недействительных формул в значения
            CopyOptions copyOptions = new CopyOptions();
            copyOptions.CopyInvalidFormulasAsValues = true;

            // Скопируйте лист с указанными параметрами
            destWorkbook.Worksheets[0].Copy(srcSheet, copyOptions);

            // Проверьте результаты
            Console.WriteLine("A1 (invalid formula copied as value): " + 
                destWorkbook.Worksheets[0].Cells["A1"].Value); // Should show #DIV/0! as value
            Console.WriteLine("A2 (valid data): " + 
                destWorkbook.Worksheets[0].Cells["A2"].Value); // Should show "Valid Data"
        }
    }
}
```

### См. также

* class [CopyOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


