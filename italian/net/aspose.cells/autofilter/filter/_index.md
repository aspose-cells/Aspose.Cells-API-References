---
title: "AutoFilter.Filter"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo AutoFilter. Filtra un elenco con i criteri specificati"
type: docs
url: /it/net/aspose.cells/autofilter/filter/
---
## AutoFilter.Filter method

Filtra un elenco con criteri specificati.

```csharp
public void Filter(int fieldIndex, string criteria)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| fieldIndex | Int32 | L'offset intero del campo su cui si desidera basare il filtro (da sinistra dell'elenco; il campo più a sinistra è il campo 0). |
| criteri | String | Il criterio specificato (una stringa; per esempio, "101"). |

### Osservazioni

Aspose.Cells rimuoverà tutte le altre impostazioni di filtro su questo campo come in MS Excel 97-2003.

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class AutoFilterMethodFilterWithInt32StringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio
            sheet.Cells["A1"].PutValue("Name");
            sheet.Cells["A2"].PutValue("Nom1");
            sheet.Cells["A3"].PutValue("Nom2");
            sheet.Cells["A4"].PutValue("Nom3");
            sheet.Cells["A5"].PutValue("Nom2");

            // Applica l'auto filtro usando i parametri corretti di SetRange
            sheet.AutoFilter.SetRange(0, 0, 4); // startRow: 0, startColumn: 0, endRow: 4
            sheet.AutoFilter.Filter(0, "Nom2"); // Filter column 0 (A) for "Nom2"
            sheet.AutoFilter.Refresh();

            // Salva il risultato
            workbook.Save("AutoFilterDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [AutoFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


