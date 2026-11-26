---
title: "PivotField.GetCalculatedFieldFormula"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод PivotField. Получить строку формулы указанного вычисляемого поля"
type: docs
url: /ru/net/aspose.cells.pivot/pivotfield/getcalculatedfieldformula/
---
## PivotField.GetCalculatedFieldFormula method

Получить строку формулы указанного вычисляемого поля.

```csharp
[Obsolete("Use PivotField.GetFormula() method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public string GetCalculatedFieldFormula()
```

### Примечания

ПРИМЕЧАНИЕ: Этот метод теперь устарел. Вместо него, пожалуйста, используйте метод PivotField.GetFormula(). Этот метод будет удалён через 12 месяцев, начиная с августа 2024 года. Компания Aspose приносит извинения за любые неудобства, которые вы могли испытать.

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotFieldMethodGetCalculatedFieldFormulaDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить примерные данные для сводной таблицы
            worksheet.Cells["A1"].Value = "Product";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["A3"].Value = "Banana";
            worksheet.Cells["A4"].Value = "Orange";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["B2"].Value = 100;
            worksheet.Cells["B3"].Value = 200;
            worksheet.Cells["B4"].Value = 150;
            worksheet.Cells["C1"].Value = "Profit";
            worksheet.Cells["C2"].Value = 20;
            worksheet.Cells["C3"].Value = 30;
            worksheet.Cells["C4"].Value = 25;

            // Создать сводную таблицу
            PivotTableCollection pivotTables = worksheet.PivotTables;
            int index = pivotTables.Add("A1:C4", "E3", "PivotTable1");
            PivotTable pivotTable = pivotTables[index];

            // Добавить поля в сводную таблицу
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Profit");

            // Добавить вычисляемое поле с помощью PivotFieldCollection
            PivotFieldCollection pivotFields = pivotTable.DataFields;
            pivotTable.AddCalculatedField("ProfitMargin", "Profit/Sales", true);

            try
            {
                // Получить вычисляемое поле из DataFields
                PivotField calculatedField = pivotTable.DataFields[2]; // Index 2 for the calculated field

                // Проверьте, является ли оно вычисляемым полем
                if (calculatedField.IsCalculatedField)
                {
                    // Получить формулу вычисляемого поля
                    string formula = calculatedField.GetFormula();
                    Console.WriteLine($"Calculated field formula: {formula}");

                    // Сохраните книгу
                    workbook.Save("GetCalculatedFieldFormulaDemo.xlsx");
                    Console.WriteLine("Workbook saved successfully.");
                }
                else
                {
                    Console.WriteLine("The field is not a calculated field.");
                }
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

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


