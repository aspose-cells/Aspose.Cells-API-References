---
title: "XmlLoadOptions.StartCell"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "XmlLoadOptions-Eigenschaft. Gibt die Startzelle zurück und legt sie fest"
type: docs
url: /de/net/aspose.cells/xmlloadoptions/startcell/
---
## XmlLoadOptions.StartCell property

Liest und setzt die Startzelle.

```csharp
public string StartCell { get; set; }
```

### Hinweise

Funktioniert nur, wenn die Datei kein SpreadsheetML ist oder XML nicht nach Excel zugeordnet wird.

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class XmlLoadOptionsPropertyStartCellDemo
    {
        public static void Run()
        {
            // Erstelle eine Instanz von XmlLoadOptions
            XmlLoadOptions options = new XmlLoadOptions();

            // Legen Sie die Startzelle für den XML-Datenimport fest
            options.StartCell = "B2";

            // Lade eine XML-Datei in ein Workbook mit den angegebenen Optionen
            Workbook workbook = new Workbook("input.xml", options);

            // Greife auf das erste Arbeitsblatt zu
            Worksheet worksheet = workbook.Worksheets[0];

            // Geben Sie den Wert der Startzelle aus, um die Eigenschaft zu demonstrieren
            Console.WriteLine("Value at start cell (B2): " + worksheet.Cells["B2"].Value);

            // Speichere die Arbeitsmappe
            workbook.Save("output.xlsx");
        }
    }
}
```

### Siehe auch

* class [XmlLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


