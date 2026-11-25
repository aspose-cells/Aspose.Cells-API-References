---
title: "AutoFilter.AddFilter"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo AutoFilter. Aggiunge un filtro per una colonna filtro"
type: docs
url: /it/net/aspose.cells/autofilter/addfilter/
---
## AutoFilter.AddFilter method

Aggiunge un filtro per una colonna filtro.

```csharp
public void AddFilter(int fieldIndex, string criteria)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| fieldIndex | Int32 | L'offset intero del campo su cui si desidera basare il filtro (da sinistra dell'elenco; il campo più a sinistra è il campo 0). |
| criteri | String | Il criterio specificato (una stringa; per esempio, "101"). Può essere solo null o uno dei valori delle celle in questa colonna. |

### Osservazioni

MS Excel 2007 supporta la selezione multipla in una colonna filtro.

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class AutoFilterMethodAddFilterWithInt32StringDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi dati di esempio
            worksheet.Cells["A1"].PutValue("Fruits");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Banana");
            worksheet.Cells["A4"].PutValue("Cherry");
            worksheet.Cells["A5"].PutValue("Date");
            worksheet.Cells["A6"].PutValue("Elderberry");
            
            // Crea intervallo di filtro automatico
            worksheet.AutoFilter.Range = "A1:A6";
            
            // Ottieni il filtro automatico
            AutoFilter filter = worksheet.AutoFilter;
            
            // Aggiungi filtri per i valori che iniziano con 'A' e 'E'
            filter.AddFilter(0, "A*");
            filter.AddFilter(0, "E*");
            
            // Aggiorna il filtro
            filter.Refresh();
            
            // Salva la cartella di lavoro
            workbook.Save("AutoFilterAddFilterDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [AutoFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


