---
title: "ICellsDataTable.Item"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ICellsDataTable. Возвращает данные, хранящиеся в столбце, указанном по индексу"
type: docs
url: /ru/net/aspose.cells/icellsdatatable/item/
---
## ICellsDataTable indexer (1 of 2)

Возвращает данные, хранящиеся в столбце, указанном по индексу.

```csharp
public object this[int columnIndex] { get; }
```

| Параметр | Описание |
| --- | --- |
| columnIndex | Нулевой (начинающийся с нуля) индекс столбца. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ICellsDataTablePropertyItemDemo
    {
        public static void Run()
        {
            // Создать пользовательский ICellsDataTable с образцовыми данными
            ICellsDataTable dataTable = new SampleDataTable();

            // Сбросить позицию курсора
            dataTable.BeforeFirst();

            Console.WriteLine("Reading data using Item property:");
            while (dataTable.Next())
            {
                // Получить значения по индексу столбца
                Console.WriteLine($"Product: {dataTable[0]}, Price: {dataTable[1]}, Stock: {dataTable[2]}");

                // Получить значения по имени столбца
                Console.WriteLine($"Product: {dataTable["Product"]}, Price: {dataTable["Price"]}, Stock: {dataTable["Stock"]}\n");
            }
        }
    }

    internal class SampleDataTable : ICellsDataTable
    {
        private readonly string[] columns = { "Product", "Price", "Stock" };
        private readonly object[][] data = 
        {
            new object[] { "Laptop", 999.99, 15 },
            new object[] { "Phone", 699.99, 25 },
            new object[] { "Tablet", 299.99, 50 }
        };
        private int currentRow = -1;

        public string[] Columns => columns;
        public int Count => data.Length;

        public object this[int columnIndex] => data[currentRow][columnIndex];
        public object this[string columnName] => data[currentRow][Array.IndexOf(columns, columnName)];

        public void BeforeFirst() => currentRow = -1;
        public bool Next() => ++currentRow < data.Length;
    }
}
```

### См. также

* interface [ICellsDataTable](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## ICellsDataTable indexer (2 of 2)

Возвращает данные, хранящиеся в столбце, указанном по имени столбца.

```csharp
public object this[string columnName] { get; }
```

| Параметр | Описание |
| --- | --- |
| columnName | Имя столбца. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ICellsDataTablePropertyItemDemo1
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Заполнить ячейки образцовыми данными
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Price");
            worksheet.Cells["A2"].PutValue("Laptop");
            worksheet.Cells["B2"].PutValue(999.99);
            worksheet.Cells["A3"].PutValue("Phone");
            worksheet.Cells["B3"].PutValue(499.99);

            // Экспортировать диапазон данных в ICellsDataTable с явным приведением типов
            ICellsDataTable dataTable = (ICellsDataTable)worksheet.Cells.ExportDataTable(0, 0, 3, 2);

            // Перейти к позиции перед первой записью
            dataTable.BeforeFirst();

            Console.WriteLine("Reading data table values:");
            while (dataTable.Next())
            {
                // Получить свойство Item, используя имена столбцов (индексатор)
                string product = dataTable["Product"].ToString();
                double price = Convert.ToDouble(dataTable["Price"]);

                Console.WriteLine($"Item[Product]: {product}, Item[Price]: {price}");
            }

            // Сохраните книгу
            workbook.Save("ItemPropertyDemo.xlsx");
        }
    }
}
```

### См. также

* interface [ICellsDataTable](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


