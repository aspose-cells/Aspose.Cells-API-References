---
title: "CopyOptions.ColumnCharacterWidth"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà CopyOptions. Indica se copiare la larghezza della colonna in unità di caratteri"
type: docs
url: /it/net/aspose.cells/copyoptions/columncharacterwidth/
---
## CopyOptions.ColumnCharacterWidth property

Indica se copiare la larghezza delle colonne in unità di caratteri.

```csharp
public bool ColumnCharacterWidth { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CopyOptionsPropertyColumnCharacterWidthDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro di origine con dati di esempio
            Workbook srcWorkbook = new Workbook();
            Worksheet srcSheet = srcWorkbook.Worksheets[0];
            
            // Imposta la larghezza della colonna in caratteri per la dimostrazione
            srcSheet.Cells.SetColumnWidth(0, 20); // 20 characters wide
            
            // Aggiungi alcuni dati di esempio
            srcSheet.Cells["A1"].PutValue("Sample Text");
            srcSheet.Cells["A2"].PutValue("Another Sample");
            
            // Crea la cartella di lavoro di destinazione
            Workbook destWorkbook = new Workbook();
            Worksheet destSheet = destWorkbook.Worksheets[0];
            
            // Copia con ColumnCharacterWidth impostato su true
            destSheet.Copy(srcSheet, new CopyOptions()
            {
                ColumnCharacterWidth = true
            });
            
            // Salva il risultato
            destWorkbook.Save("output_with_column_width.xlsx", SaveFormat.Xlsx);
            
            // Per confronto, copia senza ColumnCharacterWidth
            Workbook destWorkbook2 = new Workbook();
            Worksheet destSheet2 = destWorkbook2.Worksheets[0];
            
            destSheet2.Copy(srcSheet, new CopyOptions()
            {
                ColumnCharacterWidth = false
            });
            
            destWorkbook2.Save("output_without_column_width.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Vedi anche

* class [CopyOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


