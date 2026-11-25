---
title: "Workbook.Copy"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Workbook. Copia un altro oggetto Workbook"
type: docs
url: /it/net/aspose.cells/workbook/copy/
---
## Copy(Workbook, CopyOptions) {#copy_1}

Copia un altro oggetto Workbook.

```csharp
public void Copy(Workbook source, CopyOptions copyOptions)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| origine | Cartella di lavoro | Oggetto Workbook di origine. |
| copyOptions | CopyOptions | Le opzioni per copiare un altro workbook. |

### Osservazioni

È molto semplice clonare un file Excel.

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodCopyWithWorkbookCopyOptionsDemo
    {
        public static void Run()
        {
            // Workbook di origine con macro
            Workbook sourceWorkbook = new Workbook("source_with_macros.xlsm");
            
            // Workbook di destinazione (vuoto o esistente)
            Workbook destWorkbook = new Workbook();
            
            // Configura le opzioni di copia per mantenere le macro
            CopyOptions options = new CopyOptions();
            options.KeepMacros = true;
            
            // Copia i contenuti dal workbook di origine a quello di destinazione
            sourceWorkbook.Copy(destWorkbook, options);
            
            // Salva il risultato
            destWorkbook.Save("output_with_macros.xlsm");
        }
    }
}
```

### Vedi anche

* class [CopyOptions](../../copyoptions/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Copy(Workbook) {#copy}

Copia i dati da un oggetto Workbook di origine.

```csharp
public void Copy(Workbook source)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| origine | Cartella di lavoro | Oggetto Workbook di origine. |

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodCopyWithWorkbookDemo
    {
        public static void Run()
        {
            // Percorsi dei file di origine e di destinazione
            string sourceFile = "source.xlsx";
            string outputFile = "output.xlsx";

            // Carica la cartella di lavoro di origine
            Workbook sourceWorkbook = new Workbook(sourceFile);

            // Crea un nuovo workbook e copia i contenuti dalla sorgente
            Workbook destinationWorkbook = new Workbook();
            destinationWorkbook.Copy(sourceWorkbook);

            // Salva il workbook copiato
            destinationWorkbook.Save(outputFile);
            
            Console.WriteLine("Workbook copied successfully.");
        }
    }
}
```

### Vedi anche

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


