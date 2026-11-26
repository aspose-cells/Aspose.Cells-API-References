---
title: "CellsDataTableFactory.GetInstance"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método CellsDataTableFactory. Crea ICellsDataTable a partir de la secuencia dada de valores enteros"
type: docs
url: /es/net/aspose.cells/cellsdatatablefactory/getinstance/
---
## GetInstance(int[], string[]) {#getinstance_5}

Crea ICellsDataTable a partir de la secuencia dada de valores enteros.

```csharp
public ICellsDataTable GetInstance(int[] vals, string[] columnNames)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| vals | Int32[] | valores int para construir la tabla |
| columnNames | String[] | Nombres de columna de la tabla. Su longitud solo puede ser 1 (construir tabla por los valores int verticalmente) o la longitud de los valores int (construir tabla por los valores int horizontalmente) |

### Valor de retorno

Instancia de ICellsDataTable

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsDataTableFactoryMethodGetInstanceWithInt32StringDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Preparar datos para los parámetros del método (Int32[], String[])
            int[] values = new int[] { 100, 200, 300, 400, 500 };
            string[] columnNames = new string[] { "Column1", "Column2", "Column3", "Column4", "Column5" };

            try
            {
                // Crear instancia de CellsDataTableFactory usando reflexión
                CellsDataTableFactory factory = (CellsDataTableFactory)Activator.CreateInstance(typeof(CellsDataTableFactory), nonPublic: true);
                
                // Llamar a GetInstance con parámetros (Int32[], String[])
                ICellsDataTable dataTable = factory.GetInstance(values, columnNames);

                // Exportar los datos a la hoja de cálculo
                worksheet.Cells.ImportData(dataTable, 0, 0, new ImportTableOptions());

                // Mostrar información sobre la tabla creada
                Console.WriteLine("Method executed successfully with parameters (Int32[], String[])");
                Console.WriteLine($"Created table with {dataTable.Count} rows and {dataTable.Columns.Length} columns");
                
                // Imprimir nombres de columna
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
            
            // Guardar el resultado
            workbook.Save("CellsDataTableFactoryGetInstanceWithInt32StringDemo.xlsx");
        }
    }
}
```

### Ver también

* interface [ICellsDataTable](../../icellsdatatable/)
* class [CellsDataTableFactory](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetInstance(int[], bool) {#getinstance_4}

Crea ICellsDataTable a partir de la secuencia dada de valores enteros.

```csharp
public ICellsDataTable GetInstance(int[] vals, bool vertial)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| vals | Int32[] | valores int para construir la tabla |
| vertical | Booleano | si se construye la tabla por los valores int verticalmente (true) o horizontalmente (false) |

### Valor de retorno

Instancia de ICellsDataTable

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsDataTableFactoryMethodGetInstanceWithInt32ArrayBooleanDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Preparar datos para los parámetros del método (Int32[], Boolean)
            int[] values = new int[] { 10, 20, 30, 40, 50 };
            bool vertical = true;

            try
            {
                // Crear instancia de CellsDataTableFactory
                CellsDataTableFactory factory = (CellsDataTableFactory)Activator.CreateInstance(typeof(CellsDataTableFactory), nonPublic: true);
                
                // Llamar a GetInstance con parámetros (Int32[], Boolean)
                ICellsDataTable dataTable = factory.GetInstance(values, vertical);

                // Exportar los datos a la hoja de cálculo
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
            
            // Guardar el resultado
            workbook.Save("CellsDataTableFactoryGetInstanceWithInt32ArrayBooleanDemo.xlsx");
        }
    }
}
```

### Ver también

* interface [ICellsDataTable](../../icellsdatatable/)
* class [CellsDataTableFactory](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetInstance(double[], string[]) {#getinstance_2}

Crea ICellsDataTable a partir de la secuencia dada de valores double.

```csharp
public ICellsDataTable GetInstance(double[] vals, string[] columnNames)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| vals | Double[] | valores double para construir la tabla |
| columnNames | String[] | Nombres de columna de la tabla. Su longitud solo puede ser 1(construir tabla con los valores dobles verticalmente) o la longitud de los valores dobles(construir tabla con los valores dobles horizontalmente) |

### Valor de retorno

Instancia de ICellsDataTable

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsDataTableFactoryMethodGetInstanceWithDoubleStringDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Preparar datos para los parámetros del método (Double[], String[])
            double[] values = new double[] { 10.5, 20.25, 30.75, 40.1, 50.9 };
            string[] columnNames = new string[] { "Price", "Cost", "Margin", "Tax", "Total" };

            try
            {
                // Crear instancia de CellsDataTableFactory
                CellsDataTableFactory factory = (CellsDataTableFactory)Activator.CreateInstance(typeof(CellsDataTableFactory), nonPublic: true);
                
                // Llamar a GetInstance con los parámetros (Double[], String[])
                ICellsDataTable dataTable = factory.GetInstance(values, columnNames);

                // Exportar los datos a la hoja de cálculo
                worksheet.Cells.ImportData(dataTable, 0, 0, new ImportTableOptions());

                // Mostrar información sobre la tabla creada
                Console.WriteLine("Method executed successfully with parameters (Double[], String[])");
                Console.WriteLine($"Created table with {dataTable.Count} rows and {dataTable.Columns.Length} columns");
                
                // Imprimir nombres de columna y valores
                Console.WriteLine("Column Names:");
                foreach (string colName in dataTable.Columns)
                {
                    Console.WriteLine(colName);
                }

                // Imprimir valores
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
            
            // Guardar el resultado
            workbook.Save("CellsDataTableFactoryGetInstanceWithDoubleStringDemo.xlsx");
        }
    }
}
```

### Ver también

* interface [ICellsDataTable](../../icellsdatatable/)
* class [CellsDataTableFactory](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetInstance(double[], bool) {#getinstance_1}

Crea ICellsDataTable a partir de la secuencia dada de valores double.

```csharp
public ICellsDataTable GetInstance(double[] vals, bool vertial)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| vals | Double[] | valores double para construir la tabla |
| vertical | Booleano | si construir tabla con los valores dobles verticalmente(true) o horizontalmente(false) |

### Valor de retorno

Instancia de ICellsDataTable

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsDataTableFactoryMethodGetInstanceWithDoubleBooleanDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Preparar datos para los parámetros del método (Double[], Boolean)
            double[] values = new double[] { 10.5, 20.25, 30.75, 40.1, 50.9 };
            bool vertical = true;

            try
            {
                // Crear instancia de CellsDataTableFactory
                CellsDataTableFactory factory = (CellsDataTableFactory)Activator.CreateInstance(typeof(CellsDataTableFactory), nonPublic: true);
                
                // Llamar a GetInstance con (Double[], Boolean)
                ICellsDataTable dataTable = factory.GetInstance(values, vertical);

                // Exportar los datos a la hoja de cálculo
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
            
            // Guardar el resultado
            workbook.Save("CellsDataTableFactoryGetInstanceWithDoubleBooleanDemo.xlsx");
        }
    }
}
```

### Ver también

* interface [ICellsDataTable](../../icellsdatatable/)
* class [CellsDataTableFactory](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetInstance(object[], string[]) {#getinstance_10}

Crea ICellsDataTable a partir de la secuencia dada de objetos.

```csharp
public ICellsDataTable GetInstance(object[] vals, string[] columnNames)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| vals | Object[] | objetos para construir tabla |
| columnNames | String[] | Nombres de columna de la tabla. Su longitud solo puede ser 1(construir tabla con los objetos verticalmente) o la longitud de los objetos(construir tabla con los objetos horizontalmente) |

### Valor de retorno

Instancia de ICellsDataTable

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsDataTableFactoryMethodGetInstanceWithObjectStringDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Preparar datos para los parámetros del método (Object[], String[])
            object[] values = new object[] { "John Doe", 35, 75000.50, DateTime.Now };
            string[] columnNames = new string[] { "Name", "Age", "Salary", "Hire Date" };

            try
            {
                // Crear instancia de CellsDataTableFactory usando reflexión
                CellsDataTableFactory factory = (CellsDataTableFactory)Activator.CreateInstance(typeof(CellsDataTableFactory), nonPublic: true);
                
                // Llamar al método GetInstance con los parámetros (Object[], String[])
                ICellsDataTable dataTable = factory.GetInstance(values, columnNames);

                // Exportar los datos a la hoja de cálculo usando ImportData en lugar de ImportDataTable
                worksheet.Cells.ImportData(dataTable, 0, 0, new ImportTableOptions());

                Console.WriteLine("Method executed successfully with parameters (Object[], String[])");
                Console.WriteLine($"Created table with {dataTable.Count} rows and {dataTable.Columns.Length} columns");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetInstance method: {ex.Message}");
            }
            
            // Guardar el resultado
            workbook.Save("CellsDataTableFactoryGetInstanceWithObjectStringDemo.xlsx");
        }
    }
}
```

### Ver también

* interface [ICellsDataTable](../../icellsdatatable/)
* class [CellsDataTableFactory](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetInstance(object[][], bool, string[]) {#getinstance_11}

Crea un ICellsDataTable a partir de una secuencia dada de objetos.

```csharp
public ICellsDataTable GetInstance(object[][] vals, bool hasHeader, string[] columnNames)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| vals | Object[][] | objetos para construir tabla |
| hasHeader | Booleano | Indica si la primera fila es la fila de encabezado. |
| columnNames | String[] | Nombres de columna de la tabla. Su longitud solo puede ser 1(construir tabla con los objetos verticalmente) o la longitud de los objetos(construir tabla con los objetos horizontalmente) |

### Valor de retorno

Instancia de ICellsDataTable

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsDataTableFactoryMethodGetInstanceWithObjectBooleanStringDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Preparar datos para los parámetros del método (Object[][], Boolean, String[])
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
                // Crear instancia de CellsDataTableFactory
                CellsDataTableFactory factory = (CellsDataTableFactory)Activator.CreateInstance(typeof(CellsDataTableFactory), nonPublic: true);
                
                // Llamar a GetInstance con (Object[][], Boolean, String[])
                ICellsDataTable dataTable = factory.GetInstance(data, hasHeader, columnNames);

                // Exportar los datos a la hoja de cálculo
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
            
            // Guardar el resultado
            workbook.Save("CellsDataTableFactoryGetInstanceWithObjectBooleanStringDemo.xlsx");
        }
    }
}
```

### Ver también

* interface [ICellsDataTable](../../icellsdatatable/)
* class [CellsDataTableFactory](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetInstance(object[], bool) {#getinstance_9}

Crea ICellsDataTable a partir de la secuencia dada de objetos.

```csharp
public ICellsDataTable GetInstance(object[] vals, bool vertial)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| vals | Object[] | objetos para construir tabla |
| vertical | Booleano | si construir tabla con los objetos verticalmente(true) o horizontalmente(false) |

### Valor de retorno

Instancia de ICellsDataTable

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsDataTableFactoryMethodGetInstanceWithObjectBooleanDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Preparar datos para los parámetros del método (Object[], Boolean)
            object[] data = new object[] { "Product", "Price", "Stock", "Available" };
            bool vertical = true;

            try
            {
                // Crear instancia de CellsDataTableFactory usando reflexión
                CellsDataTableFactory factory = (CellsDataTableFactory)Activator.CreateInstance(typeof(CellsDataTableFactory), nonPublic: true);
                
                // Llamar a GetInstance con los parámetros (Object[], Boolean)
                ICellsDataTable dataTable = factory.GetInstance(data, vertical);

                // Exportar los datos a la hoja de cálculo
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
            
            // Guardar el resultado
            workbook.Save("CellsDataTableFactoryGetInstanceWithObjectBooleanDemo.xlsx");
        }
    }
}
```

### Ver también

* interface [ICellsDataTable](../../icellsdatatable/)
* class [CellsDataTableFactory](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetInstance(int[]) {#getinstance_3}

```csharp
public ICellsDataTable GetInstance(int[] vals)
```

### Ver también

* interface [ICellsDataTable](../../icellsdatatable/)
* class [CellsDataTableFactory](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetInstance(double[]) {#getinstance}

```csharp
public ICellsDataTable GetInstance(double[] vals)
```

### Ver también

* interface [ICellsDataTable](../../icellsdatatable/)
* class [CellsDataTableFactory](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetInstance(object[]) {#getinstance_8}

```csharp
public ICellsDataTable GetInstance(object[] vals)
```

### Ver también

* interface [ICellsDataTable](../../icellsdatatable/)
* class [CellsDataTableFactory](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetInstance(ICollection) {#getinstance_6}

Crea ICellsDataTable a partir de la colección proporcionada.

```csharp
public ICellsDataTable GetInstance(ICollection collection)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| colección | ICollection | la colección para construir tabla |

### Valor de retorno

Instancia de ICellsDataTable

### Ejemplos

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
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Preparar un ArrayList como ICollection
            ArrayList data = new ArrayList
            {
                new ArrayList { "Product", "Price", "Stock" },
                new ArrayList { "Keyboard", 49.99, 120 },
                new ArrayList { "Mouse", 29.99, 200 },
                new ArrayList { "Monitor", 199.99, 35 }
            };

            try
            {
                // Crear instancia de CellsDataTableFactory
                CellsDataTableFactory factory = (CellsDataTableFactory)Activator.CreateInstance(typeof(CellsDataTableFactory), nonPublic: true);
                
                // Llamar a GetInstance con el parámetro ICollection
                ICellsDataTable dataTable = factory.GetInstance(data);

                // Exportar los datos a la hoja de cálculo
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
            
            // Guardar el resultado
            workbook.Save("CellsDataTableFactoryGetInstanceWithICollectionDemo.xlsx");
        }
    }
}
```

### Ver también

* interface [ICellsDataTable](../../icellsdatatable/)
* class [CellsDataTableFactory](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetInstance(ICollection, bool) {#getinstance_7}

Crea ICellsDataTable a partir de la colección proporcionada.

```csharp
public ICellsDataTable GetInstance(ICollection collection, bool hasHeader)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| colección | ICollection | la colección para construir tabla |
| hasHeader | Booleano | Indica si la primera fila es encabezado |

### Valor de retorno

Instancia de ICellsDataTable

### Ejemplos

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
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Prepare la colección de datos para los parámetros del método (ICollection, Boolean)
            ArrayList dataCollection = new ArrayList
            {
                new { Product = "Apple", Price = 2.5, Stock = 100 },
                new { Product = "Orange", Price = 1.8, Stock = 150 },
                new { Product = "Banana", Price = 0.9, Stock = 200 }
            };
            bool hasHeader = true;

            try
            {
                // Crear instancia de CellsDataTableFactory
                CellsDataTableFactory factory = (CellsDataTableFactory)Activator.CreateInstance(typeof(CellsDataTableFactory), nonPublic: true);
                
                // Llame a GetInstance con los parámetros (ICollection, Boolean)
                ICellsDataTable dataTable = factory.GetInstance(dataCollection, hasHeader);

                // Exportar los datos a la hoja de cálculo
                worksheet.Cells.ImportData(dataTable, 0, 0, new ImportTableOptions());

                // Mostrar información sobre la tabla creada
                Console.WriteLine("Method executed successfully with parameters (ICollection, Boolean)");
                Console.WriteLine($"Created table with {dataTable.Count} rows and {dataTable.Columns.Length} columns");
                
                // Imprimir nombres de columna
                Console.WriteLine("Column Names:");
                foreach (string colName in dataTable.Columns)
                {
                    Console.WriteLine(colName);
                }

                // Imprimir valores
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
            
            // Guardar el resultado
            workbook.Save("CellsDataTableFactoryGetInstanceWithICollectionBooleanDemo.xlsx");
        }
    }
}
```

### Ver también

* interface [ICellsDataTable](../../icellsdatatable/)
* class [CellsDataTableFactory](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


