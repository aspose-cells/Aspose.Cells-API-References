---
title: "DataSorter.AddKey"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo DataSorter. Aggiunge l'indice della colonna ordinata e l'ordine di ordinamento"
type: docs
url: /it/net/aspose.cells/datasorter/addkey/
---
## AddKey(int, SortOrder) {#addkey_1}

Aggiunge l'indice della colonna ordinata e l'ordine di ordinamento.

```csharp
public void AddKey(int key, SortOrder order)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| chiave | Int32 | L'indice della colonna ordinata (posizione assoluta, la colonna A è 0, B è 1, ...) |
| ordine | SortOrder | L'ordine di ordinamento |

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DataSorterMethodAddKeyWithInt32SortOrderDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Dati di esempio
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue("Alice");
            worksheet.Cells["B3"].PutValue(25);
            worksheet.Cells["A4"].PutValue("Bob");
            worksheet.Cells["B4"].PutValue(35);

            // Aggiungi chiave di ordinamento per la colonna B (indice 1) con ordine crescente
            workbook.DataSorter.AddKey(1, SortOrder.Ascending);
            
            // Ordina l'intervallo di dati (A1:B4)
            workbook.DataSorter.Sort(worksheet.Cells, 0, 0, 3, 1);

            // Genera i valori ordinati
            Console.WriteLine("Sorted by Age (Ascending):");
            for (int i = 1; i <= 3; i++)
            {
                Console.WriteLine($"{worksheet.Cells[$"A{i+1}"].StringValue}: {worksheet.Cells[$"B{i+1}"].IntValue}");
            }
        }
    }
}
```

### Vedi anche

* enum [SortOrder](../../sortorder/)
* class [DataSorter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## AddKey(int, SortOrder, string) {#addkey_2}

Aggiunge l'indice di colonna ordinata e l'ordine di ordinamento con un elenco di ordinamento personalizzato.

```csharp
public void AddKey(int key, SortOrder order, string customList)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| chiave | Int32 | L'indice della colonna ordinata (posizione assoluta, la colonna A è 0, B è 1, ...) |
| ordine | SortOrder | L'ordine di ordinamento. |
| customList | String | L'elenco di ordinamento personalizzato. |

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DataSorterMethodAddKeyWithInt32SortOrderStringDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Dati di esempio da ordinare
            worksheet.Cells["A1"].PutValue("Header");
            worksheet.Cells["A2"].PutValue("ddd");
            worksheet.Cells["A3"].PutValue("aaa");
            worksheet.Cells["A4"].PutValue("ccc");
            worksheet.Cells["A5"].PutValue("bbb");

            // Crea ordinatore di dati e aggiungi chiave di ordinamento personalizzata
            DataSorter sorter = workbook.DataSorter;
            sorter.AddKey(0, SortOrder.Ascending, "aaa,ddd,ccc,bbb");
            sorter.HasHeaders = true;

            // Ordina i dati
            sorter.Sort(worksheet.Cells, CellArea.CreateCellArea("A1", "A5"));

            // Salva il risultato
            workbook.Save("output.xlsx");
        }
    }
}
```

### Vedi anche

* enum [SortOrder](../../sortorder/)
* class [DataSorter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## AddKey(int, SortOnType, SortOrder, object) {#addkey}

Aggiunge l'indice di colonna ordinata e l'ordine di ordinamento con un elenco di ordinamento personalizzato.

```csharp
public void AddKey(int key, SortOnType type, SortOrder order, object customList)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| chiave | Int32 | L'indice della colonna ordinata (posizione assoluta, la colonna A è 0, B è 1, ...) |
| type | SortOnType | Il tipo di valore ordinato. |
| ordine | SortOrder | L'ordine di ordinamento. |
| customList | Object | L'elenco di ordinamento personalizzato. |

### Osservazioni

Se il tipo è SortOnType.CellColor o SortOnType.FontColor, la customList è Color.

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class DataSorterMethodAddKeyWithInt32SortOnTypeSortOrderObjectDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio al foglio di lavoro
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue("Alice");
            worksheet.Cells["B3"].PutValue(25);
            worksheet.Cells["A4"].PutValue("Bob");
            worksheet.Cells["B4"].PutValue(35);

            // Crea un ordinatore di dati
            DataSorter sorter = workbook.DataSorter;
            sorter.HasHeaders = true;

            try
            {
                // Chiama AddKey con i parametri: (Int32, SortOnType, SortOrder, Object)
                sorter.AddKey(
                    1,                          // Column index (B column)
                    SortOnType.Value,           // Sort on values (fixed from Values to Value)
                    SortOrder.Ascending,        // Sort order
                    null                        // Custom list (null for default)
                );

                // Definisci l'intervallo da ordinare
                CellArea area = new CellArea();
                area.StartRow = 0;
                area.StartColumn = 0;
                area.EndRow = 3;
                area.EndColumn = 1;

                // Ordina i dati
                sorter.Sort(worksheet.Cells, area);

                Console.WriteLine("Data sorted successfully using AddKey with parameters (Int32, SortOnType, SortOrder, Object)");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing AddKey method: {ex.Message}");
            }

            // Salva il risultato
            workbook.Save("DataSorterMethodAddKeyWithInt32SortOnTypeSortOrderObjectDemo.xlsx");
        }
    }
}
```

### Vedi anche

* enum [SortOnType](../../sortontype/)
* enum [SortOrder](../../sortorder/)
* class [DataSorter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## AddKey(int, SortOrder, string[]) {#addkey_3}

Aggiunge l'indice di colonna ordinata e l'ordine di ordinamento con un elenco di ordinamento personalizzato.

```csharp
public void AddKey(int key, SortOrder order, string[] customList)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| chiave | Int32 | L'indice della colonna ordinata (posizione assoluta, la colonna A è 0, B è 1, ...) |
| ordine | SortOrder | L'ordine di ordinamento. |
| customList | String[] | L'elenco di ordinamento personalizzato. |

### Vedi anche

* enum [SortOrder](../../sortorder/)
* class [DataSorter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


