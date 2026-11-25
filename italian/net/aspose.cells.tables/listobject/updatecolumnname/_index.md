---
title: "ListObject.UpdateColumnName"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo ListObject. Aggiorna tutti i nomi delle colonne della lista nelle celle della tabella"
type: docs
url: /it/net/aspose.cells.tables/listobject/updatecolumnname/
---
## ListObject.UpdateColumnName method

Aggiorna i nomi di tutte le colonne dell'elenco nelle celle della tabella.

```csharp
public void UpdateColumnName()
```

### Osservazioni

Il valore delle celle nella riga di intestazione della tabella deve essere uguale al nome della ListColumn; Cell.PutValue non modifica automaticamente il nome della ListColumn per motivi di prestazioni.

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ListObjectMethodUpdateColumnNameDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro
            Workbook wb = new Workbook();
            Worksheet ws = wb.Worksheets[0];

            // Crea un oggetto tabella/elenco
            var listObject = ws.ListObjects[ws.ListObjects.Add(3, 3, 6, 6, true)];
            
            // Popola alcuni dati nella tabella
            for (int r = 0; r < 3; r++)
            {
                for (int c = 0; c < 3; c++)
                {
                    if (c > 0)
                        ws.Cells[listObject.StartRow + r, listObject.StartColumn + c].PutValue(r + c);
                    else
                        ws.Cells[listObject.StartRow + r, listObject.StartColumn + c].PutValue("");
                }
            }

            // Aggiorna i nomi delle colonne (imposterà nomi predefiniti come Column1, Column2 ecc.)
            listObject.UpdateColumnName();

            // Salva la cartella di lavoro
            wb.Save("output.xlsx");

            // Verifica che il nome della colonna sia stato aggiornato
            Console.WriteLine("First column name: " + ws.Cells[listObject.StartRow, listObject.StartColumn].StringValue);
        }
    }
}
```

### Vedi anche

* class [ListObject](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


