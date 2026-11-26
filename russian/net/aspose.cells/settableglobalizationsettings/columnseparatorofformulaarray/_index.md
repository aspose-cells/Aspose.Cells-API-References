---
title: "SettableGlobalizationSettings.ColumnSeparatorOfFormulaArray"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство SettableGlobalizationSettings. Возвращает разделитель для элементов в строковых данных массивов в формуле"
type: docs
url: /ru/net/aspose.cells/settableglobalizationsettings/columnseparatorofformulaarray/
---
## SettableGlobalizationSettings.ColumnSeparatorOfFormulaArray property

Получает разделитель для элементов в строковых данных массива в формуле.

```csharp
public override char ColumnSeparatorOfFormulaArray { get; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SettableGlobalizationSettingsPropertyColumnSeparatorOfFormulaArrayDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Создайте экземпляр SettableGlobalizationSettings
            SettableGlobalizationSettings settings = new SettableGlobalizationSettings();

            // Отобразить текущее значение ColumnSeparatorOfFormulaArray
            Console.WriteLine("Current ColumnSeparatorOfFormulaArray value: " + settings.ColumnSeparatorOfFormulaArray);

            // Установить новое значение для ColumnSeparatorOfFormulaArray
            settings.SetColumnSeparatorOfFormulaArray(';');

            // Применить настройки к рабочей книге
            workbook.Settings.GlobalizationSettings = settings;

            // Создать массивную формулу с пользовательским разделителем, используя SetArrayFormula
            worksheet.Cells["A1"].SetArrayFormula("SUM({1,2,3;4,5,6})", 1, 1);
            worksheet.Cells["A2"].Formula = "=SUM(A1)";

            // Вычислить формулы
            workbook.CalculateFormula();

            // Отобразить результат
            Console.WriteLine("Result of array formula calculation: " + worksheet.Cells["A2"].Value);

            // Сохраните книгу
            workbook.Save("PropertyColumnSeparatorOfFormulaArrayDemo.xlsx");
        }
    }
}
```

### См. также

* class [SettableGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


