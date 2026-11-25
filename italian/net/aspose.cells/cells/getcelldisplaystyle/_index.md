---
title: "Cells.GetCellDisplayStyle"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Cells. Ottieni lo stile di visualizzazione della cella specificata"
type: docs
url: /it/net/aspose.cells/cells/getcelldisplaystyle/
---
## GetCellDisplayStyle(int, int) {#getcelldisplaystyle}

Ottieni lo stile di visualizzazione della cella fornita.

```csharp
public Style GetCellDisplayStyle(int row, int column)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| riga | Int32 | indice di riga della cella specificata |
| colonna | Int32 | colonna della cella specificata |

### Valore di ritorno

lo stile di visualizzazione della cella specificata.

### Osservazioni

Stesso con [`GetDisplayStyle`](../../cell/getdisplaystyle/), e stesso con l'uso di SideBorders per `GetCellDisplayStyle`.

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsMethodGetCellDisplayStyleWithInt32Int32Demo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Prepara lo stile della cella per la dimostrazione
            Cell cell = cells[0, 0];
            cell.PutValue("Style Demo");
            
            // Crea uno stile personalizzato
            Style style = workbook.CreateStyle();
            style.Font.IsBold = true;
            style.ForegroundColor = System.Drawing.Color.Yellow;
            style.Pattern = BackgroundType.Solid;
            
            // Applica lo stile alla cella
            cell.SetStyle(style);

            try
            {
                // Chiama GetCellDisplayStyle con riga 0 e colonna 0
                Style displayStyle = cells.GetCellDisplayStyle(0, 0);

                // Proprietà dello stile di visualizzazione
                Console.WriteLine($"Bold: {displayStyle.Font.IsBold}");
                Console.WriteLine($"Background Color: {displayStyle.ForegroundColor}");

                // Applica lo stile di visualizzazione a un'altra cella per una verifica visiva
                cells[2, 2].SetStyle(displayStyle);
                cells[2, 2].PutValue("Style Copied");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetCellDisplayStyle method: {ex.Message}");
            }

            // Salva la cartella di lavoro
            workbook.Save("CellsMethodGetCellDisplayStyleWithInt32Int32Demo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Style](../../style/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetCellDisplayStyle(int, int, BorderType) {#getcelldisplaystyle_1}

Ottieni lo stile di visualizzazione della cella fornita.

```csharp
public Style GetCellDisplayStyle(int row, int column, BorderType adjacentBorders)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| riga | Int32 | indice di riga della cella specificata |
| colonna | Int32 | colonna della cella specificata |
| adjacentBorders | BorderType | Indica quali bordi devono essere controllati e regolati in base ai bordi delle celle adiacenti. Si prega di consultare la descrizione per lo stesso parametro di [`GetDisplayStyle`](../../cell/getdisplaystyle/). |

### Valore di ritorno

lo stile di visualizzazione della cella specificata.

### Osservazioni

Se la cella è anche influenzata da altre impostazioni come la formattazione condizionale, gli oggetti elenco, ecc., lo stile di visualizzazione potrebbe differire da [`GetCellStyle`](../getcellstyle/). E poiché tali impostazioni possono essere applicate anche a celle vuote (non esistenti), l'uso di questo metodo può evitare l'istanziazione di quelle celle vuote, quindi le prestazioni saranno migliori rispetto a ottenere l'istanza Cell da Cells e poi chiamare [`GetDisplayStyle`](../../cell/getdisplaystyle/).

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsMethodGetCellDisplayStyleWithInt32Int32BorderTypeDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Accedi alla cella A1 e imposta uno stile di bordo
            Cell cell = worksheet.Cells["A1"];
            Style style = cell.GetStyle();
            style.Borders[BorderType.TopBorder].LineStyle = CellBorderType.Thick;
            style.Borders[BorderType.TopBorder].Color = System.Drawing.Color.Red;
            cell.SetStyle(style);

            try
            {
                // Chiama GetCellDisplayStyle con parametri specifici (0,0 per A1, tipo TopBorder)
                Style displayStyle = worksheet.Cells.GetCellDisplayStyle(0, 0, BorderType.TopBorder);

                // Verifica se lo stile recuperato corrisponde al nostro colore del bordo
                if (displayStyle.Borders[BorderType.TopBorder].Color == System.Drawing.Color.Red)
                {
                    Console.WriteLine("Top border display style retrieved successfully - Color: Red");
                }

                // Dimostra l'applicazione dello stile modificando un'altra cella
                Cell targetCell = worksheet.Cells["B1"];
                targetCell.SetStyle(displayStyle);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetCellDisplayStyle method: {ex.Message}");
            }

            // Salva il risultato
            workbook.Save("GetCellDisplayStyleWithBorderTypeDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Style](../../style/)
* enum [BorderType](../../bordertype/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


