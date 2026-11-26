---
title: "PivotTable.TableRange2"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство PivotTable. Возвращает объект CellArea, представляющий диапазон, содержащий весь отчет сводной таблицы, включая поля страниц. Только для чтения"
type: docs
url: /ru/net/aspose.cells.pivot/pivottable/tablerange2/
---
## PivotTable.TableRange2 property

Возвращает объект CellArea, представляющий диапазон, содержащий весь отчет PivotTable, включая поля страниц. Только для чтения.

```csharp
public CellArea TableRange2 { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyTableRange2Demo
    {
        public static void Run()
        {
            // Создать книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить примерные данные для сводной таблицы
            worksheet.Cells["A1"].Value = "Fruit";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["A3"].Value = "Orange";
            worksheet.Cells["A4"].Value = "Banana";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["B2"].Value = 1000;
            worksheet.Cells["B3"].Value = 2000;
            worksheet.Cells["B4"].Value = 3000;

            // Добавить сводную таблицу
            int index = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];

            // Добавить поля в сводную таблицу
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Вычислить данные
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // Получить TableRange2, который включает всю сводную таблицу
            CellArea tableRange2 = pivotTable.TableRange2;
            Console.WriteLine($"TableRange2: StartRow={tableRange2.StartRow}, StartColumn={tableRange2.StartColumn}, " +
                $"EndRow={tableRange2.EndRow}, EndColumn={tableRange2.EndColumn}");

            // Создать диапазон на основе TableRange2
            Aspose.Cells.Range pivotRange = worksheet.Cells.CreateRange(
                tableRange2.StartRow, 
                tableRange2.StartColumn, 
                tableRange2.EndRow - tableRange2.StartRow + 1, 
                tableRange2.EndColumn - tableRange2.StartColumn + 1);

            // Вывести адрес диапазона
            Console.WriteLine($"Pivot Table Range: {pivotRange.Address}");
        }
    }
}
```

### См. также

* struct [CellArea](../../../aspose.cells/cellarea/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


