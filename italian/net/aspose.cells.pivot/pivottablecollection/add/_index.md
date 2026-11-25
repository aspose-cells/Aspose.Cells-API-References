---
title: "PivotTableCollection.Add"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo PivotTableCollection. Aggiunge una nuova PivotTable moderna (da Excel 2007) nella posizione di riga e colonna del foglio di lavoro specificata con opzioni predefinite"
type: docs
url: /it/net/aspose.cells.pivot/pivottablecollection/add/
---
## Add(string, string) {#add_2}

Aggiunge un nuovo PivotTable moderno (dal 2007) nella posizione di riga e colonna del foglio di lavoro specificato con le opzioni predefinite.

```csharp
public PivotTable Add(string sourceData, string cellName)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| sourceData | String | L'intervallo di celle dati per la nuova PivotTable. Esempio: Sheet1!A1:C8 |
| cellName | String | Il nome della cella in alto a sinistra per la destinazione della PivotTable. |

### Valore di ritorno

L'istanza della PivotTable appena creata.

### Vedi anche

* class [PivotTable](../../pivottable/)
* class [PivotTableCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## Add(string, string, PivotTableCreateOptions) {#add_3}

Aggiunge un nuovo PivotTable moderno (dal 2007) nella posizione di riga e colonna del foglio di lavoro specificato con le opzioni predefinite.

```csharp
public PivotTable Add(string sourceData, string cellName, PivotTableCreateOptions options)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| sourceData | String | L'intervallo di celle dati per la nuova PivotTable. Esempio: Sheet1!A1:C8 |
| cellName | String | Il nome della cella in alto a sinistra per la destinazione della PivotTable. |
| opzioni | PivotTableCreateOptions | Le opzioni per la creazione della PivotTable. |

### Valore di ritorno

L'istanza della PivotTable appena creata.

### Vedi anche

* class [PivotTable](../../pivottable/)
* class [PivotTableCreateOptions](../../pivottablecreateoptions/)
* class [PivotTableCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## Add(string, int, int) {#add}

Aggiunge un nuovo PivotTable moderno (dal 2007) nella posizione di riga e colonna del foglio di lavoro specificato con le opzioni predefinite.

```csharp
public PivotTable Add(string sourceData, int row, int column)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| sourceData | String | L'intervallo di celle dati per la nuova PivotTable. Esempio: Sheet1!A1:C8 |
| riga | Int32 | L'indice di riga basato su zero dell'angolo in alto a sinistra per la destinazione della PivotTable. |
| colonna | Int32 | L'indice di colonna basato su zero dell'angolo in alto a sinistra per la destinazione della PivotTable. |

### Valore di ritorno

L'istanza della PivotTable appena creata.

### Vedi anche

* class [PivotTable](../../pivottable/)
* class [PivotTableCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## Add(string, int, int, PivotTableCreateOptions) {#add_1}

Aggiunge un nuovo PivotTable nella posizione di riga e colonna del foglio di lavoro specificato.

```csharp
public PivotTable Add(string sourceData, int row, int column, PivotTableCreateOptions options)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| sourceData | String | L'intervallo di celle dati per la nuova PivotTable. Esempio: Sheet1!A1:C8 |
| riga | Int32 | L'indice di riga basato su zero dell'angolo in alto a sinistra per la destinazione della PivotTable. |
| colonna | Int32 | L'indice di colonna basato su zero dell'angolo in alto a sinistra per la destinazione della PivotTable. |
| opzioni | PivotTableCreateOptions | Opzioni di creazione della PivotTable. |

### Valore di ritorno

L'istanza della PivotTable appena creata.

### Vedi anche

* class [PivotTable](../../pivottable/)
* class [PivotTableCreateOptions](../../pivottablecreateoptions/)
* class [PivotTableCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## Add(string, string, string) {#add_9}

Aggiunge una nuova PivotTable con layout e stile legacy di Excel 97-2003.

```csharp
[Obsolete("Use PivotTableCollection.Add(string, int, int, PivotTableCreateOptions) overload instead. This method is equivalent to setting NewPivotTableOptions.IsXlsClassic = true.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int Add(string sourceData, string destCellName, string tableName)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| sourceData | String | I dati per la cache della nuova PivotTable. |
| destCellName | String | La cella nell'angolo in alto a sinistra dell'intervallo di destinazione del report PivotTable. |
| tableName | String | Il nome del nuovo report PivotTable. |

### Valore di ritorno

L'indice in questo elenco di PivotTable.

### Osservazioni

NOTA: Questo metodo è obsoleto. È equivalente a chiamare PivotTableCollection.Add(string, int, int, PivotTableCreateOptions) con `NewPivotTableOptions.IsXlsClassic = true`. Si prega di utilizzare invece la sovraccarico di PivotTableCollection.Add(string, int, int, PivotTableCreateOptions). Questo metodo sarà rimosso 12 mesi dopo settembre 2026. Ci scusiamo per qualsiasi inconveniente.

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableCollectionMethodAddWithStringStringStringDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro dal CSV di origine
            Workbook workbook = new Workbook();
            Worksheet sourceSheet = workbook.Worksheets[0];
            sourceSheet.Name = "SourceData";
            
            // Aggiungi dati di esempio
            sourceSheet.Cells["A1"].PutValue("Category");
            sourceSheet.Cells["B1"].PutValue("Value");
            sourceSheet.Cells["A2"].PutValue("A");
            sourceSheet.Cells["B2"].PutValue(10);
            sourceSheet.Cells["A3"].PutValue("B");
            sourceSheet.Cells["B3"].PutValue(20);
            sourceSheet.Cells["A4"].PutValue("A");
            sourceSheet.Cells["B4"].PutValue(30);

            // Crea foglio di lavoro della tabella pivot
            Worksheet pivotSheet = workbook.Worksheets.Add("PivotTable");
            
            // Ottieni l'intervallo di dati di origine
            Aspose.Cells.Range sourceRange = sourceSheet.Cells.MaxDisplayRange;
            string sourceData = String.Format("=SourceData!{0}", sourceRange.Address);
            
            // Aggiungi una pivot table usando parametri String, String, String
            PivotTableCollection pivotTables = pivotSheet.PivotTables;
            int pivotIndex = pivotTables.Add(sourceData, "A1", "MyPivotTable");
            
            // Configura la tabella pivot
            PivotTable pivotTable = pivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Category");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Value");
            
            // Salva la cartella di lavoro
            workbook.Save("PivotTableDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [PivotTableCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## Add(string, string, string, bool) {#add_10}

Aggiunge una nuova PivotTable con layout e stile legacy di Excel 97-2003.

```csharp
[Obsolete("Use PivotTableCollection.Add(string, string, PivotTableCreateOptions) overload instead. This method is equivalent to setting NewPivotTableOptions.IsXlsClassic = true.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int Add(string sourceData, string destCellName, string tableName, bool useSameSource)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| sourceData | String | I dati per la cache della nuova PivotTable. |
| destCellName | String | La cella nell'angolo in alto a sinistra dell'intervallo di destinazione del report PivotTable. |
| tableName | String | Il nome del nuovo report PivotTable. |
| useSameSource | Booleano | Indica se utilizzare la stessa origine dati quando un'altra pivot table esistente ha già usato questa origine dati. Se la proprietà è true, risparmierà memoria. |

### Valore di ritorno

L'indice della nuova cache aggiunta.

### Osservazioni

NOTA: Questo metodo è obsoleto. È equivalente a chiamare PivotTableCollection.Add(string, int, int, PivotTableCreateOptions) con `NewPivotTableOptions.IsXlsClassic = true`. Si prega di utilizzare invece la sovraccarico di PivotTableCollection.Add(string, int, int, PivotTableCreateOptions). Questo metodo sarà rimosso 12 mesi dopo settembre 2026. Ci scusiamo per qualsiasi inconveniente.

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotTableCollectionMethodAddWithStringStringStringBooleanDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio per la tabella pivot
            Cells cells = worksheet.Cells;
            cells["A1"].Value = "Fruit";
            cells["B1"].Value = "Quantity";
            cells["A2"].Value = "Apple";
            cells["B2"].Value = 10;
            cells["A3"].Value = "Orange";
            cells["B3"].Value = 15;
            cells["A4"].Value = "Banana";
            cells["B4"].Value = 20;

            // Definisci i parametri per il metodo Add
            string sourceData = "A1:B4";
            string destCellName = "E5";
            string tableName = "FruitPivotTable";
            bool useSameSource = true;

            try
            {
                // Chiama il metodo Add con i parametri (String, String, String, Boolean)
                int index = worksheet.PivotTables.Add(sourceData, destCellName, tableName, useSameSource);
                
                Console.WriteLine($"Pivot table added successfully at index: {index}");
                Console.WriteLine($"Pivot table name: {worksheet.PivotTables[index].Name}");
                Console.WriteLine($"Pivot table location: {worksheet.PivotTables[index].TableRange1}");

                // Configura la tabella pivot
                PivotTable pivotTable = worksheet.PivotTables[index];
                pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
                pivotTable.AddFieldToArea(PivotFieldType.Data, "Quantity");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Add method: {ex.Message}");
            }
            
            // Salva la cartella di lavoro
            workbook.Save("PivotTableAddDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [PivotTableCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## Add(string, int, int, string) {#add_6}

Aggiunge una nuova PivotTable con layout e stile legacy di Excel 97-2003.

```csharp
[Obsolete("Use PivotTableCollection.Add(string, int, int, PivotTableCreateOptions) overload instead. This method is equivalent to setting NewPivotTableOptions.IsXlsClassic = true.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int Add(string sourceData, int row, int column, string tableName)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| sourceData | String | L'intervallo di celle dati per la nuova PivotTable.Esempio : Sheet1!A1:C8 |
| riga | Int32 | Indice di riga della cella nell'angolo in alto a sinistra dell'intervallo di destinazione del report PivotTable. |
| colonna | Int32 | Indice di colonna della cella nell'angolo in alto a sinistra dell'intervallo di destinazione del report PivotTable. |
| tableName | String | Il nome del nuovo report PivotTable. |

### Valore di ritorno

L'indice in questo elenco di PivotTable.

### Osservazioni

NOTA: Questo metodo è obsoleto. È equivalente a chiamare PivotTableCollection.Add(string, int, int, PivotTableCreateOptions) con `NewPivotTableOptions.IsXlsClassic = true`. Si prega di utilizzare invece la sovraccarico di PivotTableCollection.Add(string, int, int, PivotTableCreateOptions). Questo metodo sarà rimosso 12 mesi dopo settembre 2026. Ci scusiamo per qualsiasi inconveniente.

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableCollectionMethodAddWithStringInt32Int32StringDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Aggiungi un foglio di lavoro per i dati
            Worksheet dataWorksheet = workbook.Worksheets[0];
            dataWorksheet.Name = "Data";
            
            // Aggiungi dati di esempio
            dataWorksheet.Cells["A1"].PutValue("Category");
            dataWorksheet.Cells["B1"].PutValue("Product");
            dataWorksheet.Cells["C1"].PutValue("Sales");
            
            dataWorksheet.Cells["A2"].PutValue("Electronics");
            dataWorksheet.Cells["B2"].PutValue("Laptop");
            dataWorksheet.Cells["C2"].PutValue(1000);
            
            dataWorksheet.Cells["A3"].PutValue("Electronics");
            dataWorksheet.Cells["B3"].PutValue("Phone");
            dataWorksheet.Cells["C3"].PutValue(800);
            
            dataWorksheet.Cells["A4"].PutValue("Furniture");
            dataWorksheet.Cells["B4"].PutValue("Chair");
            dataWorksheet.Cells["C4"].PutValue(200);
            
            // Aggiungi un foglio di lavoro per la pivot table
            Worksheet pivotWorksheet = workbook.Worksheets.Add("PivotTable");
            
            // Aggiungi una pivot table usando il metodo Add con parametri (String, Int32, Int32, String)
            string pivotDataRange = "Data!A1:C4";
            int row = 0;
            int column = 0;
            string tableName = "SalesPivotTable";
            
            int pivotIndex = pivotWorksheet.PivotTables.Add(pivotDataRange, row, column, tableName);
            
            // Accedi alla tabella pivot
            PivotTable pivotTable = pivotWorksheet.PivotTables[pivotIndex];
            
            // Aggiungi campi alla tabella pivot
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Category");
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            
            // Imposta la funzione di consolidamento
            pivotTable.DataFields[0].Function = ConsolidationFunction.Sum;
            
            // Aggiorna e calcola i dati della tabella pivot
            pivotTable.RefreshData();
            pivotTable.CalculateData();
            
            // Salva la cartella di lavoro
            workbook.Save("PivotTableDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [PivotTableCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## Add(string, int, int, string, bool) {#add_7}

Aggiunge una nuova PivotTable con layout e stile legacy di Excel 97-2003.

```csharp
[Obsolete("Use PivotTableCollection.Add(string, int, int, PivotTableCreateOptions) overload instead. This method is equivalent to setting NewPivotTableOptions.IsXlsClassic = true.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int Add(string sourceData, int row, int column, string tableName, bool useSameSource)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| sourceData | String | L'intervallo di celle dati per la nuova PivotTable.Esempio : Sheet1!A1:C8 |
| riga | Int32 | Indice di riga della cella nell'angolo in alto a sinistra dell'intervallo di destinazione del report PivotTable. |
| colonna | Int32 | Indice di colonna della cella nell'angolo in alto a sinistra dell'intervallo di destinazione del report PivotTable. |
| tableName | String | Il nome del nuovo report PivotTable. |
| useSameSource | Booleano | Indica se utilizzare la stessa origine dati quando un'altra pivot table esistente ha già usato questa origine dati. Se la proprietà è true, risparmierà memoria. |

### Valore di ritorno

L'indice della nuova cache aggiunta.

### Osservazioni

NOTA: Questo metodo è obsoleto. È equivalente a chiamare PivotTableCollection.Add(string, int, int, PivotTableCreateOptions) con `NewPivotTableOptions.IsXlsClassic = true`. Si prega di utilizzare invece la sovraccarico di PivotTableCollection.Add(string, int, int, PivotTableCreateOptions). Questo metodo sarà rimosso 12 mesi dopo settembre 2026. Ci scusiamo per qualsiasi inconveniente.

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotTableCollectionMethodAddWithStringInt32Int32StringBooleanDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi dati di esempio per la tabella pivot
            Cells cells = worksheet.Cells;
            cells["A1"].PutValue("Product");
            cells["B1"].PutValue("Region");
            cells["C1"].PutValue("Sales");
            
            cells["A2"].PutValue("Product1");
            cells["B2"].PutValue("North");
            cells["C2"].PutValue(1000);
            
            cells["A3"].PutValue("Product2");
            cells["B3"].PutValue("South");
            cells["C3"].PutValue(2000);
            
            cells["A4"].PutValue("Product3");
            cells["B4"].PutValue("East");
            cells["C4"].PutValue(3000);
            
            // Definisci l'intervallo di dati
            string sourceData = "A1:C4";
            
            try
            {
                // Chiama il metodo Add con i parametri: (String sourceData, Int32 row, Int32 column, String tableName, Boolean useSameSource)
                int index = worksheet.PivotTables.Add(sourceData, 6, 0, "PivotTable1", false);
                
                Console.WriteLine("Pivot table added successfully at index: " + index);
                
                // Accedi alla pivot table appena creata
                PivotTable pivotTable = worksheet.PivotTables[index];
                
                // Configura la tabella pivot
                pivotTable.AddFieldToArea(PivotFieldType.Row, 0); // Product as row
                pivotTable.AddFieldToArea(PivotFieldType.Column, 1); // Region as column
                pivotTable.AddFieldToArea(PivotFieldType.Data, 2); // Sales as data
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Add method: {ex.Message}");
            }
            
            // Salva il risultato
            workbook.Save("PivotTableAddDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [PivotTableCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## Add(string, int, int, string, bool, bool) {#add_8}

Aggiunge una nuova PivotTable con layout e stile legacy di Excel 97-2003.

```csharp
[Obsolete("Use PivotTableCollection.Add(string, int, int, PivotTableCreateOptions) overload instead. This method is equivalent to setting NewPivotTableOptions.IsXlsClassic = true.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int Add(string sourceData, int row, int column, string tableName, bool useSameSource, 
    bool isXlsClassic)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| sourceData | String | L'intervallo di celle dati per la nuova PivotTable.Esempio : Sheet1!A1:C8 |
| riga | Int32 | Indice di riga della cella nell'angolo in alto a sinistra dell'intervallo di destinazione del report PivotTable. |
| colonna | Int32 | Indice di colonna della cella nell'angolo in alto a sinistra dell'intervallo di destinazione del report PivotTable. |
| tableName | String | Il nome del nuovo report PivotTable. |
| useSameSource | Booleano | Indica se utilizzare la stessa origine dati quando un'altra pivot table esistente ha già usato questa origine dati. Se la proprietà è true, risparmierà memoria. |
| isXlsClassic | Booleano | Indica se aggiungere una pivot table classica di Excel 97-2003. |

### Valore di ritorno

L'indice della nuova cache aggiunta.

### Osservazioni

NOTA: Questo metodo è obsoleto. È equivalente a chiamare PivotTableCollection.Add(string, int, int, PivotTableCreateOptions) con `NewPivotTableOptions.IsXlsClassic = true`. Si prega di utilizzare invece la sovraccarico di PivotTableCollection.Add(string, int, int, PivotTableCreateOptions). Questo metodo sarà rimosso 12 mesi dopo ottobre 2026. Ci scusiamo per qualsiasi inconveniente.

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotTableCollectionMethodAddWithStringInt32Int32StringBooleanBDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio per la tabella pivot
            Cells cells = worksheet.Cells;
            cells["A1"].PutValue("Product");
            cells["B1"].PutValue("Region");
            cells["C1"].PutValue("Sales");
            cells["A2"].PutValue("Product1");
            cells["B2"].PutValue("North");
            cells["C2"].PutValue(1000);
            cells["A3"].PutValue("Product2");
            cells["B3"].PutValue("South");
            cells["C3"].PutValue(2000);
            cells["A4"].PutValue("Product3");
            cells["B4"].PutValue("East");
            cells["C4"].PutValue(3000);
            cells["A5"].PutValue("Product4");
            cells["B5"].PutValue("West");
            cells["C5"].PutValue(4000);

            // Definisci l'intervallo di dati di origine
            string sourceData = "A1:C5";

            try
            {
                // Chiama il metodo Add con i parametri (String, Int32, Int32, String, Boolean, Boolean)
                int index = worksheet.PivotTables.Add(
                    sourceData,    // String sourceData
                    3,            // Int32 row - pivot table will start at row 3
                    0,            // Int32 column - pivot table will start at column 0
                    "PivotTable1", // String tableName
                    false,        // Boolean useSameSource
                    false         // Boolean isXlsClassic
                );

                Console.WriteLine("Pivot table added successfully at index: " + index);

                // Configura la tabella pivot
                PivotTable pivotTable = worksheet.PivotTables[index];
                pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
                pivotTable.AddFieldToArea(PivotFieldType.Column, "Region");
                pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Add method: {ex.Message}");
            }

            // Salva il risultato
            workbook.Save("PivotTableAddDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [PivotTableCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## Add(string, string, string, bool, bool) {#add_11}

Aggiunge una nuova PivotTable.

```csharp
[Obsolete("Use PivotTableCollection.Add(string, int, int, PivotTableCreateOptions) overload instead. This method is equivalent to setting NewPivotTableOptions.IsXlsClassic = true.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int Add(string sourceData, string cell, string tableName, bool useSameSource, 
    bool isXlsClassic)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| sourceData | String | L'intervallo di celle dati per la nuova PivotTable.Esempio : Sheet1!A1:C8 |
| cella | String | La cella nell'angolo in alto a sinistra dell'intervallo di destinazione del report PivotTable. |
| tableName | String | Il nome del nuovo report PivotTable. |
| useSameSource | Booleano | Indica se utilizzare la stessa origine dati quando un'altra tabella pivot esistente ha già usato questa origine dati. Se la proprietà è true, risparmierà memoria quando la stessa origine dati è stata raggruppata in un unico cache pivot. |
| isXlsClassic | Booleano | Indica se aggiungere una pivot table classica di Excel 97-2003. |

### Valore di ritorno

L'indice della nuova cache aggiunta.

### Osservazioni

NOTA: Questo metodo è obsoleto. È equivalente a chiamare PivotTableCollection.Add(string, int, int, PivotTableCreateOptions) con `NewPivotTableOptions.IsXlsClassic = true`. Si prega di utilizzare invece la sovraccarico di PivotTableCollection.Add(string, int, int, PivotTableCreateOptions). Questo metodo sarà rimosso 12 mesi dopo ottobre 2026. Ci scusiamo per qualsiasi inconveniente.

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableCollectionMethodAddWithStringStringStringBooleanBooleDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Popola dati di esempio
            Cells cells = worksheet.Cells;
            cells["A1"].PutValue("Category");
            cells["B1"].PutValue("Product");
            cells["C1"].PutValue("Sales");
            
            for (int i = 2; i <= 10; i++)
            {
                cells["A" + i].PutValue("Cat" + (i % 3 + 1));
                cells["B" + i].PutValue("Prod" + i);
                cells["C" + i].PutValue(i * 100);
            }

            // Aggiungi una tabella pivot con i parametri specificati
            int pivotTableIndex = worksheet.PivotTables.Add("=A1:C10", "E1", "SalesPivot", false, false);
            Aspose.Cells.Pivot.PivotTable pivotTable = worksheet.PivotTables[pivotTableIndex];

            // Configura la tabella pivot
            pivotTable.AddFieldToArea(Aspose.Cells.Pivot.PivotFieldType.Row, 0); // Category as row
            pivotTable.AddFieldToArea(Aspose.Cells.Pivot.PivotFieldType.Data, 2); // Sum of Sales
            
            workbook.Save("PivotTableDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [PivotTableCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## Add(PivotTable, string, string) {#add_5}

Aggiunge un nuovo PivotTable basato su un altro PivotTable.

```csharp
public int Add(PivotTable pivotTable, string destCellName, string tableName)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| pivotTable | PivotTable | La pivotTable di origine. |
| destCellName | String | La cella nell'angolo in alto a sinistra dell'intervallo di destinazione del report PivotTable. |
| tableName | String | Il nome del nuovo report PivotTable. |

### Valore di ritorno

L'indice della nuova PivotTable aggiunta.

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotTableCollectionMethodAddWithPivotTableStringStringDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio per la tabella pivot
            Cells cells = worksheet.Cells;
            cells["A1"].Value = "Fruit";
            cells["B1"].Value = "Quantity";
            cells["A2"].Value = "Apple";
            cells["B2"].Value = 10;
            cells["A3"].Value = "Orange";
            cells["B3"].Value = 5;
            cells["A4"].Value = "Banana";
            cells["B4"].Value = 7;

            // Crea una tabella pivot dall'intervallo di dati
            PivotTableCollection pivotTables = worksheet.PivotTables;
            int pivotIndex = pivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable sourcePivotTable = pivotTables[pivotIndex];

            try
            {
                // Chiama il metodo Add con i parametri (PivotTable, String, String)
                int newPivotIndex = pivotTables.Add(sourcePivotTable, "E10", "PivotTable2");
                Console.WriteLine($"New pivot table added at index: {newPivotIndex}");

                // Salva la cartella di lavoro per mostrare l'effetto
                workbook.Save("PivotTableCollectionMethodAddWithPivotTableStringStringDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Add method: {ex.Message}");
            }
        }
    }
}
```

### Vedi anche

* class [PivotTable](../../pivottable/)
* class [PivotTableCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## Add(PivotTable, int, int, string) {#add_4}

Aggiunge un nuovo PivotTable basato su un altro PivotTable.

```csharp
public int Add(PivotTable pivotTable, int row, int column, string tableName)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| pivotTable | PivotTable | La pivotTable di origine. |
| riga | Int32 | Indice di riga della cella nell'angolo in alto a sinistra dell'intervallo di destinazione del report PivotTable. |
| colonna | Int32 | Indice di colonna della cella nell'angolo in alto a sinistra dell'intervallo di destinazione del report PivotTable. |
| tableName | String | Il nome del nuovo report PivotTable. |

### Valore di ritorno

L'indice della nuova PivotTable aggiunta.

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotTableCollectionMethodAddWithPivotTableInt32Int32StringDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio per la tabella pivot
            Cells cells = worksheet.Cells;
            cells["A1"].Value = "Fruit";
            cells["B1"].Value = "Quantity";
            cells["A2"].Value = "Apple";
            cells["B2"].Value = 10;
            cells["A3"].Value = "Orange";
            cells["B3"].Value = 5;
            cells["A4"].Value = "Banana";
            cells["B4"].Value = 7;

            // Crea una tabella pivot di origine
            PivotTableCollection pivotTables = worksheet.PivotTables;
            int pivotIndex = pivotTables.Add("A1:B4", "C3", "SourcePivotTable");
            PivotTable sourcePivotTable = pivotTables[pivotIndex];
            sourcePivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            sourcePivotTable.AddFieldToArea(PivotFieldType.Data, "Quantity");

            try
            {
                // Chiama il metodo Add con i parametri (PivotTable, Int32, Int32, String)
                int newPivotIndex = pivotTables.Add(sourcePivotTable, 10, 5, "NewPivotTable");
                Console.WriteLine($"New pivot table added at index: {newPivotIndex}");

                // Salva la cartella di lavoro per mostrare l'effetto
                workbook.Save("PivotTableCollectionMethodAddWithPivotTableInt32Int32StringDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Add method: {ex.Message}");
            }
        }
    }
}
```

### Vedi anche

* class [PivotTable](../../pivottable/)
* class [PivotTableCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## Add(string[], bool, PivotPageFields, string, string) {#add_13}

Aggiunge un nuovo oggetto PivotTable alla raccolta con più intervalli di consolidamento come origine dati.

```csharp
public int Add(string[] sourceData, bool isAutoPage, PivotPageFields pageFields, 
    string destCellName, string tableName)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| sourceData | String[] | Gli intervalli di consolidamento multipli, come {"Sheet1!A1:C8","Sheet2!A1:B8"} |
| isAutoPage | Booleano | Indica se creare automaticamente un campo di pagina singolo. Se true, il parametro pageFields seguente sarà ignorato. |
| pageFields | PivotPageFields | Gli elementi del campo di pagina pivot. |
| destCellName | String | destCellName Il nome del nuovo report PivotTable. |
| tableName | String | Il nome del nuovo report PivotTable. |

### Valore di ritorno

L'indice della nuova PivotTable aggiunta.

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotTableCollectionMethodAddWithStringBooleanPivotPageFieldsDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio per la tabella pivot
            Cells cells = worksheet.Cells;
            cells["A1"].Value = "Product";
            cells["B1"].Value = "Region";
            cells["C1"].Value = "Sales";
            cells["A2"].Value = "Product1";
            cells["B2"].Value = "North";
            cells["C2"].Value = 1000;
            cells["A3"].Value = "Product2";
            cells["B3"].Value = "South";
            cells["C3"].Value = 2000;
            cells["A4"].Value = "Product3";
            cells["B4"].Value = "East";
            cells["C4"].Value = 3000;

            // Definisci l'intervallo di dati
            string[] sourceData = { "A1:C4" };
            bool isAutoPage = true;
            PivotPageFields pageFields = new PivotPageFields();
            string destCellName = "E5";
            string tableName = "PivotTable1";

            try
            {
                // Chiama il metodo Add con i parametri specificati
                int index = worksheet.PivotTables.Add(sourceData, isAutoPage, pageFields, destCellName, tableName);
                
                Console.WriteLine($"Pivot table added successfully at index: {index}");
                
                // Accedi alla pivot table appena creata
                PivotTable pivotTable = worksheet.PivotTables[index];
                
                // Configura i campi della tabella pivot
                pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
                pivotTable.AddFieldToArea(PivotFieldType.Column, "Region");
                pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Add method: {ex.Message}");
            }
            
            // Salva la cartella di lavoro
            workbook.Save("PivotTableAddDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [PivotPageFields](../../pivotpagefields/)
* class [PivotTableCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## Add(string[], bool, PivotPageFields, int, int, string) {#add_12}

Aggiunge un nuovo oggetto PivotTable alla raccolta con più intervalli di consolidamento come origine dati.

```csharp
public int Add(string[] sourceData, bool isAutoPage, PivotPageFields pageFields, int row, 
    int column, string tableName)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| sourceData | String[] | Gli intervalli di consolidamento multipli, come {"Sheet1!A1:C8","Sheet2!A1:B8"} |
| isAutoPage | Booleano | Indica se creare automaticamente un campo di pagina singolo. Se true, il parametro pageFields seguente sarà ignorato |
| pageFields | PivotPageFields | Gli elementi del campo di pagina pivot. |
| riga | Int32 | Indice di riga della cella nell'angolo in alto a sinistra dell'intervallo di destinazione del report PivotTable. |
| colonna | Int32 | Indice di colonna della cella nell'angolo in alto a sinistra dell'intervallo di destinazione del report PivotTable. |
| tableName | String | Il nome del nuovo report PivotTable. |

### Valore di ritorno

L'indice della nuova PivotTable aggiunta.

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotTableCollectionMethodAddWithStringBooleanPivotPageFieldsDemo1
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio per la tabella pivot
            Cells cells = worksheet.Cells;
            cells["A1"].Value = "Product";
            cells["B1"].Value = "Region";
            cells["C1"].Value = "Sales";
            
            cells["A2"].Value = "Product1";
            cells["B2"].Value = "North";
            cells["C2"].Value = 1000;
            
            cells["A3"].Value = "Product2";
            cells["B3"].Value = "South";
            cells["C3"].Value = 2000;
            
            cells["A4"].Value = "Product3";
            cells["B4"].Value = "East";
            cells["C4"].Value = 3000;
            
            cells["A5"].Value = "Product1";
            cells["B5"].Value = "West";
            cells["C5"].Value = 4000;
            
            cells["A6"].Value = "Product2";
            cells["B6"].Value = "North";
            cells["C6"].Value = 5000;

            // Definisci i parametri per il metodo Add
            string[] sourceData = { "A1:C6" };
            bool isAutoPage = true;
            PivotPageFields pageFields = new PivotPageFields();
            int row = 8;
            int column = 1;
            string tableName = "PivotTable1";

            try
            {
                // Chiama il metodo Add con i parametri specificati
                int index = worksheet.PivotTables.Add(sourceData, isAutoPage, pageFields, row, column, tableName);
                
                Console.WriteLine($"Pivot table added successfully at index: {index}");
                
                // Configura la tabella pivot
                PivotTable pivotTable = worksheet.PivotTables[index];
                pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
                pivotTable.AddFieldToArea(PivotFieldType.Column, "Region");
                pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
                
                // Aggiorna i dati
                pivotTable.RefreshData();
                pivotTable.CalculateData();
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Add method: {ex.Message}");
            }
            
            // Salva il risultato
            workbook.Save("PivotTableAddDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [PivotPageFields](../../pivotpagefields/)
* class [PivotTableCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


