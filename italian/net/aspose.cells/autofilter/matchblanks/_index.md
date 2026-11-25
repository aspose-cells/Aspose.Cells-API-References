---
title: "AutoFilter.MatchBlanks"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo AutoFilter. Seleziona tutte le celle vuote nell'elenco"
type: docs
url: /it/net/aspose.cells/autofilter/matchblanks/
---
## AutoFilter.MatchBlanks method

Corrisponde a tutte le celle vuote nell'elenco.

```csharp
public void MatchBlanks(int fieldIndex)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| fieldIndex | Int32 | L'offset intero del campo su cui si desidera basare il filtro (da sinistra dell'elenco; il campo più a sinistra è il campo 0). |

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class AutoFilterMethodMatchBlanksWithInt32Demo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro con dati di esempio
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi dati di esempio con alcune celle vuote
            worksheet.Cells["A1"].PutValue("Column1");
            worksheet.Cells["B1"].PutValue("Column2");
            worksheet.Cells["C1"].PutValue("Column3");
            
            worksheet.Cells["A2"].PutValue("Data1");
            worksheet.Cells["B2"].PutValue("Data2");
            // Lascia C2 vuoto
            
            worksheet.Cells["A3"].PutValue("Data3");
            // Lascia B3 vuoto
            worksheet.Cells["C3"].PutValue("Data6");
            
            // Applica filtro automatico
            worksheet.AutoFilter.Range = "A1:C3";
            AutoFilter filter = worksheet.AutoFilter;
            
            // Filtra per mostrare solo le righe con celle vuote nella colonna 3 (C)
            filter.MatchBlanks(2); // Column index is 0-based
            
            // Aggiorna il filtro
            filter.Refresh();
            
            // Salva la cartella di lavoro
            workbook.Save("AutoFilterMatchBlanksDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [AutoFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


