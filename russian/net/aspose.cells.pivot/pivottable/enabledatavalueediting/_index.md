---
title: "PivotTable.EnableDataValueEditing"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство PivotTable. Указывает логическое значение, определяющее, может ли пользователь редактировать ячейки в области данных сводной таблицы. Значение по умолчанию — false"
type: docs
url: /ru/net/aspose.cells.pivot/pivottable/enabledatavalueediting/
---
## PivotTable.EnableDataValueEditing property

Указывает логическое значение, определяющее, разрешено ли пользователю редактировать ячейки в области данных pivottable. Значение по умолчанию — false.

```csharp
public bool EnableDataValueEditing { get; set; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotTablePropertyEnableDataValueEditingDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте образцовые данные для сводной таблицы
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["A2"].PutValue("Bike");
            worksheet.Cells["B2"].PutValue(1000);
            worksheet.Cells["A3"].PutValue("Car");
            worksheet.Cells["B3"].PutValue(2000);
            worksheet.Cells["A4"].PutValue("Bike");
            worksheet.Cells["B4"].PutValue(1500);
            worksheet.Cells["A5"].PutValue("Car");
            worksheet.Cells["B5"].PutValue(3000);

            // Добавить сводную таблицу
            int pivotIndex = worksheet.PivotTables.Add("A1:B5", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // Добавить поле строки и поле данных
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Отобразить текущее значение EnableDataValueEditing
            Console.WriteLine("Current EnableDataValueEditing value: " + pivotTable.EnableDataValueEditing);

            // Включить редактирование значений данных
            pivotTable.EnableDataValueEditing = true;

            // Вычислить данные для заполнения сводной таблицы
            pivotTable.CalculateData();

            // Сохраните книгу перед редактированием
            workbook.Save("PivotTableBeforeEdit.xlsx");

            // Теперь мы можем редактировать значения данных непосредственно в сводной таблице
            // Для демонстрации мы изменим ячейку в области данных
            Cell dataCell = worksheet.Cells["F5"]; // Assuming this is a data cell
            if (dataCell != null)
            {
                dataCell.PutValue(2500); // Modify the value
            }

            // Сохранить рабочую книгу после редактирования
            workbook.Save("PivotTableAfterEdit.xlsx");

            // Отключить редактирование значений данных
            pivotTable.EnableDataValueEditing = false;
            Console.WriteLine("EnableDataValueEditing set to: " + pivotTable.EnableDataValueEditing);
        }
    }
}
```

### См. также

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


