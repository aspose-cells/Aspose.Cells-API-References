---
title: "CellsHelper.GetDoubleFromDateTime"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo CellsHelper. Converte la data e ora in valore double"
type: docs
url: /it/net/aspose.cells/cellshelper/getdoublefromdatetime/
---
## CellsHelper.GetDoubleFromDateTime method

Converte la data/ora in valore double.

```csharp
public static double GetDoubleFromDateTime(DateTime dateTime, bool date1904)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| dateTime | DateTime | La data e ora. |
| date1904 | Booleano | Sistema data 1904. |

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsHelperMethodGetDoubleFromDateTimeWithDateTimeBooleanDemo
    {
        public static void Run()
        {
            // Crea un'istanza di cartella di lavoro
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ottieni data e ora correnti
            DateTime now = DateTime.Now;
            
            // Converti DateTime in double usando CellsHelper
            double dateDouble = CellsHelper.GetDoubleFromDateTime(now, false);
            
            // Imposta il valore nella cella A1
            worksheet.Cells["A1"].PutValue(dateDouble);
            
            // Formatta la cella per visualizzarla come data
            Style style = worksheet.Cells["A1"].GetStyle();
            style.Number = 14; // Date format
            worksheet.Cells["A1"].SetStyle(style);
            
            // Salva la cartella di lavoro
            workbook.Save("DateTimeConversionDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [CellsHelper](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


