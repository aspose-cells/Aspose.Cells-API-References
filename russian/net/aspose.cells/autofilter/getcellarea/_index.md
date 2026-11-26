---
title: "AutoFilter.GetCellArea"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод AutoFilter. Получает CellArea, к которому применяется данный AutoFilter"
type: docs
url: /ru/net/aspose.cells/autofilter/getcellarea/
---
## GetCellArea() {#getcellarea}

Получает [`CellArea`](../../cellarea/), к которому применяется данный AutoFilter.

```csharp
public CellArea GetCellArea()
```

### Возвращаемое значение

область, к которой применяется этот фильтр

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class AutoFilterMethodGetCellAreaDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Заполните примерными данными для демонстрации AutoFilter
            cells["A1"].PutValue("Product");
            cells["B1"].PutValue("Category");
            cells["C1"].PutValue("Price");

            cells["A2"].PutValue("Apple");
            cells["B2"].PutValue("Fruit");
            cells["C2"].PutValue(2.5);

            cells["A3"].PutValue("Carrot");
            cells["B3"].PutValue("Vegetable");
            cells["C3"].PutValue(1.2);

            cells["A4"].PutValue("Banana");
            cells["B4"].PutValue("Fruit");
            cells["C4"].PutValue(3.1);

            // Примените AutoFilter к заголовкам (индекс строки 0), охватывающим столбцы A-C (0-2)
            AutoFilter autoFilter = worksheet.AutoFilter;
            autoFilter.SetRange(0, 0, 2);

            try
            {
                // Получить CellArea, где применён AutoFilter
                CellArea result = autoFilter.GetCellArea();

                // Вывести координаты диапазона AutoFilter
                Console.WriteLine("AutoFilter applied to cell area:");
                Console.WriteLine($"Start Row: {result.StartRow}");
                Console.WriteLine($"Start Column: {result.StartColumn}");
                Console.WriteLine($"End Row: {result.EndRow}");
                Console.WriteLine($"End Column: {result.EndColumn}");

                // Примените простой фильтр для демонстрации функциональности (необязательно)
                autoFilter.Filter(1, "Fruit"); // Filter "Category" column (index 1) for "Fruit"
                autoFilter.Refresh();
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetCellArea method: {ex.Message}");
            }

            // Сохраните книгу с применённым AutoFilter
            workbook.Save("AutoFilterMethodGetCellAreaDemo.xlsx");
        }
    }
}
```

### См. также

* struct [CellArea](../../cellarea/)
* class [AutoFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetCellArea(bool) {#getcellarea_1}

Получает [`CellArea`](../../cellarea/), к которому применяется указанный AutoFilter.

```csharp
public CellArea GetCellArea(bool refreshAppliedRange)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| refreshAppliedRange | Boolean | Определяет, следует ли обновлять применённый диапазон. Для применённого диапазона автофильтра последняя строка может измениться при изменении данных ячеек. Если этот флаг установлен в true, то последняя строка диапазона будет пересчитана в соответствии с текущими данными ячеек. |

### Возвращаемое значение

область, к которой применяется этот фильтр

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class AutoFilterMethodGetCellAreaWithBooleanDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Подготовьте примерные данные для AutoFilter
            worksheet.Cells["A1"].PutValue("Header");
            worksheet.Cells["A2"].PutValue("Data1");
            worksheet.Cells["A3"].PutValue("Data2");
            worksheet.Cells["A4"].PutValue("Data3");

            // Установите диапазон AutoFilter (строка 0‑3, столбец 0)
            worksheet.AutoFilter.SetRange(0, 0, 0);

            try
            {
                // Вызовите GetCellArea с параметром refreshAppliedRange=true
                CellArea result = worksheet.AutoFilter.GetCellArea(true);

                // Отобразите применённый диапазон AutoFilter
                Console.WriteLine($"AutoFilter Range: StartRow={result.StartRow}, " +
                    $"StartColumn={result.StartColumn}, EndRow={result.EndRow}, " +
                    $"EndColumn={result.EndColumn}");

                Console.WriteLine("GetCellArea method executed successfully with boolean parameter");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetCellArea: {ex.Message}");
            }

            // Сохранить изменённую книгу
            workbook.Save("AutoFilterMethodGetCellAreaWithBooleanDemo.xlsx");
        }
    }
}
```

### См. также

* struct [CellArea](../../cellarea/)
* class [AutoFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


