---
title: "XmlLoadOptions.StartCell"
second_title: "Aspose.Cells för .NET API‑referens"
description: "XmlLoadOptions-egenskap. Hämtar och anger startcellen"
type: docs
url: /sv/net/aspose.cells/xmlloadoptions/startcell/
---
## XmlLoadOptions.StartCell property

Hämtar och anger startcellen.

```csharp
public string StartCell { get; set; }
```

### Anmärkningar

Fungerar endast när filen inte är speadsheetML eller mappning av XML till Excel.

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class XmlLoadOptionsPropertyStartCellDemo
    {
        public static void Run()
        {
            // Skapa en instans av XmlLoadOptions
            XmlLoadOptions options = new XmlLoadOptions();

            // Ange startcellen för XML-datainmatning
            options.StartCell = "B2";

            // Läs in en XML-fil i en Workbook med de angivna alternativen
            Workbook workbook = new Workbook("input.xml", options);

            // Åtkomst till det första kalkylbladet
            Worksheet worksheet = workbook.Worksheets[0];

            // Skriv ut värdet från startcellen för att demonstrera egenskapen
            Console.WriteLine("Value at start cell (B2): " + worksheet.Cells["B2"].Value);

            // Spara arbetsboken
            workbook.Save("output.xlsx");
        }
    }
}
```

### Se även

* class [XmlLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


