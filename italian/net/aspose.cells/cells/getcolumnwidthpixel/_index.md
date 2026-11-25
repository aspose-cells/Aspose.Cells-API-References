---
title: "Cells.GetColumnWidthPixel"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Cells. Ottiene la larghezza della colonna specificata nella visualizzazione normale in unità di pixel"
type: docs
url: /it/net/aspose.cells/cells/getcolumnwidthpixel/
---
## GetColumnWidthPixel(int) {#getcolumnwidthpixel}

Restituisce la larghezza della colonna specificata nella visualizzazione normale, in unità di pixel.

```csharp
public int GetColumnWidthPixel(int column)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| colonna | Int32 | Indice colonna |

### Valore di ritorno

Larghezza della colonna nella visualizzazione normale.

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodGetColumnWidthPixelWithInt32Demo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Imposta la larghezza della colonna in caratteri (verrà convertita in pixel)
            worksheet.Cells.SetColumnWidth(1, 25);
            
            // Ottieni la larghezza della colonna in pixel
            int widthInPixels = worksheet.Cells.GetColumnWidthPixel(1);
            
            // Restituisci il risultato
            Console.WriteLine("Column width in pixels: " + widthInPixels);
        }
    }
}
```

### Vedi anche

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetColumnWidthPixel(int, bool) {#getcolumnwidthpixel_1}

Restituisce la larghezza della colonna specificata nella visualizzazione normale, in unità di pixel.

```csharp
[Obsolete("Use Cells.GetColumnWidth(int ,bool , CellsUnitType ) method, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int GetColumnWidthPixel(int column, bool original)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| colonna | Int32 | Indice colonna |
| originale | Booleano | Indica se restituire la larghezza originale anche quando la colonna è nascosta |

### Valore di ritorno

Larghezza della colonna nella visualizzazione normale.

### Osservazioni

NOTA: Questo metodo è ora obsoleto. Invece, si prega di utilizzare il metodo Cells.GetColumnWidth(int ,bool , CellsUnitType ). Questo metodo sarà rimosso 12 mesi dopo, a partire da aprile 2024. Aspose si scusa per eventuali disagi che potresti aver riscontrato.

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsMethodGetColumnWidthPixelWithInt32BooleanDemo
    {
        public static void Run()
        {
            // Crea una nuova cartella di lavoro e accedi al primo foglio di lavoro
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Imposta la larghezza standard della colonna a 80 pixel
            worksheet.Cells.StandardWidthPixels = 80;

            // Imposta la larghezza specifica della colonna 2 (terza colonna) a 120 pixel
            worksheet.Cells.SetColumnWidthPixel(2, 120);

            try
            {
                // Ottieni la larghezza corrente con le modifiche dell'utente (originale: false)
                int currentWidth = worksheet.Cells.GetColumnWidthPixel(2, false);
                Console.WriteLine($"Column 2 current width: {currentWidth} pixels");

                // Ottieni la larghezza originale senza modifiche (originale: true)
                int originalWidth = worksheet.Cells.GetColumnWidthPixel(2, true);
                Console.WriteLine($"Column 2 original width: {originalWidth} pixels");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetColumnWidthPixel: {ex.Message}");
            }

            // Salva la cartella di lavoro per dimostrare la persistenza della larghezza della colonna
            workbook.Save("ColumnWidthDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


