---
title: "Cell.GetStyle"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Cell. Ottiene lo stile della cella"
type: docs
url: /it/net/aspose.cells/cell/getstyle/
---
## GetStyle() {#getstyle}

Ottiene lo stile della cella.

```csharp
public Style GetStyle()
```

### Valore di ritorno

Oggetto Style.

### Osservazioni

Per modificare lo stile della cella, si prega di chiamare il metodo Cell.SetStyle() dopo aver modificato l'oggetto style restituito. Questo metodo è lo stesso di `GetStyle` con valore true per il parametro.

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodGetStyleDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Imposta diversi allineamenti verticali per le celle
            cells["A1"].PutValue("Bottom Alignment");
            cells["A1"].GetStyle().VerticalAlignment = TextAlignmentType.Bottom;

            cells["A2"].PutValue("Center Alignment");
            cells["A2"].GetStyle().VerticalAlignment = TextAlignmentType.Center;

            cells["A3"].PutValue("Distributed Alignment");
            cells["A3"].GetStyle().VerticalAlignment = TextAlignmentType.Distributed;

            cells["A4"].PutValue("Justify Alignment");
            cells["A4"].GetStyle().VerticalAlignment = TextAlignmentType.Justify;

            cells["A5"].PutValue("Top Alignment");
            cells["A5"].GetStyle().VerticalAlignment = TextAlignmentType.Top;

            // Dimostra il metodo GetStyle()
            Console.WriteLine("A1 Vertical Alignment: " + cells["A1"].GetStyle().VerticalAlignment);
            Console.WriteLine("A2 Vertical Alignment: " + cells["A2"].GetStyle().VerticalAlignment);
            Console.WriteLine("A3 Vertical Alignment: " + cells["A3"].GetStyle().VerticalAlignment);
            Console.WriteLine("A4 Vertical Alignment: " + cells["A4"].GetStyle().VerticalAlignment);
            Console.WriteLine("A5 Vertical Alignment: " + cells["A5"].GetStyle().VerticalAlignment);
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

## GetStyle(bool) {#getstyle_1}

Se checkBorders è true, verifica se i bordi delle altre celle influenzeranno lo stile di questa cella.

```csharp
public Style GetStyle(bool checkBorders)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| checkBorders | Booleano | Controlla i bordi delle altre celle |

### Valore di ritorno

Oggetto Style.

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodGetStyleWithBooleanDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Accedi a una cella e imposta alcuni dati di esempio
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue(123.456);

            // Ottieni lo stile della cella senza ereditare da riga/colonna (parametro false)
            Style style = cell.GetStyle(false);
            
            // Modifica lo stile
            style.Custom = "0.000";
            style.Borders[BorderType.TopBorder].LineStyle = CellBorderType.None;

            // Applica lo stile modificato alla cella
            cell.SetStyle(style);

            // Verifica le modifiche allo stile
            Console.WriteLine("Number Format: " + cell.GetStyle(false).Custom);
            Console.WriteLine("Top Border Style: " + cell.GetStyle(false).Borders[BorderType.TopBorder].LineStyle);

            // Salva la cartella di lavoro
            workbook.Save("output.xlsx");
        }
    }
}
```

### Vedi anche

* class [Style](../../style/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


