---
title: "AbstractTextLoadOptions.LoadStyleStrategy"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "AbstractTextLoadOptions-Eigenschaft. Gibt die Strategie an, die beim Anwenden von Stil auf geparste Werte verwendet wird, wenn ein Zeichenkettenwert in eine Zahl oder ein Datum/Uhrzeit konvertiert wird"
type: docs
url: /de/net/aspose.cells/abstracttextloadoptions/loadstylestrategy/
---
## AbstractTextLoadOptions.LoadStyleStrategy property

Gibt die Strategie an, die Formatierung für geparste Werte anzuwenden, wenn ein Zeichenkettenwert in Zahl oder Datum/Uhrzeit konvertiert wird.

```csharp
public TxtLoadStyleStrategy LoadStyleStrategy { get; set; }
```

### Beispiele

```csharp
using System;
using System.IO;
using System.Text;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class AbstractTextLoadOptionsPropertyLoadStyleStrategyDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Legen Sie einen benutzerdefinierten Stil zur Demonstration fest
            Style customStyle = workbook.CreateStyle();
            customStyle.Font.Name = "Arial";
            customStyle.Font.Size = 12;
            customStyle.Font.Color = System.Drawing.Color.Blue;
            customStyle.Pattern = BackgroundType.Solid;
            customStyle.ForegroundColor = System.Drawing.Color.LightYellow;

            // Wende den Stil auf eine Zelle an
            Cell cell = cells["A1"];
            cell.PutValue("Sample Text");
            cell.SetStyle(customStyle);

            // Erstellen Sie CSV-Daten
            string csvData = "Data1,Data2\nValue1,Value2";
            byte[] byteArray = Encoding.ASCII.GetBytes(csvData);
            MemoryStream stream = new MemoryStream(byteArray);

            // Erstellen Sie Text-Ladeoptionen mit LoadStyleStrategy
            TxtLoadOptions loadOptions = new TxtLoadOptions(LoadFormat.Csv)
            {
                LoadStyleStrategy = TxtLoadStyleStrategy.BuiltIn
            };

            // Importieren Sie die CSV-Daten mit den angegebenen Ladeoptionen
            cells.ImportCSV(stream, loadOptions, 0, 0);

            // Speichere die Arbeitsmappe, um das Ergebnis zu demonstrieren
            workbook.Save("LoadStyleStrategyDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Siehe auch

* enum [TxtLoadStyleStrategy](../../txtloadstylestrategy/)
* class [AbstractTextLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


