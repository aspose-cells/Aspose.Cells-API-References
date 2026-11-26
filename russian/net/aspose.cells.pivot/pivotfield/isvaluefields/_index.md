---
title: "PivotField.IsValueFields"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство PivotField. Указывает, является ли это поле полем значений"
type: docs
url: /ru/net/aspose.cells.pivot/pivotfield/isvaluefields/
---
## PivotField.IsValueFields property

Указывает, является ли это поле полем значений.

```csharp
[Obsolete("Use PivotField.IsValuesField property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool IsValueFields { get; }
```

### Примечания

ПРИМЕЧАНИЕ: Этот метод теперь устарел. Вместо него, пожалуйста, используйте свойство PivotField.IsValuesField. Этот метод будет удалён через 12 месяцев, начиная с ноября 2023 года. Компания Aspose приносит извинения за любые причинённые неудобства.

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotFieldPropertyIsValueFieldsDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте образцовые данные для сводной таблицы
            worksheet.Cells["A1"].Value = "Product";
            worksheet.Cells["B1"].Value = "Region";
            worksheet.Cells["C1"].Value = "Sales";
            worksheet.Cells["A2"].Value = "Bike";
            worksheet.Cells["A3"].Value = "Bike";
            worksheet.Cells["A4"].Value = "Car";
            worksheet.Cells["A5"].Value = "Car";
            worksheet.Cells["B2"].Value = "East";
            worksheet.Cells["B3"].Value = "West";
            worksheet.Cells["B4"].Value = "East";
            worksheet.Cells["B5"].Value = "West";
            worksheet.Cells["C2"].Value = 1000;
            worksheet.Cells["C3"].Value = 2000;
            worksheet.Cells["C4"].Value = 3000;
            worksheet.Cells["C5"].Value = 4000;

            // Создайте сводную таблицу
            int pivotIndex = worksheet.PivotTables.Add("=A1:C5", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // Добавить поле строки
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");

            // Добавить поле столбца
            pivotTable.AddFieldToArea(PivotFieldType.Column, "Region");

            // Добавьте поле данных и получите его из коллекции DataFields
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            PivotField dataField = pivotTable.DataFields[0];

            // Отобразите значение свойства IsValueFields
            Console.WriteLine("IsValueFields for data field: " + dataField.IsValueFields);

            // Попробуйте найти поле, не являющееся данными, чтобы показать, что IsValueFields равно false
            foreach (PivotField field in pivotTable.RowFields)
            {
                Console.WriteLine("IsValueFields for row field '" + field.Name + "': " + field.IsValueFields);
            }

            // Сохранить результат
            workbook.Save("PivotFieldPropertyIsValueFieldsDemo.xlsx");
        }
    }
}
```

### См. также

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


