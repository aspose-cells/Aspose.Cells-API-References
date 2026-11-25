---
title: "OleObject.IsLink"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà OleObject. Restituisce true se l'OleObject è collegato al file"
type: docs
url: /it/net/aspose.cells.drawing/oleobject/islink/
---
## OleObject.IsLink property

Restituisce true se l'OleObject è collegato al file.

```csharp
public bool IsLink { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class OleObjectPropertyIsLinkDemo
    {
        public static void Run()
        {
            // Carica la cartella di lavoro di origine
            Workbook workbook = new Workbook("example.xlsm");

            // Elabora ogni foglio di lavoro
            foreach (Worksheet worksheet in workbook.Worksheets)
            {
                // Elabora ogni oggetto OLE nel foglio di lavoro
                foreach (Aspose.Cells.Drawing.OleObject ole in worksheet.OleObjects)
                {
                    // Salta se l'oggetto OLE non è collegato
                    if (!ole.IsLink)
                    {
                        Console.WriteLine("Skipping embedded OLE object");
                        continue;
                    }

                    // Visualizza e modifica il percorso del file collegato
                    Console.WriteLine("Original linked file: " + ole.ObjectSourceFullName);
                    string newPath = ole.ObjectSourceFullName.Replace("C:", "D:");
                    ole.ObjectSourceFullName = newPath;
                    Console.WriteLine("Modified linked file: " + ole.ObjectSourceFullName);
                }
            }

            // Salva la cartella di lavoro modificata
            workbook.Save("modified_example.xlsm");
            Console.WriteLine("File saved with updated OLE links.");
        }
    }
}
```

### Vedi anche

* class [OleObject](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


