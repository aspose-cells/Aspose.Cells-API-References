---
title: "DataSorter.Sort"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo DataSorter. Ordina i dati dell'area"
type: docs
url: /it/net/aspose.cells/datasorter/sort/
---
## Sort(Cells, int, int, int, int) {#sort_2}

Ordina i dati dell'area.

```csharp
public int[] Sort(Cells cells, int startRow, int startColumn, int endRow, int endColumn)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| celle | Celle | Le celle contengono l'area dei dati. |
| startRow | Int32 | La riga iniziale dell'area. |
| startColumn | Int32 | La colonna iniziale dell'area. |
| endRow | Int32 | La riga finale dell'area. |
| endColumn | Int32 | La colonna finale dell'area. |

### Valore di ritorno

gli indici originali (posizione assoluta, ad esempio, la colonna A è 0, B è 1, ...) delle righe/colonne ordinate. Se nessuna riga/colonna deve essere spostata da questa operazione di ordinamento, verrà restituito null.

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DataSorterMethodSortWithCellsInt32Int32Int32Int32Demo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Cells cells = wb.Worksheets[0].Cells;
            
            // Popola dati di esempio
            for (int i = 0; i < 6; i++)
            {
                cells[i, 0].PutValue(6 - i);
            }
            
            // Nascondi una riga per dimostrare l'ordinamento con righe nascoste
            cells.Rows[1].IsHidden = true;
            
            // Crea e configura l'ordinatore
            DataSorter sorter = wb.DataSorter;
            sorter.AddKey(0, SortOrder.Ascending);
            
            // Dimostra il metodo Sort con parametri Cells e Int32
            sorter.Sort(cells, 0, 0, 5, 0);
            
            // Stampa i risultati sulla console
            for (int i = 0; i < 6; i++)
            {
                Console.WriteLine($"Cell A{i+1}: {cells[i, 0].IntValue}");
            }
            Console.WriteLine($"Is row 2 hidden? {cells.Rows[1].IsHidden}");
        }
    }
}
```

### Vedi anche

* class [Cells](../../cells/)
* class [DataSorter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Sort(Cells, CellArea) {#sort_1}

Ordina i dati dell'area.

```csharp
public int[] Sort(Cells cells, CellArea area)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| celle | Celle | Le celle contengono l'area dei dati. |
| area | CellArea | L'area necessaria per l'ordinamento |

### Valore di ritorno

gli indici originali (posizione assoluta, ad esempio, la colonna A è 0, B è 1, ...) delle righe/colonne ordinate. Se nessuna riga/colonna deve essere spostata da questa operazione di ordinamento, verrà restituito null.

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DataSorterMethodSortWithCellsCellAreaDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro con dati di esempio
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi dati di esempio
            worksheet.Cells["A1"].PutValue("Year");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["A2"].PutValue(1995);
            worksheet.Cells["B2"].PutValue(10000);
            worksheet.Cells["A3"].PutValue(1996);
            worksheet.Cells["B3"].PutValue(15000);
            worksheet.Cells["A4"].PutValue(1997);
            worksheet.Cells["B4"].PutValue(12000);
            worksheet.Cells["A5"].PutValue(1998);
            worksheet.Cells["B5"].PutValue(18000);

            // Crea un ordinatore di dati
            DataSorter dataSorter = workbook.DataSorter;
            dataSorter.HasHeaders = true;
            dataSorter.Key1 = 0; // Sort by first column (Year)
            dataSorter.Order1 = SortOrder.Descending;

            // Definisci area di ordinamento
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.StartColumn = 0;
            area.EndRow = 4;
            area.EndColumn = 1;

            // Esegui ordinamento
            dataSorter.Sort(worksheet.Cells, area);

            // Salva la cartella di lavoro
            workbook.Save("SortedData.xlsx");
        }
    }
}
```

### Vedi anche

* class [Cells](../../cells/)
* struct [CellArea](../../cellarea/)
* class [DataSorter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Sort() {#sort}

Ordina i dati nell'intervallo.

```csharp
public int[] Sort()
```

### Valore di ritorno

gli indici originali (posizione assoluta, ad esempio, la colonna A è 0, B è 1, ...) delle righe/colonne ordinate. Se nessuna riga/colonna deve essere spostata da questa operazione di ordinamento, verrà restituito null.

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DataSorterMethodSortDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro con dati di esempio
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi dati di esempio da ordinare
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("C");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue("A");
            worksheet.Cells["B3"].PutValue(10);
            worksheet.Cells["A4"].PutValue("B");
            worksheet.Cells["B4"].PutValue(20);

            // Crea un oggetto tabella/elenco
            int index = worksheet.ListObjects.Add(0, 0, 3, 1, true);
            Aspose.Cells.Tables.ListObject table = worksheet.ListObjects[index];
            table.ShowTotals = true;

            // Ordina i dati per la prima colonna
            table.AutoFilter.Sorter.Sort();

            // Salva la cartella di lavoro
            workbook.Save("SortedData.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Vedi anche

* class [DataSorter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


