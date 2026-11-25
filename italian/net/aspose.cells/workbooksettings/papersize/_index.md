---
title: "WorkbookSettings.PaperSize"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "WorkbookSettings property. Ottiene e imposta la dimensione carta di stampa predefinita"
type: docs
url: /it/net/aspose.cells/workbooksettings/papersize/
---
## WorkbookSettings.PaperSize property

Ottiene e imposta la dimensione predefinita della carta di stampa.

```csharp
public PaperSizeType PaperSize { get; set; }
```

### Osservazioni

Se non esiste un'impostazione relativa alla dimensione della carta, MS Excel utilizzerà l'impostazione predefinita della stampante.

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyPaperSizeDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Imposta la dimensione della carta su A5
            workbook.Settings.PaperSize = PaperSizeType.PaperA5;
            
            // Verifica che la dimensione della carta sia impostata correttamente nel primo foglio di lavoro
            Console.WriteLine("Paper size: " + workbook.Worksheets[0].PageSetup.PaperSize);
            
            // Salva la cartella di lavoro
            workbook.Save("output.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Vedi anche

* enum [PaperSizeType](../../papersizetype/)
* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


