---
title: "Workbook.Replace"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Workbook. Sostituisce il valore di una cella con una nuova stringa"
type: docs
url: /it/net/aspose.cells/workbook/replace/
---
## Replace(string, string) {#replace_7}

Sostituisce il valore di una cella con una nuova stringa.

```csharp
public int Replace(string placeHolder, string newValue)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| segnaposto | String | Segnaposto cella |
| nuovoValore | String | Valore stringa da sostituire |

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodReplaceWithStringStringDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi dati di esempio alle celle
            worksheet.Cells["A1"].PutValue("Apple");
            worksheet.Cells["A2"].PutValue("Banana");
            worksheet.Cells["A3"].PutValue("Apple Orange");
            
            // Sostituisci tutte le occorrenze di "Apple" con "Mango"
            workbook.Replace("Apple", "Mango");
            
            // Salva la cartella di lavoro
            workbook.Save("ReplaceDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Replace(string, int) {#replace_4}

Sostituisce il valore di una cella con un nuovo intero.

```csharp
public int Replace(string placeHolder, int newValue)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| segnaposto | String | Segnaposto cella |
| nuovoValore | Int32 | Valore intero da sostituire |

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodReplaceWithStringInt32Demo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro e aggiungi alcuni dati di esempio
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("OriginalValue");
            worksheet.Cells["A2"].PutValue("OriginalValue");
            worksheet.Cells["A3"].PutValue("OriginalValue");
            
            // Sostituisci tutte le occorrenze di "OriginalValue" con l'intero 100
            workbook.Replace("OriginalValue", 100);
            
            // Salva la cartella di lavoro
            workbook.Save("ReplacedWorkbook.xlsx");
        }
    }
}
```

### Vedi anche

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Replace(string, double) {#replace_2}

Sostituisce il valore di una cella con un nuovo double.

```csharp
public int Replace(string placeHolder, double newValue)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| segnaposto | String | Segnaposto cella |
| nuovoValore | Double | Valore double da sostituire |

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodReplaceWithStringDoubleDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Inserisci alcuni dati di esempio nelle celle
            worksheet.Cells["A1"].PutValue("AnOldValue");
            worksheet.Cells["A2"].PutValue("AnotherOldValue");
            worksheet.Cells["A3"].PutValue("AnOldValue");
            
            // Sostituisci il testo con valore double
            double newValue = 100.0;
            workbook.Replace("AnOldValue", newValue);
            
            // Salva la cartella di lavoro
            workbook.Save("output.xlsx");
        }
    }
}
```

### Vedi anche

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Replace(string, string[], bool) {#replace_9}

Sostituisce il valore di una cella con un nuovo array di stringhe.

```csharp
public int Replace(string placeHolder, string[] newValues, bool isVertical)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| segnaposto | String | Segnaposto cella |
| newValues | String[] | Array di stringhe da sostituire |
| isVertical | Booleano | True - Verticale, False - Orizzontale |

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodReplaceWithStringStringBooleanDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi alcuni dati di esempio alle celle
            worksheet.Cells["A1"].PutValue("AnOldValue");
            worksheet.Cells["A2"].PutValue("AnOldValue");
            worksheet.Cells["A3"].PutValue("AnOldValue");
            
            // Definisci i nuovi valori con cui sostituire
            string[] newValues = new string[] { "Tom", "Alice", "Jerry" };
            
            // Sostituisci tutte le occorrenze di "AnOldValue" con i nuovi valori
            workbook.Replace("AnOldValue", newValues, true);
            
            // Salva la cartella di lavoro
            workbook.Save("ReplaceDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Replace(string, int[], bool) {#replace_5}

Sostituisce i valori delle celle con un array di interi.

```csharp
public int Replace(string placeHolder, int[] newValues, bool isVertical)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| segnaposto | String | Segnaposto cella |
| newValues | Int32[] | Array di interi da sostituire |
| isVertical | Booleano | True - Verticale, False - Orizzontale |

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodReplaceWithStringInt32ArrayBooleanDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi alcuni dati di esempio alle celle
            worksheet.Cells["A1"].PutValue("OldValue");
            worksheet.Cells["A2"].PutValue("OldValue");
            worksheet.Cells["A3"].PutValue("OtherValue");
            
            // Definisci i valori di sostituzione
            int[] newValues = new int[] { 1, 2, 3 };
            
            // Sostituisci "OldValue" con l'array di interi
            workbook.Replace("OldValue", newValues, true);
            
            // Salva la cartella di lavoro
            workbook.Save("ReplaceDemoOutput.xlsx");
        }
    }
}
```

### Vedi anche

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Replace(string, double[], bool) {#replace_3}

Sostituisce i valori delle celle con un array di double.

```csharp
public int Replace(string placeHolder, double[] newValues, bool isVertical)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| segnaposto | String | Segnaposto cella |
| newValues | Double[] | Array di double da sostituire |
| isVertical | Booleano | True - Verticale, False - Orizzontale |

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodReplaceWithStringDoubleBooleanDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi dati di esempio alle celle
            worksheet.Cells["A1"].PutValue("AnOldValue");
            worksheet.Cells["A2"].PutValue("AnOldValue");
            worksheet.Cells["A3"].PutValue("AnOldValue");
            
            // Definisci i valori di sostituzione
            double[] newValues = new double[] { 1.23, 2.56, 3.14159 };
            
            // Sostituisci tutte le occorrenze di "AnOldValue" con i nuovi valori
            workbook.Replace("AnOldValue", newValues, true);
            
            // Salva la cartella di lavoro
            workbook.Save("ReplaceDemoOutput.xlsx");
        }
    }
}
```

### Vedi anche

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Replace(string, DataTable) {#replace_6}

Sostituisce i valori delle celle con i dati da una DataTable.

```csharp
public int Replace(string placeHolder, DataTable insertTable)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| segnaposto | String | Segnaposto cella |
| insertTable | DataTable | DataTable da sostituire |

### Esempi

```csharp
using System;
using System.Data;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodReplaceWithStringDataTableDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Crea un DataTable di esempio
            DataTable dataTable = new DataTable("Customers");
            dataTable.Columns.Add("ID", typeof(int));
            dataTable.Columns.Add("Name", typeof(string));
            dataTable.Columns.Add("City", typeof(string));
            
            // Aggiungi dati di esempio al DataTable
            dataTable.Rows.Add(1, "John Doe", "New York");
            dataTable.Rows.Add(2, "Jane Smith", "London");
            dataTable.Rows.Add(3, "Mike Johnson", "Paris");
            
            // Aggiungi del testo al foglio di lavoro che sarà sostituito
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("CustomerData");
            
            // Sostituisci il testo con DataTable
            workbook.Replace("CustomerData", dataTable);
            
            // Salva la cartella di lavoro
            workbook.Save("Output.xlsx");
        }
    }
}
```

### Vedi anche

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Replace(bool, object) {#replace}

Sostituisce i valori delle celle con nuovi dati.

```csharp
public int Replace(bool boolValue, object newValue)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| boolValue | Booleano | Il valore booleano da sostituire. |
| nuovoValore | Object | Nuovo valore. Può essere una stringa, un intero, un double o un valore DateTime. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class WorkbookMethodReplaceWithBooleanObjectDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Popola alcune celle con valori booleani
            worksheet.Cells["A1"].PutValue(true);
            worksheet.Cells["A2"].PutValue(false);
            worksheet.Cells["A3"].PutValue(true);
            
            try
            {
                // Chiama il metodo Replace per sostituire tutti i valori 'true' con "REPLACED"
                int replacements = workbook.Replace(true, "REPLACED");
                
                Console.WriteLine($"Replaced {replacements} occurrences of 'true' with 'REPLACED'");
                
                // Visualizza i risultati
                Console.WriteLine("A1: " + worksheet.Cells["A1"].StringValue);
                Console.WriteLine("A2: " + worksheet.Cells["A2"].StringValue);
                Console.WriteLine("A3: " + worksheet.Cells["A3"].StringValue);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Replace method: {ex.Message}");
            }
            
            // Salva il risultato
            workbook.Save("WorkbookMethodReplaceWithBooleanObjectDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Replace(int, object) {#replace_1}

Sostituisce i valori delle celle con nuovi dati.

```csharp
public int Replace(int intValue, object newValue)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| intValue | Int32 | Il valore intero da sostituire. |
| nuovoValore | Object | Nuovo valore. Può essere una stringa, un intero, un double o un valore DateTime. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class WorkbookMethodReplaceWithInt32ObjectDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Popola alcune celle con valori interi da sostituire
            worksheet.Cells["A1"].PutValue(100);
            worksheet.Cells["A2"].PutValue(200);
            worksheet.Cells["A3"].PutValue(100);
            
            try
            {
                // Chiama il metodo Replace con i parametri (Int32, Object)
                int replacements = workbook.Replace(100, "ReplacedValue");
                
                Console.WriteLine($"Replaced {replacements} occurrences of the value 100");
                
                // Visualizza il contenuto del foglio di lavoro dopo la sostituzione
                Console.WriteLine("Cell A1: " + worksheet.Cells["A1"].StringValue);
                Console.WriteLine("Cell A2: " + worksheet.Cells["A2"].StringValue);
                Console.WriteLine("Cell A3: " + worksheet.Cells["A3"].StringValue);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Replace method: {ex.Message}");
            }
            
            // Salva il risultato
            workbook.Save("WorkbookMethodReplaceWithInt32ObjectDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Replace(string, string, ReplaceOptions) {#replace_8}

Sostituisce il valore di una cella con una nuova stringa.

```csharp
public int Replace(string placeHolder, string newValue, ReplaceOptions options)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| segnaposto | String | Segnaposto cella |
| nuovoValore | String | Valore stringa da sostituire |
| opzioni | ReplaceOptions | Le opzioni di sostituzione |

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodReplaceWithStringStringReplaceOptionsDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            sheet.Cells["A1"].PutValue("Hello World");
            sheet.Cells["A2"].PutValue("Hello Aspose");
            sheet.Cells["A3"].PutValue("Goodbye World");

            ReplaceOptions options = new ReplaceOptions
            {
                CaseSensitive = false,
                MatchEntireCellContents = false
            };

            int replacedCount = workbook.Replace("Hello", "Hi", options);

            Console.WriteLine($"Replacements made: {replacedCount}");
            workbook.Save("ReplaceDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [ReplaceOptions](../../replaceoptions/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


