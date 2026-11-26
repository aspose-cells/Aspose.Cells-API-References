---
title: "CellsDataTableFactory.GetInstance"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод CellsDataTableFactory. Создает ICellsDataTable из заданной последовательности целочисленных значений"
type: docs
url: /ru/net/aspose.cells/cellsdatatablefactory/getinstance/
---
## GetInstance(int[], string[]) {#getinstance_5}

Создаёт ICellsDataTable из заданной последовательности целочисленных значений.

```csharp
public ICellsDataTable GetInstance(int[] vals, string[] columnNames)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| vals | Int32[] | целочисленные значения для построения таблицы |
| columnNames | String[] | Имена столбцов таблицы. Их длина может быть только 1 (построить таблицу по целочисленным значениям вертикально) или равна длине целочисленных значений (построить таблицу по целочисленным значениям горизонтально) |

### Возвращаемое значение

Экземпляр ICellsDataTable

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsDataTableFactoryMethodGetInstanceWithInt32StringDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Подготовьте данные для параметров метода (Int32[], String[])
            int[] values = new int[] { 100, 200, 300, 400, 500 };
            string[] columnNames = new string[] { "Column1", "Column2", "Column3", "Column4", "Column5" };

            try
            {
                // Создайте экземпляр CellsDataTableFactory с помощью рефлексии
                CellsDataTableFactory factory = (CellsDataTableFactory)Activator.CreateInstance(typeof(CellsDataTableFactory), nonPublic: true);
                
                // Вызовите GetInstance с параметрами (Int32[], String[])
                ICellsDataTable dataTable = factory.GetInstance(values, columnNames);

                // Выведите данные на лист
                worksheet.Cells.ImportData(dataTable, 0, 0, new ImportTableOptions());

                // Отобразите некоторую информацию о созданной таблице
                Console.WriteLine("Method executed successfully with parameters (Int32[], String[])");
                Console.WriteLine($"Created table with {dataTable.Count} rows and {dataTable.Columns.Length} columns");
                
                // Выведите имена столбцов
                Console.WriteLine("Column Names:");
                foreach (string colName in dataTable.Columns)
                {
                    Console.WriteLine(colName);
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetInstance method: {ex.Message}");
            }
            
            // Сохранить результат
            workbook.Save("CellsDataTableFactoryGetInstanceWithInt32StringDemo.xlsx");
        }
    }
}
```

### См. также

* interface [ICellsDataTable](../../icellsdatatable/)
* class [CellsDataTableFactory](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetInstance(int[], bool) {#getinstance_4}

Создаёт ICellsDataTable из заданной последовательности целочисленных значений.

```csharp
public ICellsDataTable GetInstance(int[] vals, bool vertial)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| vals | Int32[] | целочисленные значения для построения таблицы |
| vertial | Boolean | определяет, строить таблицу по целочисленным значениям вертикально (true) или горизонтально (false) |

### Возвращаемое значение

Экземпляр ICellsDataTable

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsDataTableFactoryMethodGetInstanceWithInt32ArrayBooleanDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Подготовьте данные для параметров метода (Int32[], Boolean)
            int[] values = new int[] { 10, 20, 30, 40, 50 };
            bool vertical = true;

            try
            {
                // Создайте экземпляр CellsDataTableFactory
                CellsDataTableFactory factory = (CellsDataTableFactory)Activator.CreateInstance(typeof(CellsDataTableFactory), nonPublic: true);
                
                // Вызовите GetInstance с параметрами (Int32[], Boolean)
                ICellsDataTable dataTable = factory.GetInstance(values, vertical);

                // Выведите данные на лист
                int row = 0;
                dataTable.BeforeFirst();
                while (dataTable.Next())
                {
                    for (int col = 0; col < dataTable.Columns.Length; col++)
                    {
                        worksheet.Cells[row, col].PutValue(dataTable[col]);
                    }
                    row++;
                }

                Console.WriteLine("Data table created successfully from Int32[] with vertical orientation");
                Console.WriteLine($"Total rows processed: {row}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetInstance method: {ex.Message}");
            }
            
            // Сохранить результат
            workbook.Save("CellsDataTableFactoryGetInstanceWithInt32ArrayBooleanDemo.xlsx");
        }
    }
}
```

### См. также

* interface [ICellsDataTable](../../icellsdatatable/)
* class [CellsDataTableFactory](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetInstance(double[], string[]) {#getinstance_2}

Создаёт ICellsDataTable из заданной последовательности значений double.

```csharp
public ICellsDataTable GetInstance(double[] vals, string[] columnNames)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| vals | Double[] | значения double для построения таблицы |
| columnNames | String[] | Имена столбцов таблицы. Его длина может быть только 1 (построить таблицу по значениям double вертикально) или длина значений double (построить таблицу по значениям double горизонтально) |

### Возвращаемое значение

Экземпляр ICellsDataTable

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsDataTableFactoryMethodGetInstanceWithDoubleStringDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Подготовьте данные для параметров метода (Double[], String[])
            double[] values = new double[] { 10.5, 20.25, 30.75, 40.1, 50.9 };
            string[] columnNames = new string[] { "Price", "Cost", "Margin", "Tax", "Total" };

            try
            {
                // Создайте экземпляр CellsDataTableFactory
                CellsDataTableFactory factory = (CellsDataTableFactory)Activator.CreateInstance(typeof(CellsDataTableFactory), nonPublic: true);
                
                // Вызовите GetInstance с параметрами (Double[], String[])
                ICellsDataTable dataTable = factory.GetInstance(values, columnNames);

                // Выведите данные на лист
                worksheet.Cells.ImportData(dataTable, 0, 0, new ImportTableOptions());

                // Отобразите информацию о созданной таблице
                Console.WriteLine("Method executed successfully with parameters (Double[], String[])");
                Console.WriteLine($"Created table with {dataTable.Count} rows and {dataTable.Columns.Length} columns");
                
                // Выведите имена столбцов и значения
                Console.WriteLine("Column Names:");
                foreach (string colName in dataTable.Columns)
                {
                    Console.WriteLine(colName);
                }

                // Выведите значения
                dataTable.BeforeFirst();
                while (dataTable.Next())
                {
                    for (int i = 0; i < dataTable.Columns.Length; i++)
                    {
                        Console.WriteLine($"{dataTable.Columns[i]}: {dataTable[i]}");
                    }
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetInstance method: {ex.Message}");
            }
            
            // Сохранить результат
            workbook.Save("CellsDataTableFactoryGetInstanceWithDoubleStringDemo.xlsx");
        }
    }
}
```

### См. также

* interface [ICellsDataTable](../../icellsdatatable/)
* class [CellsDataTableFactory](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetInstance(double[], bool) {#getinstance_1}

Создаёт ICellsDataTable из заданной последовательности значений double.

```csharp
public ICellsDataTable GetInstance(double[] vals, bool vertial)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| vals | Double[] | значения double для построения таблицы |
| vertial | Boolean | построить таблицу по значениям double вертикально (true) или горизонтально (false) |

### Возвращаемое значение

Экземпляр ICellsDataTable

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsDataTableFactoryMethodGetInstanceWithDoubleBooleanDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Подготовьте данные для параметров метода (Double[], Boolean)
            double[] values = new double[] { 10.5, 20.25, 30.75, 40.1, 50.9 };
            bool vertical = true;

            try
            {
                // Создайте экземпляр CellsDataTableFactory
                CellsDataTableFactory factory = (CellsDataTableFactory)Activator.CreateInstance(typeof(CellsDataTableFactory), nonPublic: true);
                
                // Вызовите GetInstance с параметрами (Double[], Boolean)
                ICellsDataTable dataTable = factory.GetInstance(values, vertical);

                // Выведите данные на лист
                int row = 0;
                dataTable.BeforeFirst();
                while (dataTable.Next())
                {
                    for (int col = 0; col < dataTable.Columns.Length; col++)
                    {
                        worksheet.Cells[row, col].PutValue(dataTable[col]);
                    }
                    row++;
                }

                Console.WriteLine("Data table created successfully with parameters (Double[], Boolean)");
                Console.WriteLine($"Total rows processed: {row}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetInstance method: {ex.Message}");
            }
            
            // Сохранить результат
            workbook.Save("CellsDataTableFactoryGetInstanceWithDoubleBooleanDemo.xlsx");
        }
    }
}
```

### См. также

* interface [ICellsDataTable](../../icellsdatatable/)
* class [CellsDataTableFactory](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetInstance(object[], string[]) {#getinstance_10}

Создаёт ICellsDataTable из заданной последовательности объектов.

```csharp
public ICellsDataTable GetInstance(object[] vals, string[] columnNames)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| vals | Object[] | объекты для построения таблицы |
| columnNames | String[] | Имена столбцов таблицы. Его длина может быть только 1 (построить таблицу по объектам вертикально) или длина объектов (построить таблицу по объектам горизонтально) |

### Возвращаемое значение

Экземпляр ICellsDataTable

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsDataTableFactoryMethodGetInstanceWithObjectStringDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Подготовьте данные для параметров метода (Object[], String[])
            object[] values = new object[] { "John Doe", 35, 75000.50, DateTime.Now };
            string[] columnNames = new string[] { "Name", "Age", "Salary", "Hire Date" };

            try
            {
                // Создайте экземпляр CellsDataTableFactory с помощью рефлексии
                CellsDataTableFactory factory = (CellsDataTableFactory)Activator.CreateInstance(typeof(CellsDataTableFactory), nonPublic: true);
                
                // Вызовите метод GetInstance с параметрами (Object[], String[])
                ICellsDataTable dataTable = factory.GetInstance(values, columnNames);

                // Выведите данные на лист, используя ImportData вместо ImportDataTable
                worksheet.Cells.ImportData(dataTable, 0, 0, new ImportTableOptions());

                Console.WriteLine("Method executed successfully with parameters (Object[], String[])");
                Console.WriteLine($"Created table with {dataTable.Count} rows and {dataTable.Columns.Length} columns");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetInstance method: {ex.Message}");
            }
            
            // Сохранить результат
            workbook.Save("CellsDataTableFactoryGetInstanceWithObjectStringDemo.xlsx");
        }
    }
}
```

### См. также

* interface [ICellsDataTable](../../icellsdatatable/)
* class [CellsDataTableFactory](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetInstance(object[][], bool, string[]) {#getinstance_11}

Создаёт ICellsDataTable из заданной последовательности объектов.

```csharp
public ICellsDataTable GetInstance(object[][] vals, bool hasHeader, string[] columnNames)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| vals | Object[][] | объекты для построения таблицы |
| hasHeader | Boolean | Указывает, является ли первая строка строкой заголовка. |
| columnNames | String[] | Имена столбцов таблицы. Его длина может быть только 1 (построить таблицу по объектам вертикально) или длина объектов (построить таблицу по объектам горизонтально) |

### Возвращаемое значение

Экземпляр ICellsDataTable

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsDataTableFactoryMethodGetInstanceWithObjectBooleanStringDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Подготовьте данные для параметров метода (Object[][], Boolean, String[])
            object[][] data = new object[][]
            {
                new object[] { "ID", "Name", "Price" },
                new object[] { 1, "Laptop", 999.99 },
                new object[] { 2, "Phone", 699.99 },
                new object[] { 3, "Tablet", 399.99 }
            };

            bool hasHeader = true;
            string[] columnNames = new string[] { "ProductID", "ProductName", "ProductPrice" };

            try
            {
                // Создайте экземпляр CellsDataTableFactory
                CellsDataTableFactory factory = (CellsDataTableFactory)Activator.CreateInstance(typeof(CellsDataTableFactory), nonPublic: true);
                
                // Вызовите GetInstance с параметрами (Object[][], Boolean, String[])
                ICellsDataTable dataTable = factory.GetInstance(data, hasHeader, columnNames);

                // Выведите данные на лист
                int row = 0;
                dataTable.BeforeFirst();
                while (dataTable.Next())
                {
                    for (int col = 0; col < dataTable.Columns.Length; col++)
                    {
                        worksheet.Cells[row, col].PutValue(dataTable[col]);
                    }
                    row++;
                }

                Console.WriteLine("Data table created successfully with parameters (Object[][], Boolean, String[])");
                Console.WriteLine($"Total rows processed: {row}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetInstance method: {ex.Message}");
            }
            
            // Сохранить результат
            workbook.Save("CellsDataTableFactoryGetInstanceWithObjectBooleanStringDemo.xlsx");
        }
    }
}
```

### См. также

* interface [ICellsDataTable](../../icellsdatatable/)
* class [CellsDataTableFactory](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetInstance(object[], bool) {#getinstance_9}

Создаёт ICellsDataTable из заданной последовательности объектов.

```csharp
public ICellsDataTable GetInstance(object[] vals, bool vertial)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| vals | Object[] | объекты для построения таблицы |
| vertial | Boolean | построить таблицу по объектам вертикально (true) или горизонтально (false) |

### Возвращаемое значение

Экземпляр ICellsDataTable

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsDataTableFactoryMethodGetInstanceWithObjectBooleanDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Подготовьте данные для параметров метода (Object[], Boolean)
            object[] data = new object[] { "Product", "Price", "Stock", "Available" };
            bool vertical = true;

            try
            {
                // Создайте экземпляр CellsDataTableFactory с помощью рефлексии
                CellsDataTableFactory factory = (CellsDataTableFactory)Activator.CreateInstance(typeof(CellsDataTableFactory), nonPublic: true);
                
                // Вызовите GetInstance с параметрами (Object[], Boolean)
                ICellsDataTable dataTable = factory.GetInstance(data, vertical);

                // Выведите данные на лист
                dataTable.BeforeFirst();
                int row = 0;
                while (dataTable.Next())
                {
                    for (int col = 0; col < dataTable.Columns.Length; col++)
                    {
                        worksheet.Cells[row, col].PutValue(dataTable[col]);
                    }
                    row++;
                }

                Console.WriteLine("Data table created successfully with parameters (Object[], Boolean)");
                Console.WriteLine($"Data orientation: {(vertical ? "Vertical" : "Horizontal")}");
                Console.WriteLine($"Total items processed: {dataTable.Count}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetInstance method: {ex.Message}");
            }
            
            // Сохранить результат
            workbook.Save("CellsDataTableFactoryGetInstanceWithObjectBooleanDemo.xlsx");
        }
    }
}
```

### См. также

* interface [ICellsDataTable](../../icellsdatatable/)
* class [CellsDataTableFactory](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetInstance(int[]) {#getinstance_3}

```csharp
public ICellsDataTable GetInstance(int[] vals)
```

### См. также

* interface [ICellsDataTable](../../icellsdatatable/)
* class [CellsDataTableFactory](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetInstance(double[]) {#getinstance}

```csharp
public ICellsDataTable GetInstance(double[] vals)
```

### См. также

* interface [ICellsDataTable](../../icellsdatatable/)
* class [CellsDataTableFactory](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetInstance(object[]) {#getinstance_8}

```csharp
public ICellsDataTable GetInstance(object[] vals)
```

### См. также

* interface [ICellsDataTable](../../icellsdatatable/)
* class [CellsDataTableFactory](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetInstance(ICollection) {#getinstance_6}

Создаёт ICellsDataTable из заданной коллекции.

```csharp
public ICellsDataTable GetInstance(ICollection collection)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| коллекция | ICollection | коллекция для построения таблицы |

### Возвращаемое значение

Экземпляр ICellsDataTable

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Collections;

    public class CellsDataTableFactoryMethodGetInstanceWithICollectionDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Подготовьте ArrayList как ICollection
            ArrayList data = new ArrayList
            {
                new ArrayList { "Product", "Price", "Stock" },
                new ArrayList { "Keyboard", 49.99, 120 },
                new ArrayList { "Mouse", 29.99, 200 },
                new ArrayList { "Monitor", 199.99, 35 }
            };

            try
            {
                // Создайте экземпляр CellsDataTableFactory
                CellsDataTableFactory factory = (CellsDataTableFactory)Activator.CreateInstance(typeof(CellsDataTableFactory), nonPublic: true);
                
                // Вызовите GetInstance с параметром ICollection
                ICellsDataTable dataTable = factory.GetInstance(data);

                // Выведите данные на лист
                int row = 0;
                dataTable.BeforeFirst();
                while (dataTable.Next())
                {
                    for (int col = 0; col < dataTable.Columns.Length; col++)
                    {
                        worksheet.Cells[row, col].PutValue(dataTable[col]);
                    }
                    row++;
                }

                Console.WriteLine("Data table created successfully from ICollection");
                Console.WriteLine($"Total rows processed: {row}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetInstance method: {ex.Message}");
            }
            
            // Сохранить результат
            workbook.Save("CellsDataTableFactoryGetInstanceWithICollectionDemo.xlsx");
        }
    }
}
```

### См. также

* interface [ICellsDataTable](../../icellsdatatable/)
* class [CellsDataTableFactory](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetInstance(ICollection, bool) {#getinstance_7}

Создаёт ICellsDataTable из заданной коллекции.

```csharp
public ICellsDataTable GetInstance(ICollection collection, bool hasHeader)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| коллекция | ICollection | коллекция для построения таблицы |
| hasHeader | Boolean | Указывает, является ли первая строка заголовком |

### Возвращаемое значение

Экземпляр ICellsDataTable

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Collections;

    public class CellsDataTableFactoryMethodGetInstanceWithICollectionBooleanDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Подготовьте коллекцию данных для параметров метода (ICollection, Boolean)
            ArrayList dataCollection = new ArrayList
            {
                new { Product = "Apple", Price = 2.5, Stock = 100 },
                new { Product = "Orange", Price = 1.8, Stock = 150 },
                new { Product = "Banana", Price = 0.9, Stock = 200 }
            };
            bool hasHeader = true;

            try
            {
                // Создайте экземпляр CellsDataTableFactory
                CellsDataTableFactory factory = (CellsDataTableFactory)Activator.CreateInstance(typeof(CellsDataTableFactory), nonPublic: true);
                
                // Вызовите GetInstance с параметрами (ICollection, Boolean)
                ICellsDataTable dataTable = factory.GetInstance(dataCollection, hasHeader);

                // Выведите данные на лист
                worksheet.Cells.ImportData(dataTable, 0, 0, new ImportTableOptions());

                // Отобразите информацию о созданной таблице
                Console.WriteLine("Method executed successfully with parameters (ICollection, Boolean)");
                Console.WriteLine($"Created table with {dataTable.Count} rows and {dataTable.Columns.Length} columns");
                
                // Выведите имена столбцов
                Console.WriteLine("Column Names:");
                foreach (string colName in dataTable.Columns)
                {
                    Console.WriteLine(colName);
                }

                // Выведите значения
                dataTable.BeforeFirst();
                while (dataTable.Next())
                {
                    for (int i = 0; i < dataTable.Columns.Length; i++)
                    {
                        Console.WriteLine($"{dataTable.Columns[i]}: {dataTable[i]}");
                    }
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetInstance method: {ex.Message}");
            }
            
            // Сохранить результат
            workbook.Save("CellsDataTableFactoryGetInstanceWithICollectionBooleanDemo.xlsx");
        }
    }
}
```

### См. также

* interface [ICellsDataTable](../../icellsdatatable/)
* class [CellsDataTableFactory](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


