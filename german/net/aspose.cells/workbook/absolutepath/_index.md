---
title: "Workbook.AbsolutePath"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Workbook-Eigenschaft. Ruft den absoluten Pfad der Datei ab und legt ihn fest"
type: docs
url: /de/net/aspose.cells/workbook/absolutepath/
---
## Workbook.AbsolutePath property

Liest und setzt den absoluten Pfad der Datei.

```csharp
public string AbsolutePath { get; set; }
```

### Hinweise

Nur für externe Links verwendet.

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook sourceBook = new Workbook();
            
            // Einige Arbeitsblätter hinzufügen
            sourceBook.Worksheets.Add("Sheet1");
            sourceBook.Worksheets.Add("Sheet2");

            // Speichere das Arbeitsbuch, um einen physischen Pfad zu erhalten
            string sourcePath = Path.GetFullPath("output");
            if (!Directory.Exists(sourcePath))
            {
                Directory.CreateDirectory(sourcePath);
            }
            string sourceFilePath = Path.Combine(sourcePath, "example.xlsx");
            sourceBook.Save(sourceFilePath);

            // Öffne das Arbeitsbuch erneut, um AbsolutePath zu demonstrieren
            Workbook reopenedBook = new Workbook(sourceFilePath);
            
            // Verwende die AbsolutePath-Eigenschaft, um den vollständigen Pfad zu erstellen
            string pathToBook = Path.Combine(reopenedBook.AbsolutePath, reopenedBook.FileName);
            Console.WriteLine("Full path to workbook: " + pathToBook);

            // Hyperlinks mit dem Pfad hinzufügen
            SetHyperlink(reopenedBook.Worksheets[0], 0, pathToBook, reopenedBook.Worksheets[0].Name, "A1");
            SetHyperlink(reopenedBook.Worksheets[0], 1, pathToBook, reopenedBook.Worksheets[1].Name, "B1");

            // Speichere die geänderte Arbeitsmappe
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

### Siehe auch

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


