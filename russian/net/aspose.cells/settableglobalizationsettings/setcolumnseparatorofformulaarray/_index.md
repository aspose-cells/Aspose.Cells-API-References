---
title: "SettableGlobalizationSettings.SetColumnSeparatorOfFormulaArray"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод SettableGlobalizationSettings. Устанавливает разделитель для элементов в строковых данных массивов в формуле"
type: docs
url: /ru/net/aspose.cells/settableglobalizationsettings/setcolumnseparatorofformulaarray/
---
## SettableGlobalizationSettings.SetColumnSeparatorOfFormulaArray method

Устанавливает разделитель для элементов данных строки массива в формуле.

```csharp
public void SetColumnSeparatorOfFormulaArray(char c)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| c | Char | указанный разделитель |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SettableGlobalizationSettingsMethodSetColumnSeparatorOfFormulaArrayWithCharDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            SettableGlobalizationSettings globalizationSettings = new SettableGlobalizationSettings();
            
            try
            {
                globalizationSettings.SetColumnSeparatorOfFormulaArray('|');
                workbook.Settings.GlobalizationSettings = globalizationSettings;

                worksheet.Cells["A1"].SetArrayFormula("{1|2|3}", 1, 3);
                Console.WriteLine("Column separator for formula arrays set to '|'.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetColumnSeparatorOfFormulaArray: {ex.Message}");
            }

            workbook.Save("SetColumnSeparatorOfFormulaArrayWithCharDemo.xlsx");
        }
    }
}
```

### См. также

* class [SettableGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


