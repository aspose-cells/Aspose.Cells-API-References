---
title: "AutoFilter.FilterTop10"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo AutoFilter. Filtra i primi 10 elementi nella lista"
type: docs
url: /it/net/aspose.cells/autofilter/filtertop10/
---
## AutoFilter.FilterTop10 method

Filtra i primi 10 elementi dell'elenco

```csharp
public void FilterTop10(int fieldIndex, bool isTop, bool isPercent, int itemCount)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| fieldIndex | Int32 | L'offset intero del campo su cui si desidera basare il filtro (da sinistra dell'elenco; il campo più a sinistra è il campo 0). |
| isTop | Booleano | Indica se il filtro è dall'alto o dal basso |
| isPercent | Booleano | Indica se gli elementi sono percentuale o conteggio |
| itemCount | Int32 | Il conteggio degli elementi |

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class AutoFilterMethodFilterTop10WithInt32BooleanBooleanInt32Demo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro con dati di esempio
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi dati di esempio (5 righe x 3 colonne con valori numerici)
            Cells cells = worksheet.Cells;
            cells["A1"].PutValue("Numbers");
            cells["A2"].PutValue(50);
            cells["A3"].PutValue(30);
            cells["A4"].PutValue(80);
            cells["A5"].PutValue(20);
            cells["A6"].PutValue(90);

            // Imposta intervallo autofilter
            worksheet.AutoFilter.Range = "A1:A6";

            // Applica filtro top 10 (mostrando i primi 2 elementi)
            worksheet.AutoFilter.FilterTop10(0, true, false, 2);

            // Aggiorna il filtro
            worksheet.AutoFilter.Refresh();

            // Salva la cartella di lavoro
            workbook.Save("FilterTop10Demo.xlsx");
        }
    }
}
```

### Vedi anche

* class [AutoFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


