---
title: "PivotTable.Format"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод PivotTable. Форматирует выбранную область PivotTable"
type: docs
url: /ru/net/aspose.cells.pivot/pivottable/format/
---
## Format(PivotArea, Style) {#format_1}

Форматирует выбранную область сводной таблицы.

```csharp
public void Format(PivotArea pivotArea, Style style)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| pivotArea | PivotArea | Выбранная область просмотра pivot. |
| стиль | Стиль | Отформатированная настройка. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;
    using System.Drawing;

    public class PivotTableMethodFormatWithPivotAreaStyleDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте образцовые данные для сводной таблицы
            worksheet.Cells["A1"].Value = "Product";
            worksheet.Cells["A2"].Value = "Bike";
            worksheet.Cells["A3"].Value = "Car";
            worksheet.Cells["A4"].Value = "Truck";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["B2"].Value = 5000;
            worksheet.Cells["B3"].Value = 12000;
            worksheet.Cells["B4"].Value = 8000;

            // Создайте сводную таблицу
            int pivotIndex = worksheet.PivotTables.Add("A1:B4", "D3", "SalesPivot");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // Добавьте поля в сводную таблицу
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Вычислить данные для заполнения сводной таблицы
            pivotTable.CalculateData();

            // Создать стиль для форматирования
            Style style = workbook.CreateStyle();
            style.Font.Name = "Arial";
            style.Font.Size = 12;
            style.Font.IsBold = true;
            style.ForegroundColor = Color.Yellow;
            style.Pattern = BackgroundType.Solid;

            // Создать область pivot для форматирования
            PivotArea pivotArea = new PivotArea(pivotTable);
            pivotArea.RuleType = PivotAreaType.Normal;
            pivotArea.AxisType = PivotFieldType.Data;

            try
            {
                // Применить форматирование к области pivot
                pivotTable.Format(pivotArea, style);
                
                Console.WriteLine("Format method executed successfully with parameters (PivotArea, Style)");
                
                // Сохраните книгу, чтобы показать эффект
                workbook.Save("PivotTableFormatWithPivotAreaStyleDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Format method: {ex.Message}");
            }
        }
    }
}
```

### См. также

* class [PivotArea](../../pivotarea/)
* class [Style](../../../aspose.cells/style/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## Format(CellArea, Style) {#format}

Форматирует выбранную область сводной таблицы.

```csharp
public void Format(CellArea ca, Style style)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| ca | CellArea | Диапазон ячеек. |
| стиль | Стиль | Стиль |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;
    using System.Drawing;

    public class PivotTableMethodFormatWithCellAreaStyleDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте образцовые данные для сводной таблицы
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Region");
            worksheet.Cells["C1"].PutValue("Sales");
            worksheet.Cells["A2"].PutValue("Product A");
            worksheet.Cells["B2"].PutValue("North");
            worksheet.Cells["C2"].PutValue(1000);
            worksheet.Cells["A3"].PutValue("Product B");
            worksheet.Cells["B3"].PutValue("South");
            worksheet.Cells["C3"].PutValue(2000);
            worksheet.Cells["A4"].PutValue("Product C");
            worksheet.Cells["B4"].PutValue("East");
            worksheet.Cells["C4"].PutValue(3000);

            // Создайте сводную таблицу
            int pivotIndex = worksheet.PivotTables.Add("A1:C4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            
            // Добавьте строки и поля данных
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Вычислить данные и диапазоны
            pivotTable.CalculateData();
            pivotTable.CalculateRange();

            // Создать стиль для форматирования
            Style style = workbook.CreateStyle();
            style.Font.Name = "Arial";
            style.Font.Size = 12;
            style.Font.IsBold = true;
            style.ForegroundColor = Color.Yellow;
            style.Pattern = BackgroundType.Solid;

            // Определить область ячеек для форматирования (диапазон тела данных)
            CellArea area = pivotTable.DataBodyRange;

            try
            {
                // Вызвать метод Format с параметрами CellArea и Style
                pivotTable.Format(area, style);
                
                Console.WriteLine("PivotTable formatted successfully with parameters (CellArea, Style)");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error formatting PivotTable: {ex.Message}");
            }
            
            // Сохранить результат
            workbook.Save("PivotTableFormatWithCellAreaStyleDemo.xlsx");
        }
    }
}
```

### См. также

* struct [CellArea](../../../aspose.cells/cellarea/)
* class [Style](../../../aspose.cells/style/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## Format(int, int, Style) {#format_2}

Форматирует ячейку в области сводной таблицы

```csharp
public void Format(int row, int column, Style style)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| строка | Int32 | Индекс строки ячейки |
| column | Int32 | Индекс столбца ячейки |
| стиль | Стиль | Стиль, который будет использоваться для форматирования ячейки |

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableMethodFormatWithInt32Int32StyleDemo
    {
        public static void Run()
        {
            // Создать книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить примерные данные для сводной таблицы
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(200);
            worksheet.Cells["A4"].PutValue("A");
            worksheet.Cells["B4"].PutValue(150);

            // Добавьте сводную таблицу
            int pivotIndex = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            
            // Добавить поля в область строк
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            
            // Вычислить данные
            pivotTable.CalculateData();

            // Создать стиль для форматирования
            Style style = workbook.CreateStyle();
            style.BackgroundColor = System.Drawing.Color.LightBlue;
            style.Font.IsBold = true;

            // Отформатировать ячейку заголовка сводной таблицы (строка 2, столбец 0 в координатах сводной таблицы)
            pivotTable.Format(2, 0, style);

            // Сохраните книгу
            workbook.Save("PivotTableFormatDemo.xlsx");
        }
    }
}
```

### См. также

* class [Style](../../../aspose.cells/style/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


