---
title: "PivotConditionalFormat.RuleType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство PivotConditionalFormat. Получайте и задавайте тип правила для условного форматирования сводной таблицы"
type: docs
url: /ru/net/aspose.cells.pivot/pivotconditionalformat/ruletype/
---
## PivotConditionalFormat.RuleType property

Получить и установить тип правила для условного форматирования сводной таблицы.

```csharp
public PivotConditionFormatRuleType RuleType { get; set; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotConditionalFormatPropertyRuleTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Создайте минимальные данные для сводной таблицы
                worksheet.Cells["A1"].Value = "Category";
                worksheet.Cells["A2"].Value = "Value";

                // Создать сводную таблицу
                int pivotIndex = worksheet.PivotTables.Add("A1:A2", "C3", "DemoPivotTable");
                PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

                // Добавить условный формат
                int formatIndex = pivotTable.ConditionalFormats.Add();
                PivotConditionalFormat format = pivotTable.ConditionalFormats[formatIndex];

                // Продемонстрируйте свойство RuleType
                Console.WriteLine("Initial RuleType: " + format.RuleType);
                
                // Установите новый тип правила
                format.RuleType = PivotConditionFormatRuleType.Row;
                Console.WriteLine("Updated RuleType: " + format.RuleType);

                workbook.Save("RuleTypeDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### См. также

* enum [PivotConditionFormatRuleType](../../pivotconditionformatruletype/)
* class [PivotConditionalFormat](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


