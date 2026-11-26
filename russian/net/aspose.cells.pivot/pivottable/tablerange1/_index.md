---
title: "PivotTable.TableRange1"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство PivotTable. Возвращает объект CellArea, представляющий диапазон, содержащий весь отчет PivotTable, но не включающий поля страниц. Только для чтения."
type: docs
url: /ru/net/aspose.cells.pivot/pivottable/tablerange1/
---
## PivotTable.TableRange1 property

Возвращает объект CellArea, представляющий диапазон, содержащий весь отчет PivotTable, но без полей страниц. Только для чтения.

```csharp
public CellArea TableRange1 { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyTableRange1Demo
    {
        public static void Run()
        {
            // Создать книгу
            Workbook workbook = new Workbook();
            
            // Добавить лист с образцовыми данными
            Worksheet dataSheet = workbook.Worksheets[0];
            dataSheet.Name = "Data";
            dataSheet.Cells["A1"].PutValue("Label");
            dataSheet.Cells["B1"].PutValue("Value");
            dataSheet.Cells["A2"].PutValue("A");
            dataSheet.Cells["B2"].PutValue(10);
            dataSheet.Cells["A3"].PutValue("B");
            dataSheet.Cells["B3"].PutValue(20);

            // Создайте сводную таблицу
            Worksheet pivotSheet = workbook.Worksheets.Add("Pivot");
            int pivotTableIndex = pivotSheet.PivotTables.Add("=Data!A1:B3", "A1", "PivotTable1");
            PivotTable pivotTable = pivotSheet.PivotTables[pivotTableIndex];
            
            // Добавить поля в сводную таблицу
            int labelFieldIndex = pivotTable.AddFieldToArea(PivotFieldType.Row, "Label");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Value");
            
            // Настройте сводную таблицу
            pivotTable.ShowInTabularForm();
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // Продемонстрировать свойство TableRange1
            Console.WriteLine("Pivot Table Range:");
            Console.WriteLine($"Start Row: {pivotTable.TableRange1.StartRow}");
            Console.WriteLine($"End Row: {pivotTable.TableRange1.EndRow}");
            Console.WriteLine($"Start Column: {pivotTable.TableRange1.StartColumn}");
            Console.WriteLine($"End Column: {pivotTable.TableRange1.EndColumn}");

            // Сохраните книгу
            workbook.Save("PivotTablePropertyTableRange1Demo.xlsx");
        }
    }
}
```

### См. также

* struct [CellArea](../../../aspose.cells/cellarea/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


