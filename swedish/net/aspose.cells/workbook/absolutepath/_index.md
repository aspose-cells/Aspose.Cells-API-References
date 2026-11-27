---
title: "Workbook.AbsolutePath"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Workbook-egenskap. Hämtar och anger den absoluta sökvägen för filen"
type: docs
url: /sv/net/aspose.cells/workbook/absolutepath/
---
## Workbook.AbsolutePath property

Hämtar och anger den absoluta sökvägen för filen.

```csharp
public string AbsolutePath { get; set; }
```

### Anmärkningar

Endast används för externa länkar.

### Exempel

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
            // Skapa en ny arbetsbok
            Workbook sourceBook = new Workbook();
            
            // Lägg till några arbetsblad
            sourceBook.Worksheets.Add("Sheet1");
            sourceBook.Worksheets.Add("Sheet2");

            // Spara arbetsboken för att få en fysisk sökväg
            string sourcePath = Path.GetFullPath("output");
            if (!Directory.Exists(sourcePath))
            {
                Directory.CreateDirectory(sourcePath);
            }
            string sourceFilePath = Path.Combine(sourcePath, "example.xlsx");
            sourceBook.Save(sourceFilePath);

            // Öppna arbetsboken igen för att demonstrera AbsolutePath
            Workbook reopenedBook = new Workbook(sourceFilePath);
            
            // Använd egenskapen AbsolutePath för att konstruera fullständig sökväg
            string pathToBook = Path.Combine(reopenedBook.AbsolutePath, reopenedBook.FileName);
            Console.WriteLine("Full path to workbook: " + pathToBook);

            // Lägg till hyperlänkar med hjälp av sökvägen
            SetHyperlink(reopenedBook.Worksheets[0], 0, pathToBook, reopenedBook.Worksheets[0].Name, "A1");
            SetHyperlink(reopenedBook.Worksheets[0], 1, pathToBook, reopenedBook.Worksheets[1].Name, "B1");

            // Spara den modifierade arbetsboken
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

### Se även

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


