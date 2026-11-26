---
title: "SettableGlobalizationSettings.RowSeparatorOfFormulaArray"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство SettableGlobalizationSettings. Возвращает разделитель строк в массивных данных формулы"
type: docs
url: /ru/net/aspose.cells/settableglobalizationsettings/rowseparatorofformulaarray/
---
## SettableGlobalizationSettings.RowSeparatorOfFormulaArray property

Получает разделитель для строк в массивных данных в формуле.

```csharp
public override char RowSeparatorOfFormulaArray { get; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SettableGlobalizationSettingsPropertyRowSeparatorOfFormulaArrayDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Создайте экземпляр SettableGlobalizationSettings
            SettableGlobalizationSettings settings = new SettableGlobalizationSettings();

            // Отобразить разделитель строк по умолчанию для массивов формул
            Console.WriteLine("Default RowSeparatorOfFormulaArray value: " + settings.RowSeparatorOfFormulaArray);

            // Установить новый разделитель строк для массивов формул
            settings.SetRowSeparatorOfFormulaArray(';');

            // Применить настройки к рабочей книге
            workbook.Settings.GlobalizationSettings = settings;

            // Создать массивную формулу в листе
            worksheet.Cells["A1"].SetArrayFormula("={1,2,3;4,5,6}", 2, 3);
            worksheet.Cells["A2"].SetArrayFormula("=SUM(A1:C2)", 1, 1);

            // Вычислить формулы
            workbook.CalculateFormula();

            // Сохраните книгу
            workbook.Save("PropertyRowSeparatorOfFormulaArrayDemo.xlsx");
        }
    }
}
```

### См. также

* class [SettableGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


