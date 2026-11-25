---
title: "Cell.Characters"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Cell. Restituisce un oggetto Characters che rappresenta un intervallo di caratteri all'interno del testo della cella"
type: docs
url: /it/net/aspose.cells/cell/characters/
---
## Cell.Characters method

Restituisce un oggetto Characters che rappresenta un intervallo di caratteri nel testo della cella.

```csharp
public FontSetting Characters(int startIndex, int length)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| startIndex | Int32 | L'indice dell'inizio del carattere. |
| lunghezza | Int32 | Il numero di caratteri. |

### Valore di ritorno

Oggetto Characters.

### Osservazioni

Questo metodo funziona solo su celle con valore stringa.

### Esempi

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class CellMethodCharactersWithInt32Int32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            
            cells["A1"].PutValue("Helloworld");
            cells["A1"].Characters(5, 5).Font.IsBold = true;
            cells["A1"].Characters(5, 5).Font.Color = Color.Blue;
            
            workbook.Save("output.xlsx");
        }
    }
}
```

### Vedi anche

* class [FontSetting](../../fontsetting/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


