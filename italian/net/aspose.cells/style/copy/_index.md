---
title: "Style.Copy"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Style. Copia i dati da un altro oggetto style"
type: docs
url: /it/net/aspose.cells/style/copy/
---
## Style.Copy method

Copia i dati da un altro oggetto stile

```csharp
public void Copy(Style style)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| stile | Stile | Oggetto Style di origine |

### Osservazioni

Questo metodo non copia il nome dello style. Se vuoi copiare il nome, per favore chiama il seguente codice dopo aver copiato lo style: destStyle.Name = style.Name.

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StyleMethodCopyWithStyleDemo
    {
        public static void Run()
        {
            // Crea la cartella di lavoro di origine con dati di esempio
            Workbook srcWorkbook = new Workbook();
            Worksheet srcSheet = srcWorkbook.Worksheets[0];
            srcSheet.Cells["A1"].PutValue("Sample Text");
            Style srcStyle = srcWorkbook.CreateStyle();
            srcStyle.Font.Name = "Arial";
            srcStyle.Font.Size = 14;
            srcSheet.Cells["A1"].SetStyle(srcStyle);

            // Crea la cartella di lavoro di destinazione
            Workbook destWorkbook = new Workbook();
            Worksheet destSheet = destWorkbook.Worksheets[0];
            
            // Copia lo style dalla sorgente alla destinazione
            Style destStyle = destWorkbook.CreateStyle();
            destStyle.Copy(srcStyle);
            
            // Applica lo style copiato
            destSheet.Cells["B2"].PutValue("Copied Style Text");
            destSheet.Cells["B2"].SetStyle(destStyle);

            // Salva il risultato
            destWorkbook.Save("output.xlsx");
        }
    }
}
```

### Vedi anche

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


