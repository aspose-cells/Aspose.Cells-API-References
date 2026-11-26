---
title: "PivotItem.IsFormula"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство PivotItem. Указывает, является ли этот элемент сводной таблицы вычисляемым формульным элементом"
type: docs
url: /ru/net/aspose.cells.pivot/pivotitem/isformula/
---
## PivotItem.IsFormula property

Указывает, является ли этот элемент сводки вычисляемым элементом формулы.

```csharp
[Obsolete("Use PivotItem.IsCalculatedItem property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool IsFormula { get; set; }
```

### Примечания

ПРИМЕЧАНИЕ: Это свойство теперь устарело. Вместо него, пожалуйста, используйте свойство PivotItem.IsCalculatedItem. Это свойство будет удалено через 12 месяцев, начиная с ноября 2024 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotItemPropertyIsFormulaDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте образцовые данные для сводной таблицы
            worksheet.Cells["A1"].Value = "Fruit";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["A3"].Value = "Orange";
            worksheet.Cells["A4"].Value = "Banana";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["B2"].Value = 10;
            worksheet.Cells["B3"].Value = 20;
            worksheet.Cells["B4"].Value = 30;

            // Создайте сводную таблицу
            int pivotIndex = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Получить первый элемент сводной таблицы
            PivotField pivotField = pivotTable.RowFields[0];
            PivotItem pivotItem = pivotField.PivotItems[0];

            // Отобразить текущее значение IsFormula (устаревшее свойство)
            Console.WriteLine("Current IsFormula value: " + pivotItem.IsFormula);

            // Установить новое значение для IsFormula (устаревшее свойство)
            pivotItem.IsFormula = true;

            // Продемонстрировать эффект — это пометит элемент сводной таблицы как формульный элемент
            Console.WriteLine("After setting IsFormula to true: " + pivotItem.IsFormula);

            // Примечание: При реальном использовании следует использовать IsCalculatedItem вместо IsFormula, который устарел
            Console.WriteLine("IsCalculatedItem (recommended property): " + pivotItem.IsCalculatedItem);

            // Сохранить результат
            workbook.Save("PivotItemPropertyIsFormulaDemo.xlsx");
        }
    }
}
```

### См. также

* class [PivotItem](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


