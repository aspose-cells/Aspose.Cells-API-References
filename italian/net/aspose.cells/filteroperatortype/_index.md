---
title: "Enum FilterOperatorType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Enum Aspose.Cells.FilterOperatorType. Tipo di operatore di filtro personalizzato"
type: docs
url: /it/net/aspose.cells/filteroperatortype/
---
## FilterOperatorType enumeration

Tipo di operatore del filtro personalizzato.

```csharp
public enum FilterOperatorType
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| LessOrEqual | `0` | Rappresenta l'operatore LessOrEqual. |
| LessThan | `1` | Rappresenta l'operatore LessThan. |
| Equal | `2` | Rappresenta l'operatore Equal. |
| GreaterThan | `3` | Rappresenta l'operatore GreaterThan. |
| NotEqual | `4` | Rappresenta l'operatore NotEqual. |
| GreaterOrEqual | `5` | Rappresenta l'operatore GreaterOrEqual. |
| None | `6` | Rappresenta nessun confronto. |
| BeginsWith | `7` | Inizia con il testo. |
| EndsWith | `8` | Termina con il testo. |
| Contains | `9` | Contiene il testo. |
| NotContains | `10` | Non contiene il testo. |
| NotBeginsWith | `11` | Non inizia con il testo. |
| NotEndsWith | `12` | Non termina con il testo. |

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassFilterOperatorTypeDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi dati di esempio
            worksheet.Cells["A1"].PutValue("Names");
            worksheet.Cells["A2"].PutValue("Bob");
            worksheet.Cells["A3"].PutValue("Alice");
            worksheet.Cells["A4"].PutValue("Bobby");
            worksheet.Cells["A5"].PutValue("Tom");
            
            // Imposta l'intervallo del filtro automatico
            worksheet.AutoFilter.Range = "A1:A5";
            
            // Applica filtro personalizzato per mostrare i nomi che iniziano con "Bo"
            worksheet.AutoFilter.Custom(0, FilterOperatorType.BeginsWith, "Bo");
            
            // Aggiorna il filtro
            worksheet.AutoFilter.Refresh();
            
            // Salva la cartella di lavoro
            workbook.Save("FilterOperatorTypeDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


