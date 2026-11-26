---
title: "FormulaSettings.CalculateOnOpen"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство FormulaSettings. Указывает, требуется ли приложению выполнять полное вычисление при открытии книги"
type: docs
url: /ru/net/aspose.cells/formulasettings/calculateonopen/
---
## FormulaSettings.CalculateOnOpen property

Указывает, требуется ли приложению выполнить полное вычисление при открытии книги.

```csharp
public bool CalculateOnOpen { get; set; }
```

### Примечания

Это свойство предназначено только для сохранения настроек в результирующий файл таблицы, чтобы другие приложения (например, MS Excel) могли соответствующим образом реагировать при загрузке результирующего файла. С учётом производительности большинства пользовательских приложений мы не вычисляем автоматически ни одну формулу в книге, независимо от того, какое значение установлено для этого свойства.

### Примеры

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FormulaSettingsPropertyCalculateOnOpenDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Установить формулу в ячейке A1, которая ссылается на B1
            worksheet.Cells["A1"].Formula = "=B1";
            
            // Установить значение в ячейке B1
            worksheet.Cells["B1"].PutValue(10);
            
            // Отключить автоматическое вычисление формул при открытии
            workbook.Settings.FormulaSettings.CalculateOnOpen = false;
            
            // Сохраните книгу
            workbook.Save("output.xlsx", SaveFormat.Xlsx);
            
            // Повторно открыть сохранённую книгу
            Workbook reopenedWorkbook = new Workbook("output.xlsx");
            
            // Проверить, что формула не была вычислена при открытии
            Console.WriteLine("A1 value (should be 0 before calculation): " + reopenedWorkbook.Worksheets[0].Cells["A1"].IntValue);
            
            // Вычислить формулы вручную
            reopenedWorkbook.CalculateFormula();
            
            // Проверить, что формула была вычислена
            Console.WriteLine("A1 value (should be 10 after calculation): " + reopenedWorkbook.Worksheets[0].Cells["A1"].IntValue);
        }
    }
}
```

### См. также

* class [FormulaSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


