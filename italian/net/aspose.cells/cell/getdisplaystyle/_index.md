---
title: "Cell.GetDisplayStyle"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Cell. Restituisce lo stile di visualizzazione di questa cella"
type: docs
url: /it/net/aspose.cells/cell/getdisplaystyle/
---
## GetDisplayStyle() {#getdisplaystyle}

Ottiene lo stile di visualizzazione di questa cella.

```csharp
public Style GetDisplayStyle()
```

### Valore di ritorno

stile di visualizzazione di questa cella

### Osservazioni

Stesso comportamento usando SideBorders per `GetDisplayStyle`. Cioè, questo metodo controllerà e regolerà i bordi superiore/inferiore/sinistro/destro di questa cella in base allo stile ([`GetStyle`](../getstyle/)) delle celle adiacenti, ma non controllerà le celle unite e non controllerà lo stile di visualizzazione delle celle adiacenti.

### Esempi

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class CellMethodGetDisplayStyleDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Imposta lo stile per la cella A1
            Style style1 = workbook.CreateStyle();
            style1.ForegroundColor = Color.FromArgb(157, 195, 230);
            worksheet.Cells["A1"].SetStyle(style1);
            
            // Imposta lo stile per la cella A23
            Style style2 = workbook.CreateStyle();
            style2.ForegroundColor = Color.Red;
            worksheet.Cells["A23"].SetStyle(style2);
            
            // Ottieni e visualizza gli stili
            Style displayStyle1 = worksheet.Cells["A1"].GetDisplayStyle();
            Console.WriteLine("A1 Foreground Color: " + displayStyle1.ForegroundColor);
            
            Style displayStyle2 = worksheet.Cells["A23"].GetDisplayStyle();
            Console.WriteLine("A23 Foreground Color: " + displayStyle2.ForegroundColor);
        }
    }
}
```

### Vedi anche

* class [Style](../../style/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetDisplayStyle(bool) {#getdisplaystyle_2}

Ottiene lo stile di visualizzazione di questa cella.

```csharp
public Style GetDisplayStyle(bool includeMergedBorders)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| includeMergedBorders | Booleano | Indica se controllare i bordi delle celle unite. |

### Valore di ritorno

stile di visualizzazione di questa cella

### Osservazioni

Se il flag specificato è false, allora è lo stesso di `GetDisplayStyle`. Altrimenti è lo stesso di usare SideBorders&#x7C;DynamicStyleBorders per `GetDisplayStyle`.

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodGetDisplayStyleWithBooleanDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Accedi alla cella B2 e imposta alcune proprietà di stile
            Cell cell = worksheet.Cells["B2"];
            Style cellStyle = cell.GetStyle();
            cellStyle.Borders[BorderType.RightBorder].LineStyle = CellBorderType.Thin;
            cell.SetStyle(cellStyle);
            
            // Ottieni lo stile di visualizzazione con formattazione (parametro true)
            Style displayStyle = cell.GetDisplayStyle(true);
            
            // Restituisci lo stile della linea del bordo destro
            Console.WriteLine("Right Border Line Style: " + displayStyle.Borders[BorderType.RightBorder].LineStyle);
        }
    }
}
```

### Vedi anche

* class [Style](../../style/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetDisplayStyle(BorderType) {#getdisplaystyle_1}

Ottiene lo stile di visualizzazione di questa cella.

```csharp
public Style GetDisplayStyle(BorderType adjacentBorders)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| adjacentBorders | BorderType | Indica quali bordi devono essere controllati e regolati in base ai bordi delle celle adiacenti. |

### Valore di ritorno

stile di visualizzazione di questa cella

### Osservazioni

Se questa cella è anche influenzata da altre impostazioni come formattazione condizionale, oggetti elenco, ecc., lo stile di visualizzazione potrebbe differire da [`GetStyle`](../getstyle/). Per i flag di regolazione dei bordi in base alle celle adiacenti, TopBorder/BottomBorder/LeftBorder/RightBorder indicano se controllare e combinare i bordi inferiore/superiore/destro/sinistro delle celle sinistra/destra/sopra/sotto adiacenti a questa. Per motivi di prestazioni e compatibilità, alcuni enum sono usati per indicare operazioni speciali: Horizontal/Vertical indicano se controllare e combinare il bordo inferiore/destro delle celle unite con questa. Diagonal (cioè, sia DiagonalUpBorder che DiagonalDownBorder sono impostati) indica il controllo e la combinazione dei bordi dallo stile di visualizzazione delle celle adiacenti. Si noti che il controllo dei bordi/stili delle celle adiacenti, specialmente gli stili di visualizzazione, è un processo dispendioso in termini di tempo. Se non è necessario ottenere i bordi per lo stile restituito, usare None per disabilitare il processo delle celle adiacenti offrirà migliori prestazioni. Quando si ottengono i bordi delle celle adiacenti dagli stili definiti solo su quelle celle (senza impostare Diagonal), le prestazioni possono essere migliori perché anche il controllo dello stile di visualizzazione di una singola cella richiede tempo.

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodGetDisplayStyleWithBorderTypeDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            Cells cells = sheet.Cells;

            // Imposta dati di esempio
            for (int i = 0; i < 10; i++)
            {
                cells[i, 0].PutValue(i);
            }

            // Crea formattazione condizionale
            FormatConditionCollection fcs = sheet.ConditionalFormattings[sheet.ConditionalFormattings.Add()];
            fcs.AddArea(CellArea.CreateCellArea(0, 0, 9, 0));
            fcs.AddCondition(FormatConditionType.ColorScale);

            // Ottieni lo stile di visualizzazione con diversi tipi di bordo
            for (int i = 0; i < 10; i++)
            {
                Style styleWithBorder = cells[i, 0].GetDisplayStyle(BorderType.TopBorder);
                Style styleWithoutBorder = cells[i, 0].GetDisplayStyle(BorderType.None);

                Console.WriteLine($"Cell {i + 1}:");
                Console.WriteLine($"  Style with border - Foreground: {styleWithBorder.ForegroundArgbColor:X}");
                Console.WriteLine($"  Style without border - Foreground: {styleWithoutBorder.ForegroundArgbColor:X}");
            }
        }
    }
}
```

### Vedi anche

* class [Style](../../style/)
* enum [BorderType](../../bordertype/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


