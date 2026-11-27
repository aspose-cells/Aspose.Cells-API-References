---
title: "CellsDataTableFactory.GetInstance"
second_title: "Aspose.Cells för .NET API‑referens"
description: "CellsDataTableFactory metod. Skapar ICellsDataTable från given sekvens av heltalsvärden"
type: docs
url: /sv/net/aspose.cells/cellsdatatablefactory/getinstance/
---
## GetInstance(int[], string[]) {#getinstance_5}

Skapar ICellsDataTable från given sekvens av heltalsvärden.

```csharp
public ICellsDataTable GetInstance(int[] vals, string[] columnNames)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| vals | Int32[] | int‑värden för att bygga tabell |
| columnNames | String[] | Kolumnnamn för tabellen. Dess längd kan bara vara antingen 1(bygg tabell med int‑värden vertikalt) eller längden på int‑värdena(bygg tabell med int‑värden horisontellt) |

### Returvärde

Instans av ICellsDataTable

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsDataTableFactoryMethodGetInstanceWithInt32StringDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Förbered data för metodparametrarna (Int32[], String[])
            int[] values = new int[] { 100, 200, 300, 400, 500 };
            string[] columnNames = new string[] { "Column1", "Column2", "Column3", "Column4", "Column5" };

            try
            {
                // Skapa CellsDataTableFactory‑instans med reflektion
                CellsDataTableFactory factory = (CellsDataTableFactory)Activator.CreateInstance(typeof(CellsDataTableFactory), nonPublic: true);
                
                // Anropa GetInstance med (Int32[], String[]) parametrar
                ICellsDataTable dataTable = factory.GetInstance(values, columnNames);

                // Skriv ut data till kalkylbladet
                worksheet.Cells.ImportData(dataTable, 0, 0, new ImportTableOptions());

                // Visa viss information om den skapade tabellen
                Console.WriteLine("Method executed successfully with parameters (Int32[], String[])");
                Console.WriteLine($"Created table with {dataTable.Count} rows and {dataTable.Columns.Length} columns");
                
                // Skriv ut kolumnnamn
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
            
            // Spara resultatet
            workbook.Save("CellsDataTableFactoryGetInstanceWithInt32StringDemo.xlsx");
        }
    }
}
```

### Se även

* interface [ICellsDataTable](../../icellsdatatable/)
* class [CellsDataTableFactory](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetInstance(int[], bool) {#getinstance_4}

Skapar ICellsDataTable från given sekvens av heltalsvärden.

```csharp
public ICellsDataTable GetInstance(int[] vals, bool vertial)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| vals | Int32[] | int‑värden för att bygga tabell |
| vertikal | Boolean | om tabellen ska byggas med int‑värden vertikalt(true) eller horisontellt(false) |

### Returvärde

Instans av ICellsDataTable

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsDataTableFactoryMethodGetInstanceWithInt32ArrayBooleanDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Förbered data för metodparametrarna (Int32[], Boolean)
            int[] values = new int[] { 10, 20, 30, 40, 50 };
            bool vertical = true;

            try
            {
                // Skapa CellsDataTableFactory‑instans
                CellsDataTableFactory factory = (CellsDataTableFactory)Activator.CreateInstance(typeof(CellsDataTableFactory), nonPublic: true);
                
                // Anropa GetInstance med (Int32[], Boolean) parametrar
                ICellsDataTable dataTable = factory.GetInstance(values, vertical);

                // Skriv ut data till kalkylbladet
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
            
            // Spara resultatet
            workbook.Save("CellsDataTableFactoryGetInstanceWithInt32ArrayBooleanDemo.xlsx");
        }
    }
}
```

### Se även

* interface [ICellsDataTable](../../icellsdatatable/)
* class [CellsDataTableFactory](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetInstance(double[], string[]) {#getinstance_2}

Skapar ICellsDataTable från given sekvens av double‑värden.

```csharp
public ICellsDataTable GetInstance(double[] vals, string[] columnNames)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| vals | Double[] | dubbelvärden för att bygga tabell |
| columnNames | String[] | Kolumnnamn för tabellen. Dess längd kan bara vara antingen 1(bygg tabell med dubbelvärden vertikalt) eller längden på dubbelvärdena(bygg tabell med dubbelvärden horisontellt) |

### Returvärde

Instans av ICellsDataTable

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsDataTableFactoryMethodGetInstanceWithDoubleStringDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Förbered data för metodparametrarna (Double[], String[])
            double[] values = new double[] { 10.5, 20.25, 30.75, 40.1, 50.9 };
            string[] columnNames = new string[] { "Price", "Cost", "Margin", "Tax", "Total" };

            try
            {
                // Skapa CellsDataTableFactory‑instans
                CellsDataTableFactory factory = (CellsDataTableFactory)Activator.CreateInstance(typeof(CellsDataTableFactory), nonPublic: true);
                
                // Anropa GetInstance med (Double[], String[]) parametrar
                ICellsDataTable dataTable = factory.GetInstance(values, columnNames);

                // Skriv ut data till kalkylbladet
                worksheet.Cells.ImportData(dataTable, 0, 0, new ImportTableOptions());

                // Visa information om den skapade tabellen
                Console.WriteLine("Method executed successfully with parameters (Double[], String[])");
                Console.WriteLine($"Created table with {dataTable.Count} rows and {dataTable.Columns.Length} columns");
                
                // Skriv ut kolumnnamn och värden
                Console.WriteLine("Column Names:");
                foreach (string colName in dataTable.Columns)
                {
                    Console.WriteLine(colName);
                }

                // Skriv ut värden
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
            
            // Spara resultatet
            workbook.Save("CellsDataTableFactoryGetInstanceWithDoubleStringDemo.xlsx");
        }
    }
}
```

### Se även

* interface [ICellsDataTable](../../icellsdatatable/)
* class [CellsDataTableFactory](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetInstance(double[], bool) {#getinstance_1}

Skapar ICellsDataTable från given sekvens av double‑värden.

```csharp
public ICellsDataTable GetInstance(double[] vals, bool vertial)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| vals | Double[] | dubbelvärden för att bygga tabell |
| vertikal | Boolean | om tabellen ska byggas med dubbelvärden vertikalt(true) eller horisontellt(false) |

### Returvärde

Instans av ICellsDataTable

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsDataTableFactoryMethodGetInstanceWithDoubleBooleanDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Förbered data för metodparametrarna (Double[], Boolean)
            double[] values = new double[] { 10.5, 20.25, 30.75, 40.1, 50.9 };
            bool vertical = true;

            try
            {
                // Skapa CellsDataTableFactory‑instans
                CellsDataTableFactory factory = (CellsDataTableFactory)Activator.CreateInstance(typeof(CellsDataTableFactory), nonPublic: true);
                
                // Anropa GetInstance med (Double[], Boolean)
                ICellsDataTable dataTable = factory.GetInstance(values, vertical);

                // Skriv ut data till kalkylbladet
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
            
            // Spara resultatet
            workbook.Save("CellsDataTableFactoryGetInstanceWithDoubleBooleanDemo.xlsx");
        }
    }
}
```

### Se även

* interface [ICellsDataTable](../../icellsdatatable/)
* class [CellsDataTableFactory](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetInstance(object[], string[]) {#getinstance_10}

Skapar ICellsDataTable från given sekvens av objekt.

```csharp
public ICellsDataTable GetInstance(object[] vals, string[] columnNames)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| vals | Object[] | objekt för att bygga tabell |
| columnNames | String[] | Kolumnnamn för tabellen. Dess längd kan bara vara antingen 1(bygg tabell med objekt vertikalt) eller längden på objekten(bygg tabell med objekt horisontellt) |

### Returvärde

Instans av ICellsDataTable

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsDataTableFactoryMethodGetInstanceWithObjectStringDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Förbered data för metodparametrarna (Object[], String[])
            object[] values = new object[] { "John Doe", 35, 75000.50, DateTime.Now };
            string[] columnNames = new string[] { "Name", "Age", "Salary", "Hire Date" };

            try
            {
                // Skapa CellsDataTableFactory‑instans med reflektion
                CellsDataTableFactory factory = (CellsDataTableFactory)Activator.CreateInstance(typeof(CellsDataTableFactory), nonPublic: true);
                
                // Anropa GetInstance‑metoden med (Object[], String[]) parametrar
                ICellsDataTable dataTable = factory.GetInstance(values, columnNames);

                // Skriv ut data till kalkylbladet med ImportData istället för ImportDataTable
                worksheet.Cells.ImportData(dataTable, 0, 0, new ImportTableOptions());

                Console.WriteLine("Method executed successfully with parameters (Object[], String[])");
                Console.WriteLine($"Created table with {dataTable.Count} rows and {dataTable.Columns.Length} columns");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetInstance method: {ex.Message}");
            }
            
            // Spara resultatet
            workbook.Save("CellsDataTableFactoryGetInstanceWithObjectStringDemo.xlsx");
        }
    }
}
```

### Se även

* interface [ICellsDataTable](../../icellsdatatable/)
* class [CellsDataTableFactory](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetInstance(object[][], bool, string[]) {#getinstance_11}

Skapar en ICellsDataTable från en given sekvens av objekt.

```csharp
public ICellsDataTable GetInstance(object[][] vals, bool hasHeader, string[] columnNames)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| vals | Object[][] | objekt för att bygga tabell |
| hasHeader | Boolean | Anger om den första raden är en rubrikrad. |
| columnNames | String[] | Kolumnnamn för tabellen. Dess längd kan bara vara antingen 1(bygg tabell med objekt vertikalt) eller längden på objekten(bygg tabell med objekt horisontellt) |

### Returvärde

Instans av ICellsDataTable

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsDataTableFactoryMethodGetInstanceWithObjectBooleanStringDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Förbered data för metodparametrarna (Object[][], Boolean, String[])
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
                // Skapa CellsDataTableFactory‑instans
                CellsDataTableFactory factory = (CellsDataTableFactory)Activator.CreateInstance(typeof(CellsDataTableFactory), nonPublic: true);
                
                // Anropa GetInstance med (Object[][], Boolean, String[])
                ICellsDataTable dataTable = factory.GetInstance(data, hasHeader, columnNames);

                // Skriv ut data till kalkylbladet
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
            
            // Spara resultatet
            workbook.Save("CellsDataTableFactoryGetInstanceWithObjectBooleanStringDemo.xlsx");
        }
    }
}
```

### Se även

* interface [ICellsDataTable](../../icellsdatatable/)
* class [CellsDataTableFactory](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetInstance(object[], bool) {#getinstance_9}

Skapar ICellsDataTable från given sekvens av objekt.

```csharp
public ICellsDataTable GetInstance(object[] vals, bool vertial)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| vals | Object[] | objekt för att bygga tabell |
| vertikal | Boolean | om tabellen byggs vertikalt (true) eller horisontellt (false) av objekten |

### Returvärde

Instans av ICellsDataTable

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsDataTableFactoryMethodGetInstanceWithObjectBooleanDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Förbered data för metodparametrarna (Object[], Boolean)
            object[] data = new object[] { "Product", "Price", "Stock", "Available" };
            bool vertical = true;

            try
            {
                // Skapa CellsDataTableFactory‑instans med reflektion
                CellsDataTableFactory factory = (CellsDataTableFactory)Activator.CreateInstance(typeof(CellsDataTableFactory), nonPublic: true);
                
                // Anropa GetInstance med (Object[], Boolean) parametrar
                ICellsDataTable dataTable = factory.GetInstance(data, vertical);

                // Skriv ut data till kalkylbladet
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
            
            // Spara resultatet
            workbook.Save("CellsDataTableFactoryGetInstanceWithObjectBooleanDemo.xlsx");
        }
    }
}
```

### Se även

* interface [ICellsDataTable](../../icellsdatatable/)
* class [CellsDataTableFactory](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetInstance(int[]) {#getinstance_3}

```csharp
public ICellsDataTable GetInstance(int[] vals)
```

### Se även

* interface [ICellsDataTable](../../icellsdatatable/)
* class [CellsDataTableFactory](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetInstance(double[]) {#getinstance}

```csharp
public ICellsDataTable GetInstance(double[] vals)
```

### Se även

* interface [ICellsDataTable](../../icellsdatatable/)
* class [CellsDataTableFactory](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetInstance(object[]) {#getinstance_8}

```csharp
public ICellsDataTable GetInstance(object[] vals)
```

### Se även

* interface [ICellsDataTable](../../icellsdatatable/)
* class [CellsDataTableFactory](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetInstance(ICollection) {#getinstance_6}

Skapar ICellsDataTable från given samling.

```csharp
public ICellsDataTable GetInstance(ICollection collection)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| samling | ICollection | samlingen för att bygga tabellen |

### Returvärde

Instans av ICellsDataTable

### Exempel

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
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Förbered en ArrayList som ICollection
            ArrayList data = new ArrayList
            {
                new ArrayList { "Product", "Price", "Stock" },
                new ArrayList { "Keyboard", 49.99, 120 },
                new ArrayList { "Mouse", 29.99, 200 },
                new ArrayList { "Monitor", 199.99, 35 }
            };

            try
            {
                // Skapa CellsDataTableFactory‑instans
                CellsDataTableFactory factory = (CellsDataTableFactory)Activator.CreateInstance(typeof(CellsDataTableFactory), nonPublic: true);
                
                // Anropa GetInstance med ICollection‑parameter
                ICellsDataTable dataTable = factory.GetInstance(data);

                // Skriv ut data till kalkylbladet
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
            
            // Spara resultatet
            workbook.Save("CellsDataTableFactoryGetInstanceWithICollectionDemo.xlsx");
        }
    }
}
```

### Se även

* interface [ICellsDataTable](../../icellsdatatable/)
* class [CellsDataTableFactory](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetInstance(ICollection, bool) {#getinstance_7}

Skapar ICellsDataTable från given samling.

```csharp
public ICellsDataTable GetInstance(ICollection collection, bool hasHeader)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| samling | ICollection | samlingen för att bygga tabellen |
| hasHeader | Boolean | Anger om den första raden är en rubrik |

### Returvärde

Instans av ICellsDataTable

### Exempel

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
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Förbered datainsamling för metodparametrarna (ICollection, Boolean)
            ArrayList dataCollection = new ArrayList
            {
                new { Product = "Apple", Price = 2.5, Stock = 100 },
                new { Product = "Orange", Price = 1.8, Stock = 150 },
                new { Product = "Banana", Price = 0.9, Stock = 200 }
            };
            bool hasHeader = true;

            try
            {
                // Skapa CellsDataTableFactory‑instans
                CellsDataTableFactory factory = (CellsDataTableFactory)Activator.CreateInstance(typeof(CellsDataTableFactory), nonPublic: true);
                
                // Anropa GetInstance med (ICollection, Boolean) parametrar
                ICellsDataTable dataTable = factory.GetInstance(dataCollection, hasHeader);

                // Skriv ut data till kalkylbladet
                worksheet.Cells.ImportData(dataTable, 0, 0, new ImportTableOptions());

                // Visa information om den skapade tabellen
                Console.WriteLine("Method executed successfully with parameters (ICollection, Boolean)");
                Console.WriteLine($"Created table with {dataTable.Count} rows and {dataTable.Columns.Length} columns");
                
                // Skriv ut kolumnnamn
                Console.WriteLine("Column Names:");
                foreach (string colName in dataTable.Columns)
                {
                    Console.WriteLine(colName);
                }

                // Skriv ut värden
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
            
            // Spara resultatet
            workbook.Save("CellsDataTableFactoryGetInstanceWithICollectionBooleanDemo.xlsx");
        }
    }
}
```

### Se även

* interface [ICellsDataTable](../../icellsdatatable/)
* class [CellsDataTableFactory](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


