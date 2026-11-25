---
title: "AutoFilter.RemoveDateFilter"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo AutoFilter. Rimuove un filtro data"
type: docs
url: /it/net/aspose.cells/autofilter/removedatefilter/
---
## AutoFilter.RemoveDateFilter method

Rimuove un filtro data.

```csharp
public void RemoveDateFilter(int fieldIndex, DateTimeGroupingType dateTimeGroupingType, int year, 
    int month, int day, int hour, int minute, int second)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| fieldIndex | Int32 | L'offset intero del campo su cui si desidera basare il filtro (da sinistra dell'elenco; il campo più a sinistra è il campo 0). |
| dateTimeGroupingType | DateTimeGroupingType | Il tipo di raggruppamento |
| anno | Int32 | L'anno. |
| mese | Int32 | Il mese. |
| giorno | Int32 | Il giorno. |
| ora | Int32 | L'ora. |
| minuto | Int32 | Il minuto. |
| secondo | Int32 | Il secondo. |

### Osservazioni

Se DateTimeGroupingType è Year, solo il parametro year ha effetto. Se DateTiemGroupingType è Month, solo i parametri year e month hanno effetto.

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class AutoFilterMethodRemoveDateFilterWithInt32DateTimeGroupingTypeInt32Demo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro con dati di esempio
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            
            // Aggiungi dati di esempio con date
            sheet.Cells["A1"].PutValue("Date");
            sheet.Cells["B1"].PutValue("Value");
            sheet.Cells["A2"].PutValue(new DateTime(2020, 1, 7));
            sheet.Cells["A3"].PutValue(new DateTime(2020, 1, 8));
            sheet.Cells["A4"].PutValue(new DateTime(2020, 1, 9));
            
            // Applica filtro automatico
            sheet.AutoFilter.Range = "A1:A4";
            
            // Aggiungi filtro data per il giorno 7
            sheet.AutoFilter.AddDateFilter(0, DateTimeGroupingType.Day, 2020, 1, 7, 0, 0, 0);
            sheet.AutoFilter.Refresh();
            
            // Verifica che il filtro sia applicato
            Console.WriteLine("Row 2 hidden: " + sheet.Cells.IsRowHidden(1)); // Should be true
            
            // Rimuovi il filtro data
            sheet.AutoFilter.RemoveDateFilter(0, DateTimeGroupingType.Day, 2020, 1, 7, 0, 0, 0);
            sheet.AutoFilter.Refresh();
            
            // Verifica che il filtro sia rimosso
            Console.WriteLine("Row 2 hidden after removal: " + sheet.Cells.IsRowHidden(1)); // Should be false
        }
    }
}
```

### Vedi anche

* enum [DateTimeGroupingType](../../datetimegroupingtype/)
* class [AutoFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


