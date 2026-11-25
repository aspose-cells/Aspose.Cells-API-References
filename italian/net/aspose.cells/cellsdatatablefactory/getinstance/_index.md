---
title: "CellsDataTableFactory.GetInstance"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo CellsDataTableFactory. Crea ICellsDataTable dalla sequenza fornita di valori interi"
type: docs
url: /it/net/aspose.cells/cellsdatatablefactory/getinstance/
---
## GetInstance(int[], string[]) {#getinstance_5}

Crea ICellsDataTable da una sequenza di valori interi fornita.

```csharp
public ICellsDataTable GetInstance(int[] vals, string[] columnNames)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| vals | Int32[] | valori interi per costruire la tabella |
| columnNames | String[] | Nomi delle colonne della tabella. La sua lunghezza può essere solo 1 (costruisci la tabella dai valori interi verticalmente) o la lunghezza dei valori interi (costruisci la tabella dai valori interi orizzontalmente) |

### Valore di ritorno

Istanza di ICellsDataTable

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsDataTableFactoryMethodGetInstanceWithInt32StringDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Prepara i dati per i parametri del metodo (Int32[], String[])
            int[] values = new int[] { 100, 200, 300, 400, 500 };
            string[] columnNames = new string[] { "Column1", "Column2", "Column3", "Column4", "Column5" };

            try
            {
                // Crea un'istanza di CellsDataTableFactory usando la riflessione
                CellsDataTableFactory factory = (CellsDataTableFactory)Activator.CreateInstance(typeof(CellsDataTableFactory), nonPublic: true);
                
                // Chiama GetInstance con parametri (Int32[], String[])
                ICellsDataTable dataTable = factory.GetInstance(values, columnNames);

                // Scrivi i dati nel foglio di lavoro
                worksheet.Cells.ImportData(dataTable, 0, 0, new ImportTableOptions());

                // Mostra alcune informazioni sulla tabella creata
                Console.WriteLine("Method executed successfully with parameters (Int32[], String[])");
                Console.WriteLine($"Created table with {dataTable.Count} rows and {dataTable.Columns.Length} columns");
                
                // Stampa i nomi delle colonne
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
            
            // Salva il risultato
            workbook.Save("CellsDataTableFactoryGetInstanceWithInt32StringDemo.xlsx");
        }
    }
}
```

### Vedi anche

* interface [ICellsDataTable](../../icellsdatatable/)
* class [CellsDataTableFactory](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetInstance(int[], bool) {#getinstance_4}

Crea ICellsDataTable da una sequenza di valori interi fornita.

```csharp
public ICellsDataTable GetInstance(int[] vals, bool vertial)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| vals | Int32[] | valori interi per costruire la tabella |
| verticale | Booleano | se costruire la tabella dai valori interi verticalmente (true) o orizzontalmente (false) |

### Valore di ritorno

Istanza di ICellsDataTable

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsDataTableFactoryMethodGetInstanceWithInt32ArrayBooleanDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Prepara i dati per i parametri del metodo (Int32[], Boolean)
            int[] values = new int[] { 10, 20, 30, 40, 50 };
            bool vertical = true;

            try
            {
                // Crea un'istanza di CellsDataTableFactory
                CellsDataTableFactory factory = (CellsDataTableFactory)Activator.CreateInstance(typeof(CellsDataTableFactory), nonPublic: true);
                
                // Chiama GetInstance con parametri (Int32[], Boolean)
                ICellsDataTable dataTable = factory.GetInstance(values, vertical);

                // Scrivi i dati nel foglio di lavoro
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
            
            // Salva il risultato
            workbook.Save("CellsDataTableFactoryGetInstanceWithInt32ArrayBooleanDemo.xlsx");
        }
    }
}
```

### Vedi anche

* interface [ICellsDataTable](../../icellsdatatable/)
* class [CellsDataTableFactory](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetInstance(double[], string[]) {#getinstance_2}

Crea ICellsDataTable da una sequenza di valori double fornita.

```csharp
public ICellsDataTable GetInstance(double[] vals, string[] columnNames)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| vals | Double[] | valori double per costruire la tabella |
| columnNames | String[] | Nomi delle colonne della tabella. La sua lunghezza può essere solo 1(crea tabella con i double values verticalmente) o la lunghezza dei double values(crea tabella con i double values orizzontalmente) |

### Valore di ritorno

Istanza di ICellsDataTable

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsDataTableFactoryMethodGetInstanceWithDoubleStringDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Prepara i dati per i parametri del metodo (Double[], String[])
            double[] values = new double[] { 10.5, 20.25, 30.75, 40.1, 50.9 };
            string[] columnNames = new string[] { "Price", "Cost", "Margin", "Tax", "Total" };

            try
            {
                // Crea un'istanza di CellsDataTableFactory
                CellsDataTableFactory factory = (CellsDataTableFactory)Activator.CreateInstance(typeof(CellsDataTableFactory), nonPublic: true);
                
                // Chiama GetInstance con i parametri (Double[], String[])
                ICellsDataTable dataTable = factory.GetInstance(values, columnNames);

                // Scrivi i dati nel foglio di lavoro
                worksheet.Cells.ImportData(dataTable, 0, 0, new ImportTableOptions());

                // Visualizza le informazioni sulla tabella creata
                Console.WriteLine("Method executed successfully with parameters (Double[], String[])");
                Console.WriteLine($"Created table with {dataTable.Count} rows and {dataTable.Columns.Length} columns");
                
                // Stampa i nomi delle colonne e i valori
                Console.WriteLine("Column Names:");
                foreach (string colName in dataTable.Columns)
                {
                    Console.WriteLine(colName);
                }

                // Stampa i valori
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
            
            // Salva il risultato
            workbook.Save("CellsDataTableFactoryGetInstanceWithDoubleStringDemo.xlsx");
        }
    }
}
```

### Vedi anche

* interface [ICellsDataTable](../../icellsdatatable/)
* class [CellsDataTableFactory](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetInstance(double[], bool) {#getinstance_1}

Crea ICellsDataTable da una sequenza di valori double fornita.

```csharp
public ICellsDataTable GetInstance(double[] vals, bool vertial)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| vals | Double[] | valori double per costruire la tabella |
| verticale | Booleano | se costruire la tabella con i double values verticalmente(true) o orizzontalmente(false) |

### Valore di ritorno

Istanza di ICellsDataTable

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsDataTableFactoryMethodGetInstanceWithDoubleBooleanDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Prepara i dati per i parametri del metodo (Double[], Boolean)
            double[] values = new double[] { 10.5, 20.25, 30.75, 40.1, 50.9 };
            bool vertical = true;

            try
            {
                // Crea un'istanza di CellsDataTableFactory
                CellsDataTableFactory factory = (CellsDataTableFactory)Activator.CreateInstance(typeof(CellsDataTableFactory), nonPublic: true);
                
                // Chiama GetInstance con (Double[], Boolean)
                ICellsDataTable dataTable = factory.GetInstance(values, vertical);

                // Scrivi i dati nel foglio di lavoro
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
            
            // Salva il risultato
            workbook.Save("CellsDataTableFactoryGetInstanceWithDoubleBooleanDemo.xlsx");
        }
    }
}
```

### Vedi anche

* interface [ICellsDataTable](../../icellsdatatable/)
* class [CellsDataTableFactory](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetInstance(object[], string[]) {#getinstance_10}

Crea ICellsDataTable da una sequenza di oggetti fornita.

```csharp
public ICellsDataTable GetInstance(object[] vals, string[] columnNames)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| vals | Object[] | oggetti per costruire la tabella |
| columnNames | String[] | Nomi delle colonne della tabella. La sua lunghezza può essere solo 1(crea tabella con gli objects verticalmente) o la lunghezza degli objects(crea tabella con gli objects orizzontalmente) |

### Valore di ritorno

Istanza di ICellsDataTable

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsDataTableFactoryMethodGetInstanceWithObjectStringDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Prepara i dati per i parametri del metodo (Object[], String[])
            object[] values = new object[] { "John Doe", 35, 75000.50, DateTime.Now };
            string[] columnNames = new string[] { "Name", "Age", "Salary", "Hire Date" };

            try
            {
                // Crea un'istanza di CellsDataTableFactory usando la riflessione
                CellsDataTableFactory factory = (CellsDataTableFactory)Activator.CreateInstance(typeof(CellsDataTableFactory), nonPublic: true);
                
                // Chiama il metodo GetInstance con i parametri (Object[], String[])
                ICellsDataTable dataTable = factory.GetInstance(values, columnNames);

                // Esporta i dati nel foglio di lavoro usando ImportData invece di ImportDataTable
                worksheet.Cells.ImportData(dataTable, 0, 0, new ImportTableOptions());

                Console.WriteLine("Method executed successfully with parameters (Object[], String[])");
                Console.WriteLine($"Created table with {dataTable.Count} rows and {dataTable.Columns.Length} columns");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetInstance method: {ex.Message}");
            }
            
            // Salva il risultato
            workbook.Save("CellsDataTableFactoryGetInstanceWithObjectStringDemo.xlsx");
        }
    }
}
```

### Vedi anche

* interface [ICellsDataTable](../../icellsdatatable/)
* class [CellsDataTableFactory](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetInstance(object[][], bool, string[]) {#getinstance_11}

Crea un ICellsDataTable da una sequenza di oggetti fornita.

```csharp
public ICellsDataTable GetInstance(object[][] vals, bool hasHeader, string[] columnNames)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| vals | Object[][] | oggetti per costruire la tabella |
| hasHeader | Booleano | Indica se la prima riga è la riga di intestazione. |
| columnNames | String[] | Nomi delle colonne della tabella. La sua lunghezza può essere solo 1(crea tabella con gli objects verticalmente) o la lunghezza degli objects(crea tabella con gli objects orizzontalmente) |

### Valore di ritorno

Istanza di ICellsDataTable

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsDataTableFactoryMethodGetInstanceWithObjectBooleanStringDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Prepara i dati per i parametri del metodo (Object[][], Boolean, String[])
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
                // Crea un'istanza di CellsDataTableFactory
                CellsDataTableFactory factory = (CellsDataTableFactory)Activator.CreateInstance(typeof(CellsDataTableFactory), nonPublic: true);
                
                // Chiama GetInstance con (Object[][], Boolean, String[])
                ICellsDataTable dataTable = factory.GetInstance(data, hasHeader, columnNames);

                // Scrivi i dati nel foglio di lavoro
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
            
            // Salva il risultato
            workbook.Save("CellsDataTableFactoryGetInstanceWithObjectBooleanStringDemo.xlsx");
        }
    }
}
```

### Vedi anche

* interface [ICellsDataTable](../../icellsdatatable/)
* class [CellsDataTableFactory](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetInstance(object[], bool) {#getinstance_9}

Crea ICellsDataTable da una sequenza di oggetti fornita.

```csharp
public ICellsDataTable GetInstance(object[] vals, bool vertial)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| vals | Object[] | oggetti per costruire la tabella |
| verticale | Booleano | se costruire la tabella con gli objects verticalmente(true) o orizzontalmente(false) |

### Valore di ritorno

Istanza di ICellsDataTable

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsDataTableFactoryMethodGetInstanceWithObjectBooleanDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Prepara i dati per i parametri del metodo (Object[], Boolean)
            object[] data = new object[] { "Product", "Price", "Stock", "Available" };
            bool vertical = true;

            try
            {
                // Crea un'istanza di CellsDataTableFactory usando la riflessione
                CellsDataTableFactory factory = (CellsDataTableFactory)Activator.CreateInstance(typeof(CellsDataTableFactory), nonPublic: true);
                
                // Chiama GetInstance con i parametri (Object[], Boolean)
                ICellsDataTable dataTable = factory.GetInstance(data, vertical);

                // Scrivi i dati nel foglio di lavoro
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
            
            // Salva il risultato
            workbook.Save("CellsDataTableFactoryGetInstanceWithObjectBooleanDemo.xlsx");
        }
    }
}
```

### Vedi anche

* interface [ICellsDataTable](../../icellsdatatable/)
* class [CellsDataTableFactory](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetInstance(int[]) {#getinstance_3}

```csharp
public ICellsDataTable GetInstance(int[] vals)
```

### Vedi anche

* interface [ICellsDataTable](../../icellsdatatable/)
* class [CellsDataTableFactory](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetInstance(double[]) {#getinstance}

```csharp
public ICellsDataTable GetInstance(double[] vals)
```

### Vedi anche

* interface [ICellsDataTable](../../icellsdatatable/)
* class [CellsDataTableFactory](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetInstance(object[]) {#getinstance_8}

```csharp
public ICellsDataTable GetInstance(object[] vals)
```

### Vedi anche

* interface [ICellsDataTable](../../icellsdatatable/)
* class [CellsDataTableFactory](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetInstance(ICollection) {#getinstance_6}

Crea ICellsDataTable dalla collezione fornita.

```csharp
public ICellsDataTable GetInstance(ICollection collection)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| collection | ICollection | la collection per costruire la tabella |

### Valore di ritorno

Istanza di ICellsDataTable

### Esempi

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
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Prepara un ArrayList come ICollection
            ArrayList data = new ArrayList
            {
                new ArrayList { "Product", "Price", "Stock" },
                new ArrayList { "Keyboard", 49.99, 120 },
                new ArrayList { "Mouse", 29.99, 200 },
                new ArrayList { "Monitor", 199.99, 35 }
            };

            try
            {
                // Crea un'istanza di CellsDataTableFactory
                CellsDataTableFactory factory = (CellsDataTableFactory)Activator.CreateInstance(typeof(CellsDataTableFactory), nonPublic: true);
                
                // Chiama GetInstance con il parametro ICollection
                ICellsDataTable dataTable = factory.GetInstance(data);

                // Scrivi i dati nel foglio di lavoro
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
            
            // Salva il risultato
            workbook.Save("CellsDataTableFactoryGetInstanceWithICollectionDemo.xlsx");
        }
    }
}
```

### Vedi anche

* interface [ICellsDataTable](../../icellsdatatable/)
* class [CellsDataTableFactory](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetInstance(ICollection, bool) {#getinstance_7}

Crea ICellsDataTable dalla collezione fornita.

```csharp
public ICellsDataTable GetInstance(ICollection collection, bool hasHeader)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| collection | ICollection | la collection per costruire la tabella |
| hasHeader | Booleano | Indica se la prima riga è un'intestazione |

### Valore di ritorno

Istanza di ICellsDataTable

### Esempi

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
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Prepara la raccolta dati per i parametri del metodo (ICollection, Boolean)
            ArrayList dataCollection = new ArrayList
            {
                new { Product = "Apple", Price = 2.5, Stock = 100 },
                new { Product = "Orange", Price = 1.8, Stock = 150 },
                new { Product = "Banana", Price = 0.9, Stock = 200 }
            };
            bool hasHeader = true;

            try
            {
                // Crea un'istanza di CellsDataTableFactory
                CellsDataTableFactory factory = (CellsDataTableFactory)Activator.CreateInstance(typeof(CellsDataTableFactory), nonPublic: true);
                
                // Chiama GetInstance con i parametri (ICollection, Boolean)
                ICellsDataTable dataTable = factory.GetInstance(dataCollection, hasHeader);

                // Scrivi i dati nel foglio di lavoro
                worksheet.Cells.ImportData(dataTable, 0, 0, new ImportTableOptions());

                // Visualizza le informazioni sulla tabella creata
                Console.WriteLine("Method executed successfully with parameters (ICollection, Boolean)");
                Console.WriteLine($"Created table with {dataTable.Count} rows and {dataTable.Columns.Length} columns");
                
                // Stampa i nomi delle colonne
                Console.WriteLine("Column Names:");
                foreach (string colName in dataTable.Columns)
                {
                    Console.WriteLine(colName);
                }

                // Stampa i valori
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
            
            // Salva il risultato
            workbook.Save("CellsDataTableFactoryGetInstanceWithICollectionBooleanDemo.xlsx");
        }
    }
}
```

### Vedi anche

* interface [ICellsDataTable](../../icellsdatatable/)
* class [CellsDataTableFactory](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


