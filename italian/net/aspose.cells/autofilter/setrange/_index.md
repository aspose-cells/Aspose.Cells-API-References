---
title: "AutoFilter.SetRange"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo AutoFilter. Imposta l'intervallo a cui si applica l'AutoFilter specificato"
type: docs
url: /it/net/aspose.cells/autofilter/setrange/
---
## AutoFilter.SetRange method

Imposta l'intervallo a cui si applica l'AutoFiltro specificato.

```csharp
public void SetRange(int row, int startColumn, int endColumn)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| riga | Int32 | Indice della riga. |
| startColumn | Int32 | Indice della colonna iniziale. |
| endColumn | Int32 | Indice della colonna finale. |

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class AutoFilterMethodSetRangeWithInt32Int32Int32Demo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio
            sheet.Cells["A1"].PutValue("Header");
            sheet.Cells["A2"].PutValue("Data1");
            sheet.Cells["A3"].PutValue("Data2");
            sheet.Cells["A4"].PutValue("Data3");

            // Imposta l'intervallo del filtro automatico (firstRow, firstColumn, totalRows)
            sheet.AutoFilter.SetRange(0, 0, 4);

            // Applica filtro
            sheet.AutoFilter.Custom(0, FilterOperatorType.Equal, "Data2");

            // Aggiorna filtro
            sheet.AutoFilter.Refresh();

            // Salva la cartella di lavoro
            workbook.Save("output.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Vedi anche

* class [AutoFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


