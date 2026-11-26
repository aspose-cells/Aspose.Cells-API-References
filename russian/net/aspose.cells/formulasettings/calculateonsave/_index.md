---
title: "FormulaSettings.CalculateOnSave"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство FormulaSettings. Указывает, следует ли пересчитывать книгу перед сохранением документа в режиме ручного расчёта."
type: docs
url: /ru/net/aspose.cells/formulasettings/calculateonsave/
---
## FormulaSettings.CalculateOnSave property

Указывает, следует ли пересчитывать книгу перед сохранением документа в режиме ручных вычислений.

```csharp
public bool CalculateOnSave { get; set; }
```

### Примечания

Это свойство используется только для сохранения настроек в результирующий файл таблицы, чтобы другие приложения (например, MS Excel) могли соответствующим образом реагировать при загрузке и работе с этим файлом. С учётом производительности большинства пользовательских приложений мы не вычисляем автоматически ни одну формулу в книге, независимо от установленного значения этого свойства.

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FormulaSettingsPropertyCalculateOnSaveDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получите доступ к листу и добавьте некоторые данные
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].Formula = "=SUM(A1:A2)";

            // Отключить CalculateOnSave (по умолчанию false)
            workbook.Settings.FormulaSettings.CalculateOnSave = false;
            
            // Сохранить без вычисления формул
            workbook.Save("output_without_calculation.xlsx");

            // Включить CalculateOnSave
            workbook.Settings.FormulaSettings.CalculateOnSave = true;
            
            // Сохранить с вычислением формул
            workbook.Save("output_with_calculation.xlsx");
        }
    }
}
```

### См. также

* class [FormulaSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


