---
title: "OleObject.IsLink"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "OleObject-Eigenschaft. Gibt true zurück, wenn das OleObject mit der Datei verknüpft ist"
type: docs
url: /de/net/aspose.cells.drawing/oleobject/islink/
---
## OleObject.IsLink property

Gibt true zurück, wenn das OleObject mit der Datei verknüpft ist.

```csharp
public bool IsLink { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class OleObjectPropertyIsLinkDemo
    {
        public static void Run()
        {
            // Lade die Quellarbeitsmappe
            Workbook workbook = new Workbook("example.xlsm");

            // Verarbeite jedes Arbeitsblatt
            foreach (Worksheet worksheet in workbook.Worksheets)
            {
                // Verarbeite jedes OLE-Objekt im Arbeitsblatt
                foreach (Aspose.Cells.Drawing.OleObject ole in worksheet.OleObjects)
                {
                    // Überspringen, wenn das OLE-Objekt nicht verknüpft ist
                    if (!ole.IsLink)
                    {
                        Console.WriteLine("Skipping embedded OLE object");
                        continue;
                    }

                    // Zeige den verknüpften Dateipfad an und ändere ihn
                    Console.WriteLine("Original linked file: " + ole.ObjectSourceFullName);
                    string newPath = ole.ObjectSourceFullName.Replace("C:", "D:");
                    ole.ObjectSourceFullName = newPath;
                    Console.WriteLine("Modified linked file: " + ole.ObjectSourceFullName);
                }
            }

            // Speichere die geänderte Arbeitsmappe
            workbook.Save("modified_example.xlsm");
            Console.WriteLine("File saved with updated OLE links.");
        }
    }
}
```

### Siehe auch

* class [OleObject](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


