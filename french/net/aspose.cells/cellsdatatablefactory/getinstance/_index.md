---
title: "CellsDataTableFactory.GetInstance"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode CellsDataTableFactory. Crée ICellsDataTable à partir d'une séquence donnée de valeurs entières"
type: docs
url: /fr/net/aspose.cells/cellsdatatablefactory/getinstance/
---
## GetInstance(int[], string[]) {#getinstance_5}

Crée ICellsDataTable à partir de la séquence donnée de valeurs entières.

```csharp
public ICellsDataTable GetInstance(int[] vals, string[] columnNames)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| vals | Int32[] | valeurs entières pour construire le tableau |
| columnNames | String[] | Noms des colonnes du tableau. Sa longueur ne peut être que 1 (construire le tableau à partir des valeurs entières verticalement) ou la longueur des valeurs entières (construire le tableau à partir des valeurs entières horizontalement) |

### Valeur de retour

Instance de ICellsDataTable

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsDataTableFactoryMethodGetInstanceWithInt32StringDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Préparer les données pour les paramètres de la méthode (Int32[], String[])
            int[] values = new int[] { 100, 200, 300, 400, 500 };
            string[] columnNames = new string[] { "Column1", "Column2", "Column3", "Column4", "Column5" };

            try
            {
                // Créer une instance de CellsDataTableFactory en utilisant la réflexion
                CellsDataTableFactory factory = (CellsDataTableFactory)Activator.CreateInstance(typeof(CellsDataTableFactory), nonPublic: true);
                
                // Appeler GetInstance avec les paramètres (Int32[], String[])
                ICellsDataTable dataTable = factory.GetInstance(values, columnNames);

                // Exporter les données vers la feuille de calcul
                worksheet.Cells.ImportData(dataTable, 0, 0, new ImportTableOptions());

                // Afficher certaines informations sur le tableau créé
                Console.WriteLine("Method executed successfully with parameters (Int32[], String[])");
                Console.WriteLine($"Created table with {dataTable.Count} rows and {dataTable.Columns.Length} columns");
                
                // Imprimer les noms des colonnes
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
            
            // Enregistrer le résultat
            workbook.Save("CellsDataTableFactoryGetInstanceWithInt32StringDemo.xlsx");
        }
    }
}
```

### Voir aussi

* interface [ICellsDataTable](../../icellsdatatable/)
* class [CellsDataTableFactory](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetInstance(int[], bool) {#getinstance_4}

Crée ICellsDataTable à partir de la séquence donnée de valeurs entières.

```csharp
public ICellsDataTable GetInstance(int[] vals, bool vertial)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| vals | Int32[] | valeurs entières pour construire le tableau |
| vertical | Boolean | indique si le tableau est construit à partir des valeurs entières verticalement (true) ou horizontalement (false) |

### Valeur de retour

Instance de ICellsDataTable

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsDataTableFactoryMethodGetInstanceWithInt32ArrayBooleanDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Préparer les données pour les paramètres de la méthode (Int32[], Boolean)
            int[] values = new int[] { 10, 20, 30, 40, 50 };
            bool vertical = true;

            try
            {
                // Créer une instance de CellsDataTableFactory
                CellsDataTableFactory factory = (CellsDataTableFactory)Activator.CreateInstance(typeof(CellsDataTableFactory), nonPublic: true);
                
                // Appeler GetInstance avec les paramètres (Int32[], Boolean)
                ICellsDataTable dataTable = factory.GetInstance(values, vertical);

                // Exporter les données vers la feuille de calcul
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
            
            // Enregistrer le résultat
            workbook.Save("CellsDataTableFactoryGetInstanceWithInt32ArrayBooleanDemo.xlsx");
        }
    }
}
```

### Voir aussi

* interface [ICellsDataTable](../../icellsdatatable/)
* class [CellsDataTableFactory](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetInstance(double[], string[]) {#getinstance_2}

Crée ICellsDataTable à partir de la séquence donnée de valeurs double.

```csharp
public ICellsDataTable GetInstance(double[] vals, string[] columnNames)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| vals | Double[] | valeurs doubles pour construire le tableau |
| columnNames | String[] | Noms de colonnes du tableau. Sa longueur ne peut être que 1(construire le tableau avec les valeurs doubles verticalement) ou la longueur des valeurs doubles(construire le tableau avec les valeurs doubles horizontalement) |

### Valeur de retour

Instance de ICellsDataTable

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsDataTableFactoryMethodGetInstanceWithDoubleStringDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Préparer les données pour les paramètres de la méthode (Double[], String[])
            double[] values = new double[] { 10.5, 20.25, 30.75, 40.1, 50.9 };
            string[] columnNames = new string[] { "Price", "Cost", "Margin", "Tax", "Total" };

            try
            {
                // Créer une instance de CellsDataTableFactory
                CellsDataTableFactory factory = (CellsDataTableFactory)Activator.CreateInstance(typeof(CellsDataTableFactory), nonPublic: true);
                
                // Appeler GetInstance avec les paramètres (Double[], String[])
                ICellsDataTable dataTable = factory.GetInstance(values, columnNames);

                // Exporter les données vers la feuille de calcul
                worksheet.Cells.ImportData(dataTable, 0, 0, new ImportTableOptions());

                // Afficher les informations sur le tableau créé
                Console.WriteLine("Method executed successfully with parameters (Double[], String[])");
                Console.WriteLine($"Created table with {dataTable.Count} rows and {dataTable.Columns.Length} columns");
                
                // Imprimer les noms de colonnes et les valeurs
                Console.WriteLine("Column Names:");
                foreach (string colName in dataTable.Columns)
                {
                    Console.WriteLine(colName);
                }

                // Imprimer les valeurs
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
            
            // Enregistrer le résultat
            workbook.Save("CellsDataTableFactoryGetInstanceWithDoubleStringDemo.xlsx");
        }
    }
}
```

### Voir aussi

* interface [ICellsDataTable](../../icellsdatatable/)
* class [CellsDataTableFactory](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetInstance(double[], bool) {#getinstance_1}

Crée ICellsDataTable à partir de la séquence donnée de valeurs double.

```csharp
public ICellsDataTable GetInstance(double[] vals, bool vertial)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| vals | Double[] | valeurs doubles pour construire le tableau |
| vertical | Boolean | si construire le tableau avec les valeurs doubles verticalement(true) ou horizontalement(false) |

### Valeur de retour

Instance de ICellsDataTable

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsDataTableFactoryMethodGetInstanceWithDoubleBooleanDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Préparer les données pour les paramètres de la méthode (Double[], Boolean)
            double[] values = new double[] { 10.5, 20.25, 30.75, 40.1, 50.9 };
            bool vertical = true;

            try
            {
                // Créer une instance de CellsDataTableFactory
                CellsDataTableFactory factory = (CellsDataTableFactory)Activator.CreateInstance(typeof(CellsDataTableFactory), nonPublic: true);
                
                // Appeler GetInstance avec (Double[], Boolean)
                ICellsDataTable dataTable = factory.GetInstance(values, vertical);

                // Exporter les données vers la feuille de calcul
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
            
            // Enregistrer le résultat
            workbook.Save("CellsDataTableFactoryGetInstanceWithDoubleBooleanDemo.xlsx");
        }
    }
}
```

### Voir aussi

* interface [ICellsDataTable](../../icellsdatatable/)
* class [CellsDataTableFactory](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetInstance(object[], string[]) {#getinstance_10}

Crée ICellsDataTable à partir de la séquence donnée d'objets.

```csharp
public ICellsDataTable GetInstance(object[] vals, string[] columnNames)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| vals | Object[] | objets pour construire le tableau |
| columnNames | String[] | Noms de colonnes du tableau. Sa longueur ne peut être que 1(construire le tableau avec les objets verticalement) ou la longueur des objets(construire le tableau avec les objets horizontalement) |

### Valeur de retour

Instance de ICellsDataTable

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsDataTableFactoryMethodGetInstanceWithObjectStringDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Préparer les données pour les paramètres de la méthode (Object[], String[])
            object[] values = new object[] { "John Doe", 35, 75000.50, DateTime.Now };
            string[] columnNames = new string[] { "Name", "Age", "Salary", "Hire Date" };

            try
            {
                // Créer une instance de CellsDataTableFactory en utilisant la réflexion
                CellsDataTableFactory factory = (CellsDataTableFactory)Activator.CreateInstance(typeof(CellsDataTableFactory), nonPublic: true);
                
                // Appeler la méthode GetInstance avec les paramètres (Object[], String[])
                ICellsDataTable dataTable = factory.GetInstance(values, columnNames);

                // Exporter les données vers la feuille de calcul en utilisant ImportData au lieu de ImportDataTable
                worksheet.Cells.ImportData(dataTable, 0, 0, new ImportTableOptions());

                Console.WriteLine("Method executed successfully with parameters (Object[], String[])");
                Console.WriteLine($"Created table with {dataTable.Count} rows and {dataTable.Columns.Length} columns");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetInstance method: {ex.Message}");
            }
            
            // Enregistrer le résultat
            workbook.Save("CellsDataTableFactoryGetInstanceWithObjectStringDemo.xlsx");
        }
    }
}
```

### Voir aussi

* interface [ICellsDataTable](../../icellsdatatable/)
* class [CellsDataTableFactory](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetInstance(object[][], bool, string[]) {#getinstance_11}

Crée un ICellsDataTable à partir d'une séquence donnée d'objets.

```csharp
public ICellsDataTable GetInstance(object[][] vals, bool hasHeader, string[] columnNames)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| vals | Object[][] | objets pour construire le tableau |
| hasHeader | Boolean | Indique si la première ligne est une ligne d'en-tête. |
| columnNames | String[] | Noms de colonnes du tableau. Sa longueur ne peut être que 1(construire le tableau avec les objets verticalement) ou la longueur des objets(construire le tableau avec les objets horizontalement) |

### Valeur de retour

Instance de ICellsDataTable

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsDataTableFactoryMethodGetInstanceWithObjectBooleanStringDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Préparer les données pour les paramètres de la méthode (Object[][], Boolean, String[])
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
                // Créer une instance de CellsDataTableFactory
                CellsDataTableFactory factory = (CellsDataTableFactory)Activator.CreateInstance(typeof(CellsDataTableFactory), nonPublic: true);
                
                // Appeler GetInstance avec (Object[][], Boolean, String[])
                ICellsDataTable dataTable = factory.GetInstance(data, hasHeader, columnNames);

                // Exporter les données vers la feuille de calcul
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
            
            // Enregistrer le résultat
            workbook.Save("CellsDataTableFactoryGetInstanceWithObjectBooleanStringDemo.xlsx");
        }
    }
}
```

### Voir aussi

* interface [ICellsDataTable](../../icellsdatatable/)
* class [CellsDataTableFactory](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetInstance(object[], bool) {#getinstance_9}

Crée ICellsDataTable à partir de la séquence donnée d'objets.

```csharp
public ICellsDataTable GetInstance(object[] vals, bool vertial)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| vals | Object[] | objets pour construire le tableau |
| vertical | Boolean | si construire le tableau avec les objets verticalement(true) ou horizontalement(false) |

### Valeur de retour

Instance de ICellsDataTable

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsDataTableFactoryMethodGetInstanceWithObjectBooleanDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Préparer les données pour les paramètres de la méthode (Object[], Boolean)
            object[] data = new object[] { "Product", "Price", "Stock", "Available" };
            bool vertical = true;

            try
            {
                // Créer une instance de CellsDataTableFactory en utilisant la réflexion
                CellsDataTableFactory factory = (CellsDataTableFactory)Activator.CreateInstance(typeof(CellsDataTableFactory), nonPublic: true);
                
                // Appeler GetInstance avec les paramètres (Object[], Boolean)
                ICellsDataTable dataTable = factory.GetInstance(data, vertical);

                // Exporter les données vers la feuille de calcul
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
            
            // Enregistrer le résultat
            workbook.Save("CellsDataTableFactoryGetInstanceWithObjectBooleanDemo.xlsx");
        }
    }
}
```

### Voir aussi

* interface [ICellsDataTable](../../icellsdatatable/)
* class [CellsDataTableFactory](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetInstance(int[]) {#getinstance_3}

```csharp
public ICellsDataTable GetInstance(int[] vals)
```

### Voir aussi

* interface [ICellsDataTable](../../icellsdatatable/)
* class [CellsDataTableFactory](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetInstance(double[]) {#getinstance}

```csharp
public ICellsDataTable GetInstance(double[] vals)
```

### Voir aussi

* interface [ICellsDataTable](../../icellsdatatable/)
* class [CellsDataTableFactory](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetInstance(object[]) {#getinstance_8}

```csharp
public ICellsDataTable GetInstance(object[] vals)
```

### Voir aussi

* interface [ICellsDataTable](../../icellsdatatable/)
* class [CellsDataTableFactory](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetInstance(ICollection) {#getinstance_6}

Crée ICellsDataTable à partir de la collection fournie.

```csharp
public ICellsDataTable GetInstance(ICollection collection)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| collection | ICollection | la collection pour construire le tableau |

### Valeur de retour

Instance de ICellsDataTable

### Exemples

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
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Préparer un ArrayList en tant que ICollection
            ArrayList data = new ArrayList
            {
                new ArrayList { "Product", "Price", "Stock" },
                new ArrayList { "Keyboard", 49.99, 120 },
                new ArrayList { "Mouse", 29.99, 200 },
                new ArrayList { "Monitor", 199.99, 35 }
            };

            try
            {
                // Créer une instance de CellsDataTableFactory
                CellsDataTableFactory factory = (CellsDataTableFactory)Activator.CreateInstance(typeof(CellsDataTableFactory), nonPublic: true);
                
                // Appeler GetInstance avec le paramètre ICollection
                ICellsDataTable dataTable = factory.GetInstance(data);

                // Exporter les données vers la feuille de calcul
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
            
            // Enregistrer le résultat
            workbook.Save("CellsDataTableFactoryGetInstanceWithICollectionDemo.xlsx");
        }
    }
}
```

### Voir aussi

* interface [ICellsDataTable](../../icellsdatatable/)
* class [CellsDataTableFactory](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetInstance(ICollection, bool) {#getinstance_7}

Crée ICellsDataTable à partir de la collection fournie.

```csharp
public ICellsDataTable GetInstance(ICollection collection, bool hasHeader)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| collection | ICollection | la collection pour construire le tableau |
| hasHeader | Boolean | Indique si la première ligne est un en-tête |

### Valeur de retour

Instance de ICellsDataTable

### Exemples

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
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Préparez la collection de données pour les paramètres de la méthode (ICollection, Boolean)
            ArrayList dataCollection = new ArrayList
            {
                new { Product = "Apple", Price = 2.5, Stock = 100 },
                new { Product = "Orange", Price = 1.8, Stock = 150 },
                new { Product = "Banana", Price = 0.9, Stock = 200 }
            };
            bool hasHeader = true;

            try
            {
                // Créer une instance de CellsDataTableFactory
                CellsDataTableFactory factory = (CellsDataTableFactory)Activator.CreateInstance(typeof(CellsDataTableFactory), nonPublic: true);
                
                // Appelez GetInstance avec les paramètres (ICollection, Boolean)
                ICellsDataTable dataTable = factory.GetInstance(dataCollection, hasHeader);

                // Exporter les données vers la feuille de calcul
                worksheet.Cells.ImportData(dataTable, 0, 0, new ImportTableOptions());

                // Afficher les informations sur le tableau créé
                Console.WriteLine("Method executed successfully with parameters (ICollection, Boolean)");
                Console.WriteLine($"Created table with {dataTable.Count} rows and {dataTable.Columns.Length} columns");
                
                // Imprimer les noms des colonnes
                Console.WriteLine("Column Names:");
                foreach (string colName in dataTable.Columns)
                {
                    Console.WriteLine(colName);
                }

                // Imprimer les valeurs
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
            
            // Enregistrer le résultat
            workbook.Save("CellsDataTableFactoryGetInstanceWithICollectionBooleanDemo.xlsx");
        }
    }
}
```

### Voir aussi

* interface [ICellsDataTable](../../icellsdatatable/)
* class [CellsDataTableFactory](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


