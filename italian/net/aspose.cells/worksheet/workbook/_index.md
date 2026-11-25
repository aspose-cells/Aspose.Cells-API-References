---
title: "Worksheet.Workbook"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Worksheet. Ottiene l'oggetto workbook che contiene questo foglio"
type: docs
url: /it/net/aspose.cells/worksheet/workbook/
---
## Worksheet.Workbook property

Ottiene l'oggetto cartella di lavoro che contiene questo foglio.

```csharp
public Workbook Workbook { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyWorkbookDemo
    {
        public static void Run()
        {
            // Crea un workbook di origine e ottieni un foglio di lavoro
            Workbook sourceWorkbook = new Workbook();
            Worksheet sourceSheet = sourceWorkbook.Worksheets[0];
            
            // Aggiungi dati di esempio al foglio di lavoro di origine
            sourceSheet.Cells["A1"].PutValue("Sample Data");
            sourceSheet.Cells["A2"].PutValue(100);
            sourceSheet.Cells["A3"].PutValue(200);
            
            // Crea una cartella di lavoro di destinazione
            Workbook destWorkbook = new Workbook();
            
            // Copia il tema dal workbook di origine usando la proprietà Worksheet.Workbook
            destWorkbook.CopyTheme(sourceSheet.Workbook);
            
            // Accedi al foglio di lavoro di destinazione e copia i dati
            Worksheet destSheet = destWorkbook.Worksheets[0];
            Aspose.Cells.Range sourceRange = sourceSheet.Cells.CreateRange("A1:A3");
            Aspose.Cells.Range destRange = destSheet.Cells.CreateRange("A1:A3");
            
            // Copia i dati con formattazione
            destRange.Copy(sourceRange);
            
            // Salva il workbook di destinazione
            destWorkbook.Save("output.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Vedi anche

* class [Workbook](../../workbook/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


