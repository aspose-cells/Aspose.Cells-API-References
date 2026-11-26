---
title: "FormulaSettings.PreservePaddingSpaces"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство FormulaSettings. Указывает, следует ли сохранять пробелы и разрывы строк, добавленные между токенами формулы при получении и установке формул. Значение по умолчанию — false."
type: docs
url: /ru/net/aspose.cells/formulasettings/preservepaddingspaces/
---
## FormulaSettings.PreservePaddingSpaces property

Указывает, сохранять ли пробелы и разрывы строк, вставленные между токенами формулы при получении и установке формул. Значение по умолчанию — false.

```csharp
public bool PreservePaddingSpaces { get; set; }
```

### Примечания

Обычно эти пробелы и разрывы строк нужны только для визуального оформления, их сохранение или отсутствие не влияет на вычисленный результат. С учётом производительности, если нет особых требований, лучше не сохранять их при обработке формул.

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FormulaSettingsPropertyPreservePaddingSpacesDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Установить формулу с пробелами-отступами
            string formulaWithSpaces = "=SUM( IF( A1:A5 > 10, B1:B5, 0 ) )";
            worksheet.Cells["C1"].Formula = formulaWithSpaces;
            
            // Поведение по умолчанию (PreservePaddingSpaces = true)
            Console.WriteLine("Formula with spaces preserved: " + worksheet.Cells["C1"].Formula);
            
            // Изменить настройку для удаления пробелов-отступов
            workbook.Settings.FormulaSettings.PreservePaddingSpaces = false;
            worksheet.Cells["C2"].Formula = formulaWithSpaces;
            
            Console.WriteLine("Formula with spaces removed: " + worksheet.Cells["C2"].Formula);
            
            // Сохраните книгу
            workbook.Save("FormulaSpacesDemo.xlsx");
        }
    }
}
```

### См. также

* class [FormulaSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


