---
title: "Workbook.AbsolutePath"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Workbook. Ottiene e imposta il percorso assoluto del file"
type: docs
url: /it/net/aspose.cells/workbook/absolutepath/
---
## Workbook.AbsolutePath property

Ottiene e imposta il percorso assoluto del file.

```csharp
public string AbsolutePath { get; set; }
```

### Osservazioni

Utilizzato solo per collegamenti esterni.

### Esempi

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookPropertyAbsolutePathDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook sourceBook = new Workbook();
            
            // Aggiungi alcuni fogli di lavoro
            sourceBook.Worksheets.Add("Sheet1");
            sourceBook.Worksheets.Add("Sheet2");

            // Salva la cartella di lavoro per ottenere un percorso fisico
            string sourcePath = Path.GetFullPath("output");
            if (!Directory.Exists(sourcePath))
            {
                Directory.CreateDirectory(sourcePath);
            }
            string sourceFilePath = Path.Combine(sourcePath, "example.xlsx");
            sourceBook.Save(sourceFilePath);

            // Riapri la cartella di lavoro per dimostrare AbsolutePath
            Workbook reopenedBook = new Workbook(sourceFilePath);
            
            // Usa la proprietà AbsolutePath per costruire il percorso completo
            string pathToBook = Path.Combine(reopenedBook.AbsolutePath, reopenedBook.FileName);
            Console.WriteLine("Full path to workbook: " + pathToBook);

            // Aggiungi collegamenti ipertestuali usando il percorso
            SetHyperlink(reopenedBook.Worksheets[0], 0, pathToBook, reopenedBook.Worksheets[0].Name, "A1");
            SetHyperlink(reopenedBook.Worksheets[0], 1, pathToBook, reopenedBook.Worksheets[1].Name, "B1");

            // Salva la cartella di lavoro modificata
            string destPath = Path.Combine(sourcePath, "modified_example.xlsx");
            reopenedBook.Save(destPath);
        }

        private static void SetHyperlink(Worksheet sheet, int linkIndex, string path, string sheetName, string cellRef)
        {
            HyperlinkCollection hyperlinks = sheet.Hyperlinks;
            hyperlinks.Add(cellRef, 1, 1, path + "#" + sheetName + "!A1");
        }
    }
}
```

### Vedi anche

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


