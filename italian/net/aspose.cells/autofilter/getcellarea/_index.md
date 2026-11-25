---
title: "AutoFilter.GetCellArea"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo AutoFilter. Ottiene il CellArea a cui si applica questo AutoFilter"
type: docs
url: /it/net/aspose.cells/autofilter/getcellarea/
---
## GetCellArea() {#getcellarea}

Ottiene il [`CellArea`](../../cellarea/) a cui si applica questo AutoFilter.

```csharp
public CellArea GetCellArea()
```

### Valore di ritorno

l'area a cui si applica questo filtro

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class AutoFilterMethodGetCellAreaDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Popola dati di esempio per la dimostrazione dell'AutoFilter
            cells["A1"].PutValue("Product");
            cells["B1"].PutValue("Category");
            cells["C1"].PutValue("Price");

            cells["A2"].PutValue("Apple");
            cells["B2"].PutValue("Fruit");
            cells["C2"].PutValue(2.5);

            cells["A3"].PutValue("Carrot");
            cells["B3"].PutValue("Vegetable");
            cells["C3"].PutValue(1.2);

            cells["A4"].PutValue("Banana");
            cells["B4"].PutValue("Fruit");
            cells["C4"].PutValue(3.1);

            // Applica AutoFilter alle intestazioni (indice riga 0) coprendo le colonne A-C (0-2)
            AutoFilter autoFilter = worksheet.AutoFilter;
            autoFilter.SetRange(0, 0, 2);

            try
            {
                // Ottieni il CellArea dove è applicato AutoFilter
                CellArea result = autoFilter.GetCellArea();

                // Restituisci le coordinate dell'intervallo AutoFilter
                Console.WriteLine("AutoFilter applied to cell area:");
                Console.WriteLine($"Start Row: {result.StartRow}");
                Console.WriteLine($"Start Column: {result.StartColumn}");
                Console.WriteLine($"End Row: {result.EndRow}");
                Console.WriteLine($"End Column: {result.EndColumn}");

                // Applica un filtro semplice per dimostrare la funzionalità (opzionale)
                autoFilter.Filter(1, "Fruit"); // Filter "Category" column (index 1) for "Fruit"
                autoFilter.Refresh();
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetCellArea method: {ex.Message}");
            }

            // Salva la cartella di lavoro con AutoFilter applicato
            workbook.Save("AutoFilterMethodGetCellAreaDemo.xlsx");
        }
    }
}
```

### Vedi anche

* struct [CellArea](../../cellarea/)
* class [AutoFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetCellArea(bool) {#getcellarea_1}

Ottiene il [`CellArea`](../../cellarea/) a cui si applica l'AutoFilter specificato.

```csharp
public CellArea GetCellArea(bool refreshAppliedRange)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| refreshAppliedRange | Booleano | Indica se aggiornare l'intervallo applicato. Per l'intervallo applicato dell'auto filter, l'ultima riga può cambiare quando i dati delle celle cambiano. Se questo flag è true, l'ultima riga dell'intervallo verrà ricalcolata in base ai dati attuali delle celle. |

### Valore di ritorno

l'area a cui si applica questo filtro

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class AutoFilterMethodGetCellAreaWithBooleanDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Prepara dati di esempio per AutoFilter
            worksheet.Cells["A1"].PutValue("Header");
            worksheet.Cells["A2"].PutValue("Data1");
            worksheet.Cells["A3"].PutValue("Data2");
            worksheet.Cells["A4"].PutValue("Data3");

            // Imposta l'intervallo AutoFilter (riga 0 a 3, colonna 0)
            worksheet.AutoFilter.SetRange(0, 0, 0);

            try
            {
                // Chiama GetCellArea con refreshAppliedRange=true
                CellArea result = worksheet.AutoFilter.GetCellArea(true);

                // Visualizza l'intervallo applicato di AutoFilter
                Console.WriteLine($"AutoFilter Range: StartRow={result.StartRow}, " +
                    $"StartColumn={result.StartColumn}, EndRow={result.EndRow}, " +
                    $"EndColumn={result.EndColumn}");

                Console.WriteLine("GetCellArea method executed successfully with boolean parameter");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetCellArea: {ex.Message}");
            }

            // Salva la cartella di lavoro modificata
            workbook.Save("AutoFilterMethodGetCellAreaWithBooleanDemo.xlsx");
        }
    }
}
```

### Vedi anche

* struct [CellArea](../../cellarea/)
* class [AutoFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


