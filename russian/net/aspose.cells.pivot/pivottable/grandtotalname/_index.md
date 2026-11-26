---
title: "PivotTable.GrandTotalName"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство PivotTable. Возвращает метку, отображаемую в заголовке столбца или строки итоговой суммы. Значение по умолчанию — строка Grand Total"
type: docs
url: /ru/net/aspose.cells.pivot/pivottable/grandtotalname/
---
## PivotTable.GrandTotalName property

Возвращает метку, отображаемую в заголовке столбца или строки общей суммы. Значение по умолчанию — строка "Grand Total".

```csharp
public string GrandTotalName { get; set; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotTablePropertyGrandTotalNameDemo
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
            
            worksheet.Cells["A2"].Value = "Laptop";
            worksheet.Cells["B2"].Value = "North";
            worksheet.Cells["C2"].Value = 1000;
            
            worksheet.Cells["A3"].Value = "Laptop";
            worksheet.Cells["B3"].Value = "South";
            worksheet.Cells["C3"].Value = 1500;
            
            worksheet.Cells["A4"].Value = "Phone";
            worksheet.Cells["B4"].Value = "North";
            worksheet.Cells["C4"].Value = 800;
            
            worksheet.Cells["A5"].Value = "Phone";
            worksheet.Cells["B5"].Value = "South";
            worksheet.Cells["C5"].Value = 1200;

            // Создайте сводную таблицу
            PivotTableCollection pivotTables = worksheet.PivotTables;
            int index = pivotTables.Add("A1:C5", "E3", "PivotTable1");
            PivotTable pivotTable = pivotTables[index];

            // Добавьте строки и поля данных
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Отобразить текущее значение GrandTotalName
            Console.WriteLine("Current GrandTotalName: " + pivotTable.GrandTotalName);

            // Изменить GrandTotalName
            pivotTable.GrandTotalName = "Total Summary";

            // Вычислить данные и обновить сводную таблицу
            pivotTable.CalculateData();
            pivotTable.RefreshData();

            // Сохраните книгу
            workbook.Save("PivotTableGrandTotalNameDemo.xlsx");
        }
    }
}
```

### См. также

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


