---
title: "AutoFilter.Refresh"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo AutoFilter. Aggiorna gli auto filter per nascondere o mostrare le righe"
type: docs
url: /it/net/aspose.cells/autofilter/refresh/
---
## Refresh() {#refresh}

Aggiorna i filtri automatici per nascondere o mostrare le righe.

```csharp
public int[] Refresh()
```

### Valore di ritorno

Restituisce tutti gli indici delle righe nascoste.

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class AutoFilterMethodRefreshDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro con dati di esempio
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi dati di esempio
            worksheet.Cells["B6"].PutValue("Header1");
            worksheet.Cells["C6"].PutValue("Header2");
            worksheet.Cells["D6"].PutValue("Header3");
            worksheet.Cells["E6"].PutValue("Values");
            
            for (int i = 7; i <= 15; i++)
            {
                worksheet.Cells["B" + i].PutValue("Item " + (i-6));
                worksheet.Cells["E" + i].PutValue((i-6) * 100);
            }

            // Applica filtro automatico
            worksheet.AutoFilter.Range = "B6:E6";
            
            // Filtra i valori maggiori di 500
            worksheet.AutoFilter.Custom(3, FilterOperatorType.GreaterThan, 500);
            worksheet.AutoFilter.Refresh();
            
            Console.WriteLine("Row 7 hidden: " + worksheet.Cells.IsRowHidden(7));
            Console.WriteLine("Row 13 hidden: " + worksheet.Cells.IsRowHidden(13));
            
            // Modifica il filtro per mostrare i valori uguali a 500 o maggiori di 700
            worksheet.AutoFilter.Custom(3, FilterOperatorType.Equal, 500, false, FilterOperatorType.GreaterThan, 700);
            worksheet.AutoFilter.Refresh();
            
            Console.WriteLine("After refresh - Row 7 hidden: " + worksheet.Cells.IsRowHidden(7));
            Console.WriteLine("After refresh - Row 13 hidden: " + worksheet.Cells.IsRowHidden(13));
        }
    }
}
```

### Vedi anche

* class [AutoFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Refresh(bool) {#refresh_1}

Ottiene gli indici di tutte le righe nascoste.

```csharp
public int[] Refresh(bool hideRows)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| hideRows | Booleano | Se vero, nascondi le righe filtrate. |

### Valore di ritorno

Restituisce tutti gli indici delle righe nascoste.

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class AutoFilterMethodRefreshWithBooleanDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro con dati di esempio
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi dati di esempio
            worksheet.Cells["A1"].PutValue("Column1");
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["A3"].PutValue(2);
            worksheet.Cells["A4"].PutValue(1);
            worksheet.Cells["A5"].PutValue(3);
            
            // Applica filtro automatico
            worksheet.AutoFilter.Range = "A1:A5";
            worksheet.AutoFilter.AddFilter(0, "1"); // Filter to show only rows with value 1
            
            // Aggiorna il filtro e ottieni le righe nascoste
            int[] hiddenRows = worksheet.AutoFilter.Refresh(false);
            
            Console.WriteLine("Hidden rows after filter:");
            if (hiddenRows != null)
            {
                foreach (int row in hiddenRows)
                {
                    Console.WriteLine(row);
                }
            }
            
            // Mostra tutti i dati e aggiorna di nuovo
            worksheet.AutoFilter.ShowAll();
            hiddenRows = worksheet.AutoFilter.Refresh(false);
            
            Console.WriteLine("\nHidden rows after showing all:");
            if (hiddenRows == null)
            {
                Console.WriteLine("No hidden rows");
            }
        }
    }
}
```

### Vedi anche

* class [AutoFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


