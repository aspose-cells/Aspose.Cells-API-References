---
title: "Cells.Subtotal"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Cells. Создаёт промежуточные итоги для диапазона"
type: docs
url: /ru/net/aspose.cells/cells/subtotal/
---
## Subtotal(CellArea, int, ConsolidationFunction, int[]) {#subtotal}

Создаёт промежуточные итоги для диапазона.

```csharp
public void Subtotal(CellArea ca, int groupBy, ConsolidationFunction function, int[] totalList)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| ca | CellArea | Диапазон |
| groupBy | Int32 | Поле для группировки, как целочисленное смещение, начинающееся с нуля |
| функция | ConsolidationFunction | Функция промежуточного итога. |
| totalList | Int32[] | Массив смещений полей, начинающихся с нуля, указывающий поля, к которым добавляются промежуточные итоги. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsMethodSubtotalWithCellAreaInt32ConsolidationFuncDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Заполнить примерные данные для подсчёта промежуточных итогов
            CreateSampleData(worksheet);

            // Определить область ячеек, содержащую данные (A1:C6)
            CellArea cellArea = CellArea.CreateCellArea(0, 0, 5, 2);

            try
            {
                // Вызвать метод Subtotal с параметрами:
                // - Группировать по столбцу 0 (Region)
                // - Использовать функцию SUM
                // - Применить к столбцу 2 (Sales)
                worksheet.Cells.Subtotal(
                    cellArea,
                    0,
                    ConsolidationFunction.Sum,
                    new int[] { 2 }
                );

                Console.WriteLine("Subtotal added successfully for parameters (CellArea, 0, Sum, [2])");
                
                // Методы ExpandColumnLevel и ExpandRowLevel были удалены, чтобы исправить ошибки компиляции
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Subtotal method: {ex.Message}");
            }

            // Сохранить результат
            workbook.Save("CellsMethodSubtotalWithCellAreaInt32ConsolidationFuncDemo.xlsx");
        }

        private static void CreateSampleData(Worksheet worksheet)
        {
            // Создать строку заголовка
            worksheet.Cells["A1"].PutValue("Region");
            worksheet.Cells["B1"].PutValue("Product");
            worksheet.Cells["C1"].PutValue("Sales");

            // Создать строки данных
            object[,] data = new object[,] {
                {"North", "Widget", 5000},
                {"North", "Gadget", 3000},
                {"South", "Widget", 6000},
                {"South", "Gadget", 4000},
                {"West", "Widget", 4500}
            };

            // Заполнить данные, начиная со строки 2 (нумерация с нуля, индекс 1)
            for (int i = 0; i < data.GetLength(0); i++)
            {
                worksheet.Cells[i + 1, 0].PutValue(data[i, 0]);
                worksheet.Cells[i + 1, 1].PutValue(data[i, 1]);
                worksheet.Cells[i + 1, 2].PutValue(data[i, 2]);
            }
        }
    }
}
```

### См. также

* struct [CellArea](../../cellarea/)
* enum [ConsolidationFunction](../../consolidationfunction/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Subtotal(CellArea, int, ConsolidationFunction, int[], bool, bool, bool) {#subtotal_1}

Создаёт промежуточные итоги для диапазона.

```csharp
public void Subtotal(CellArea ca, int groupBy, ConsolidationFunction function, int[] totalList, 
    bool replace, bool pageBreaks, bool summaryBelowData)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| ca | CellArea | Диапазон |
| groupBy | Int32 | Поле для группировки, как целочисленное смещение, начинающееся с нуля |
| функция | ConsolidationFunction | Функция промежуточного итога. |
| totalList | Int32[] | Массив смещений полей, начинающихся с нуля, указывающий поля, к которым добавляются промежуточные итоги. |
| заменить | Boolean | Указывает, следует ли заменять текущие промежуточные итоги |
| разрывы страниц | Boolean | Указывает, следует ли добавлять разрыв страницы между группами |
| summaryBelowData | Boolean | Указывает, следует ли добавить сводку ниже данных. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsMethodSubtotalWithCellAreaInt32ConsolidationFuncDemo1
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Создать примерные данные для расчёта промежуточных итогов
            cells["A1"].PutValue("Category");
            cells["B1"].PutValue("Product");
            cells["C1"].PutValue("Sales");
            
            object[,] data = new object[,] {
                { "Fruits", "Apple", 1500 },
                { "Fruits", "Orange", 2500 },
                { "Vegetables", "Carrot", 1800 },
                { "Vegetables", "Potato", 3000 },
                { "Fruits", "Banana", 2000 }
            };

            for (int row = 0; row < 5; row++)
            {
                for (int col = 0; col < 3; col++)
                {
                    cells[row + 1, col].PutValue(data[row, col]);
                }
            }

            try
            {
                // Определить область ячеек для промежуточного итога (A1:C6)
                CellArea area = new CellArea();
                area.StartRow = 0;
                area.StartColumn = 0;
                area.EndRow = 5;
                area.EndColumn = 2;

                // Вызвать Subtotal с параметрами:
                // - Группировать по первому столбцу (нумерация с нуля, индекс 0)
                // - Использовать функцию Sum
                // - Применить к третьему столбцу (нумерация с нуля, индекс 2)
                // - Заменить существующие промежуточные итоги, разрывы страниц между группами, резюме под данными
                cells.Subtotal(
                    area,
                    0,
                    ConsolidationFunction.Sum,
                    new int[] { 2 },
                    true,
                    true,
                    true
                );

                Console.WriteLine("Subtotal added successfully for parameters: (CellArea, Int32, ConsolidationFunction, Int32[], Boolean, Boolean, Boolean)");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error creating subtotal: {ex.Message}");
            }

            workbook.Save("SubtotalDemo.xlsx");
        }
    }
}
```

### См. также

* struct [CellArea](../../cellarea/)
* enum [ConsolidationFunction](../../consolidationfunction/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


