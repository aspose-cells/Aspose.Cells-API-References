---
title: "PivotTable.CalculateData"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод PivotTable. Вычисляет данные сводной таблицы в ячейки"
type: docs
url: /ru/net/aspose.cells.pivot/pivottable/calculatedata/
---
## CalculateData() {#calculatedata_1}

Вычисляет данные сводной таблицы в ячейки.

```csharp
public void CalculateData()
```

### Примечания

Этот метод вычисляет данные только с использованием кэшированных данных в [`PivotCache`](../pivotcache/). Поэтому, если вы хотите вычислить данные с последнего источника, пожалуйста, используйте метод [`Refresh`](../../pivotcache/refresh/). Если изменены только настройки сводной таблицы, достаточно `CalculateData`.

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableMethodCalculateDataDemo
    {
        public static void Run()
        {
            // Создайте книгу с примерными данными
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавьте примерные данные
            worksheet.Cells["A1"].PutValue("Date");
            worksheet.Cells["B1"].PutValue("Sales");
            
            DateTime baseDate = new DateTime(2021, 11, 1);
            for (int i = 0; i < 15; i++)
            {
                worksheet.Cells[$"A{i+2}"].PutValue(baseDate.AddDays(i));
                worksheet.Cells[$"B{i+2}"].PutValue(100 + i * 10);
            }

            // Создать сводную таблицу — исправлено за счёт обеспечения правильных параметров
            int pivotIndex = worksheet.PivotTables.Add("A1:B16", "D3", "PivotTable");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            
            // Добавить поля в сводную таблицу
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Date");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            
            // Применить фильтр даты
            PivotField dateField = pivotTable.RowFields[0];
            dateField.FilterByDate(PivotFilterType.November, new DateTime(2021, 1, 1), new DateTime(2021, 12, 31));
            
            // Вычислить данные сводной таблицы
            pivotTable.RefreshData();
            pivotTable.CalculateData();
            
            // Сохраните книгу
            workbook.Save("PivotTableCalculateDataDemo.xlsx");
        }
    }
}
```

### См. также

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## CalculateData(PivotTableCalculateOption) {#calculatedata}

Вычисляет сводную таблицу с параметрами.

```csharp
public PivotTable[] CalculateData(PivotTableCalculateOption option)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| опция | PivotTableCalculateOption | Параметры расчёта сводной таблицы |

### Возвращаемое значение

Возвращает все сводные таблицы, которые были рассчитаны. Если [`RefreshData`](../../pivottablecalculateoption/refreshdata/) равно true, все сводные таблицы, основанные на одном и том же кэше, будут рассчитаны вместе.

### Примечания

Если [`RefreshData`](../../pivottablecalculateoption/refreshdata/) равно true, этот метод обновит кэш сводной таблицы из источника данных, а затем вычислит все сводные таблицы, основанные на этом кэше. В противном случае будет использоваться только кэшированные данные в кэше сводной таблицы.

### Примеры

```csharp
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableMethodCalculateDataWithPivotTableCalculateOptionDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Пример данных
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Создать сводную таблицу
            int pivotIndex = worksheet.PivotTables.Add("A1:B4", "D1", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // Настройте сводную таблицу
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Category");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Value");

            // Установите параметры расчёта
            PivotTableCalculateOption options = new PivotTableCalculateOption
            {
                RefreshData = true,
                ReserveMissingPivotItemType = ReserveMissingPivotItemType.All
            };

            // Вычислить с параметрами
            pivotTable.CalculateData(options);

            workbook.Save("PivotTableCalculateDataDemo.xlsx");
        }
    }
}
```

### См. также

* class [PivotTableCalculateOption](../../pivottablecalculateoption/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


