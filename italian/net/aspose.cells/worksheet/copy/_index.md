---
title: "Worksheet.Copy"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Worksheet. Copia contenuti e formati da un altro foglio di lavoro"
type: docs
url: /it/net/aspose.cells/worksheet/copy/
---
## Copy(Worksheet) {#copy}

Copia contenuti e formati da un altro foglio di lavoro.

```csharp
public void Copy(Worksheet sourceSheet)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| sourceSheet | Worksheet | Foglio di lavoro di origine. |

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodCopyWithWorksheetDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro di origine con dati di esempio
            Workbook sourceWorkbook = new Workbook();
            Worksheet sourceSheet = sourceWorkbook.Worksheets[0];
            sourceSheet.Cells["A1"].PutValue("Source Worksheet");
            
            // Crea una cartella di lavoro di destinazione
            Workbook destWorkbook = new Workbook();
            Worksheet destSheet = destWorkbook.Worksheets[0];
            
            // Copia il foglio di lavoro di origine nel foglio di lavoro di destinazione
            destSheet.Copy(sourceSheet);
            
            // Salva il risultato
            destWorkbook.Save("output.xlsx");
        }
    }
}
```

### Vedi anche

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Copy(Worksheet, CopyOptions) {#copy_1}

Copia contenuti e formati da un altro foglio di lavoro.

```csharp
public void Copy(Worksheet sourceSheet, CopyOptions copyOptions)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| sourceSheet | Worksheet | Foglio di lavoro di origine. |
| copyOptions | CopyOptions |  |

### Osservazioni

È possibile copiare dati da un altro foglio di lavoro nello stesso file o in un altro file. Tuttavia, questo metodo non supporta la copia di oggetti di disegno, come commenti, immagini e grafici.

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodCopyWithWorksheetCopyOptionsDemo
    {
        public static void Run()
        {
            // Crea la cartella di lavoro di origine con dati di esempio
            Workbook srcWorkbook = new Workbook();
            Worksheet srcSheet = srcWorkbook.Worksheets[0];
            srcSheet.Name = "SourceSheet";
            srcSheet.Cells["A1"].PutValue("Source Data");

            // Crea la cartella di lavoro di destinazione
            Workbook destWorkbook = new Workbook();
            Worksheet destSheet = destWorkbook.Worksheets[0];
            destSheet.Name = "DestinationSheet";

            // Configura le opzioni di copia
            CopyOptions options = new CopyOptions();
            options.ReferToDestinationSheet = true;

            // Copia il foglio di lavoro con opzioni
            srcSheet.Copy(destSheet, options);

            // Verifica l'operazione di copia
            Console.WriteLine("Copied cell value: " + destSheet.Cells["A1"].StringValue);
            
            // Salva il risultato
            destWorkbook.Save("output.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Vedi anche

* class [CopyOptions](../../copyoptions/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


