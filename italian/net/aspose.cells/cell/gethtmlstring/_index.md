---
title: "Cell.GetHtmlString"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Cell. Ottiene la stringa HTML che contiene dati e alcuni formati in questa cella"
type: docs
url: /it/net/aspose.cells/cell/gethtmlstring/
---
## Cell.GetHtmlString method

Ottiene la stringa HTML che contiene dati e alcuni formati in questa cella.

```csharp
public string GetHtmlString(bool html5)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| html5 | Booleano | Indica se il valore è compatibile con html5 |

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodGetHtmlStringWithBooleanDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Imposta un valore di cella di esempio con formattazione
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Sample Text");
            Style style = cell.GetStyle();
            style.Font.Name = "Calibri";
            style.Font.Size = 11;
            style.Font.Color = System.Drawing.Color.Red;
            cell.SetStyle(style);

            // Dimostra GetHtmlString con parametro booleano
            string htmlWithoutDiv = cell.GetHtmlString(false);
            string htmlWithDiv = cell.GetHtmlString(true);
            
            Console.WriteLine("HTML without div wrapper:");
            Console.WriteLine(htmlWithoutDiv);
            Console.WriteLine("\nHTML with div wrapper:");
            Console.WriteLine(htmlWithDiv);
        }
    }
}
```

### Vedi anche

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


