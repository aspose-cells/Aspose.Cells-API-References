---
title: "CellsDataTableFactory.GetInstance"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "CellsDataTableFactory‑Methode. Erstellt ICellsDataTable aus einer gegebenen Sequenz von Ganzzahlwerten"
type: docs
url: /de/net/aspose.cells/cellsdatatablefactory/getinstance/
---
## GetInstance(int[], string[]) {#getinstance_5}

Erstellt ICellsDataTable aus der angegebenen Sequenz von Integer-Werten.

```csharp
public ICellsDataTable GetInstance(int[] vals, string[] columnNames)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| vals | Int32[] | int‑Werte zum Erstellen der Tabelle |
| columnNames | String[] | Spaltennamen der Tabelle. Ihre Länge kann nur entweder 1 sein (Tabelle vertikal aus den int‑Werten erstellen) oder die Länge der int‑Werte (Tabelle horizontal aus den int‑Werten erstellen) |

### Rückgabewert

Instanz von ICellsDataTable

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsDataTableFactoryMethodGetInstanceWithInt32StringDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Daten für die Methodenparameter vorbereiten (Int32[], String[])
            int[] values = new int[] { 100, 200, 300, 400, 500 };
            string[] columnNames = new string[] { "Column1", "Column2", "Column3", "Column4", "Column5" };

            try
            {
                // Erstelle eine CellsDataTableFactory-Instanz mithilfe von Reflection
                CellsDataTableFactory factory = (CellsDataTableFactory)Activator.CreateInstance(typeof(CellsDataTableFactory), nonPublic: true);
                
                // Rufe GetInstance mit den Parametern (Int32[], String[]) auf
                ICellsDataTable dataTable = factory.GetInstance(values, columnNames);

                // Gib die Daten in das Arbeitsblatt aus
                worksheet.Cells.ImportData(dataTable, 0, 0, new ImportTableOptions());

                // Zeige einige Informationen über die erstellte Tabelle an
                Console.WriteLine("Method executed successfully with parameters (Int32[], String[])");
                Console.WriteLine($"Created table with {dataTable.Count} rows and {dataTable.Columns.Length} columns");
                
                // Spaltennamen ausgeben
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
            
            // Ergebnis speichern
            workbook.Save("CellsDataTableFactoryGetInstanceWithInt32StringDemo.xlsx");
        }
    }
}
```

### Siehe auch

* interface [ICellsDataTable](../../icellsdatatable/)
* class [CellsDataTableFactory](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetInstance(int[], bool) {#getinstance_4}

Erstellt ICellsDataTable aus der angegebenen Sequenz von Integer-Werten.

```csharp
public ICellsDataTable GetInstance(int[] vals, bool vertial)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| vals | Int32[] | int‑Werte zum Erstellen der Tabelle |
| vertikal | Boolean | ob die Tabelle anhand der int-Werte vertikal (true) oder horizontal (false) erstellt wird |

### Rückgabewert

Instanz von ICellsDataTable

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsDataTableFactoryMethodGetInstanceWithInt32ArrayBooleanDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Daten für die Methodenparameter (Int32[], Boolean) vorbereiten
            int[] values = new int[] { 10, 20, 30, 40, 50 };
            bool vertical = true;

            try
            {
                // Erstelle eine CellsDataTableFactory-Instanz
                CellsDataTableFactory factory = (CellsDataTableFactory)Activator.CreateInstance(typeof(CellsDataTableFactory), nonPublic: true);
                
                // Rufe GetInstance mit den Parametern (Int32[], Boolean) auf
                ICellsDataTable dataTable = factory.GetInstance(values, vertical);

                // Gib die Daten in das Arbeitsblatt aus
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
            
            // Ergebnis speichern
            workbook.Save("CellsDataTableFactoryGetInstanceWithInt32ArrayBooleanDemo.xlsx");
        }
    }
}
```

### Siehe auch

* interface [ICellsDataTable](../../icellsdatatable/)
* class [CellsDataTableFactory](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetInstance(double[], string[]) {#getinstance_2}

Erstellt ICellsDataTable aus der angegebenen Sequenz von Double-Werten.

```csharp
public ICellsDataTable GetInstance(double[] vals, string[] columnNames)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| vals | Double[] | double-Werte zum Erstellen der Tabelle |
| columnNames | String[] | Spaltennamen der Tabelle. Die Länge kann nur entweder 1 sein (Tabelle anhand der double-Werte vertikal erstellen) oder die Länge der double-Werte (Tabelle anhand der double-Werte horizontal erstellen) |

### Rückgabewert

Instanz von ICellsDataTable

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsDataTableFactoryMethodGetInstanceWithDoubleStringDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Daten für die Methodenparameter (Double[], String[]) vorbereiten
            double[] values = new double[] { 10.5, 20.25, 30.75, 40.1, 50.9 };
            string[] columnNames = new string[] { "Price", "Cost", "Margin", "Tax", "Total" };

            try
            {
                // Erstelle eine CellsDataTableFactory-Instanz
                CellsDataTableFactory factory = (CellsDataTableFactory)Activator.CreateInstance(typeof(CellsDataTableFactory), nonPublic: true);
                
                // Rufe GetInstance mit den Parametern (Double[], String[]) auf
                ICellsDataTable dataTable = factory.GetInstance(values, columnNames);

                // Gib die Daten in das Arbeitsblatt aus
                worksheet.Cells.ImportData(dataTable, 0, 0, new ImportTableOptions());

                // Informationen über die erstellte Tabelle anzeigen
                Console.WriteLine("Method executed successfully with parameters (Double[], String[])");
                Console.WriteLine($"Created table with {dataTable.Count} rows and {dataTable.Columns.Length} columns");
                
                // Spaltennamen und Werte ausgeben
                Console.WriteLine("Column Names:");
                foreach (string colName in dataTable.Columns)
                {
                    Console.WriteLine(colName);
                }

                // Werte ausgeben
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
            
            // Ergebnis speichern
            workbook.Save("CellsDataTableFactoryGetInstanceWithDoubleStringDemo.xlsx");
        }
    }
}
```

### Siehe auch

* interface [ICellsDataTable](../../icellsdatatable/)
* class [CellsDataTableFactory](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetInstance(double[], bool) {#getinstance_1}

Erstellt ICellsDataTable aus der angegebenen Sequenz von Double-Werten.

```csharp
public ICellsDataTable GetInstance(double[] vals, bool vertial)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| vals | Double[] | double-Werte zum Erstellen der Tabelle |
| vertikal | Boolean | ob die Tabelle anhand der double-Werte vertikal (true) oder horizontal (false) erstellt wird |

### Rückgabewert

Instanz von ICellsDataTable

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsDataTableFactoryMethodGetInstanceWithDoubleBooleanDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Daten für die Methodenparameter (Double[], Boolean) vorbereiten
            double[] values = new double[] { 10.5, 20.25, 30.75, 40.1, 50.9 };
            bool vertical = true;

            try
            {
                // Erstelle eine CellsDataTableFactory-Instanz
                CellsDataTableFactory factory = (CellsDataTableFactory)Activator.CreateInstance(typeof(CellsDataTableFactory), nonPublic: true);
                
                // Rufe GetInstance mit (Double[], Boolean) auf
                ICellsDataTable dataTable = factory.GetInstance(values, vertical);

                // Gib die Daten in das Arbeitsblatt aus
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
            
            // Ergebnis speichern
            workbook.Save("CellsDataTableFactoryGetInstanceWithDoubleBooleanDemo.xlsx");
        }
    }
}
```

### Siehe auch

* interface [ICellsDataTable](../../icellsdatatable/)
* class [CellsDataTableFactory](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetInstance(object[], string[]) {#getinstance_10}

Erstellt ICellsDataTable aus der angegebenen Sequenz von Objekten.

```csharp
public ICellsDataTable GetInstance(object[] vals, string[] columnNames)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| vals | Object[] | Objekte zum Erstellen der Tabelle |
| columnNames | String[] | Spaltennamen der Tabelle. Die Länge kann nur entweder 1 sein (Tabelle anhand der Objekte vertikal erstellen) oder die Länge der Objekte (Tabelle anhand der Objekte horizontal erstellen) |

### Rückgabewert

Instanz von ICellsDataTable

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsDataTableFactoryMethodGetInstanceWithObjectStringDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Daten für die Methodenparameter (Object[], String[]) vorbereiten
            object[] values = new object[] { "John Doe", 35, 75000.50, DateTime.Now };
            string[] columnNames = new string[] { "Name", "Age", "Salary", "Hire Date" };

            try
            {
                // Erstelle eine CellsDataTableFactory-Instanz mithilfe von Reflection
                CellsDataTableFactory factory = (CellsDataTableFactory)Activator.CreateInstance(typeof(CellsDataTableFactory), nonPublic: true);
                
                // Rufe die GetInstance-Methode mit den Parametern (Object[], String[]) auf
                ICellsDataTable dataTable = factory.GetInstance(values, columnNames);

                // Gib die Daten in das Arbeitsblatt aus, wobei ImportData anstelle von ImportDataTable verwendet wird
                worksheet.Cells.ImportData(dataTable, 0, 0, new ImportTableOptions());

                Console.WriteLine("Method executed successfully with parameters (Object[], String[])");
                Console.WriteLine($"Created table with {dataTable.Count} rows and {dataTable.Columns.Length} columns");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetInstance method: {ex.Message}");
            }
            
            // Ergebnis speichern
            workbook.Save("CellsDataTableFactoryGetInstanceWithObjectStringDemo.xlsx");
        }
    }
}
```

### Siehe auch

* interface [ICellsDataTable](../../icellsdatatable/)
* class [CellsDataTableFactory](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetInstance(object[][], bool, string[]) {#getinstance_11}

Erstellt ein ICellsDataTable aus einer angegebenen Sequenz von Objekten.

```csharp
public ICellsDataTable GetInstance(object[][] vals, bool hasHeader, string[] columnNames)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| vals | Object[][] | Objekte zum Erstellen der Tabelle |
| hasHeader | Boolean | Gibt an, ob die erste Zeile eine Kopfzeile ist. |
| columnNames | String[] | Spaltennamen der Tabelle. Die Länge kann nur entweder 1 sein (Tabelle anhand der Objekte vertikal erstellen) oder die Länge der Objekte (Tabelle anhand der Objekte horizontal erstellen) |

### Rückgabewert

Instanz von ICellsDataTable

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsDataTableFactoryMethodGetInstanceWithObjectBooleanStringDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Bereiten Sie Daten für die Methodenparameter (Object[][], Boolean, String[]) vor
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
                // Erstelle eine CellsDataTableFactory-Instanz
                CellsDataTableFactory factory = (CellsDataTableFactory)Activator.CreateInstance(typeof(CellsDataTableFactory), nonPublic: true);
                
                // Rufen Sie GetInstance mit (Object[][], Boolean, String[]) auf
                ICellsDataTable dataTable = factory.GetInstance(data, hasHeader, columnNames);

                // Gib die Daten in das Arbeitsblatt aus
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
            
            // Ergebnis speichern
            workbook.Save("CellsDataTableFactoryGetInstanceWithObjectBooleanStringDemo.xlsx");
        }
    }
}
```

### Siehe auch

* interface [ICellsDataTable](../../icellsdatatable/)
* class [CellsDataTableFactory](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetInstance(object[], bool) {#getinstance_9}

Erstellt ICellsDataTable aus der angegebenen Sequenz von Objekten.

```csharp
public ICellsDataTable GetInstance(object[] vals, bool vertial)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| vals | Object[] | Objekte zum Erstellen der Tabelle |
| vertikal | Boolean | ob die Tabelle vertikal (true) oder horizontal (false) aus den Objekten erstellt wird |

### Rückgabewert

Instanz von ICellsDataTable

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsDataTableFactoryMethodGetInstanceWithObjectBooleanDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Bereiten Sie Daten für die Methodenparameter (Object[], Boolean) vor
            object[] data = new object[] { "Product", "Price", "Stock", "Available" };
            bool vertical = true;

            try
            {
                // Erstelle eine CellsDataTableFactory-Instanz mithilfe von Reflection
                CellsDataTableFactory factory = (CellsDataTableFactory)Activator.CreateInstance(typeof(CellsDataTableFactory), nonPublic: true);
                
                // Rufen Sie GetInstance mit (Object[], Boolean)-Parametern auf
                ICellsDataTable dataTable = factory.GetInstance(data, vertical);

                // Gib die Daten in das Arbeitsblatt aus
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
            
            // Ergebnis speichern
            workbook.Save("CellsDataTableFactoryGetInstanceWithObjectBooleanDemo.xlsx");
        }
    }
}
```

### Siehe auch

* interface [ICellsDataTable](../../icellsdatatable/)
* class [CellsDataTableFactory](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetInstance(int[]) {#getinstance_3}

```csharp
public ICellsDataTable GetInstance(int[] vals)
```

### Siehe auch

* interface [ICellsDataTable](../../icellsdatatable/)
* class [CellsDataTableFactory](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetInstance(double[]) {#getinstance}

```csharp
public ICellsDataTable GetInstance(double[] vals)
```

### Siehe auch

* interface [ICellsDataTable](../../icellsdatatable/)
* class [CellsDataTableFactory](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetInstance(object[]) {#getinstance_8}

```csharp
public ICellsDataTable GetInstance(object[] vals)
```

### Siehe auch

* interface [ICellsDataTable](../../icellsdatatable/)
* class [CellsDataTableFactory](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetInstance(ICollection) {#getinstance_6}

Erstellt ICellsDataTable aus der angegebenen Sammlung.

```csharp
public ICellsDataTable GetInstance(ICollection collection)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Sammlung | ICollection | die Sammlung zum Erstellen der Tabelle |

### Rückgabewert

Instanz von ICellsDataTable

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Bereiten Sie eine ArrayList als ICollection vor
            ArrayList data = new ArrayList
            {
                new ArrayList { "Product", "Price", "Stock" },
                new ArrayList { "Keyboard", 49.99, 120 },
                new ArrayList { "Mouse", 29.99, 200 },
                new ArrayList { "Monitor", 199.99, 35 }
            };

            try
            {
                // Erstelle eine CellsDataTableFactory-Instanz
                CellsDataTableFactory factory = (CellsDataTableFactory)Activator.CreateInstance(typeof(CellsDataTableFactory), nonPublic: true);
                
                // Rufen Sie GetInstance mit dem ICollection-Parameter auf
                ICellsDataTable dataTable = factory.GetInstance(data);

                // Gib die Daten in das Arbeitsblatt aus
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
            
            // Ergebnis speichern
            workbook.Save("CellsDataTableFactoryGetInstanceWithICollectionDemo.xlsx");
        }
    }
}
```

### Siehe auch

* interface [ICellsDataTable](../../icellsdatatable/)
* class [CellsDataTableFactory](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetInstance(ICollection, bool) {#getinstance_7}

Erstellt ICellsDataTable aus der angegebenen Sammlung.

```csharp
public ICellsDataTable GetInstance(ICollection collection, bool hasHeader)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Sammlung | ICollection | die Sammlung zum Erstellen der Tabelle |
| hasHeader | Boolean | Gibt an, ob die erste Zeile eine Kopfzeile ist |

### Rückgabewert

Instanz von ICellsDataTable

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Bereiten Sie die Datensammlung für die Methodenparameter (ICollection, Boolean) vor
            ArrayList dataCollection = new ArrayList
            {
                new { Product = "Apple", Price = 2.5, Stock = 100 },
                new { Product = "Orange", Price = 1.8, Stock = 150 },
                new { Product = "Banana", Price = 0.9, Stock = 200 }
            };
            bool hasHeader = true;

            try
            {
                // Erstelle eine CellsDataTableFactory-Instanz
                CellsDataTableFactory factory = (CellsDataTableFactory)Activator.CreateInstance(typeof(CellsDataTableFactory), nonPublic: true);
                
                // Rufen Sie GetInstance mit (ICollection, Boolean)-Parametern auf
                ICellsDataTable dataTable = factory.GetInstance(dataCollection, hasHeader);

                // Gib die Daten in das Arbeitsblatt aus
                worksheet.Cells.ImportData(dataTable, 0, 0, new ImportTableOptions());

                // Informationen über die erstellte Tabelle anzeigen
                Console.WriteLine("Method executed successfully with parameters (ICollection, Boolean)");
                Console.WriteLine($"Created table with {dataTable.Count} rows and {dataTable.Columns.Length} columns");
                
                // Spaltennamen ausgeben
                Console.WriteLine("Column Names:");
                foreach (string colName in dataTable.Columns)
                {
                    Console.WriteLine(colName);
                }

                // Werte ausgeben
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
            
            // Ergebnis speichern
            workbook.Save("CellsDataTableFactoryGetInstanceWithICollectionBooleanDemo.xlsx");
        }
    }
}
```

### Siehe auch

* interface [ICellsDataTable](../../icellsdatatable/)
* class [CellsDataTableFactory](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


