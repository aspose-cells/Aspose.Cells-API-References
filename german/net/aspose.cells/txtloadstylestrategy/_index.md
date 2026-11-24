---
title: "Enum TxtLoadStyleStrategy"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.TxtLoadStyleStrategy enum. Gibt an, wie Stil für geparste Werte angewendet wird, wenn ein Zeichenfolgenwert in eine Zahl oder ein Datum/Uhrzeit konvertiert wird."
type: docs
url: /de/net/aspose.cells/txtloadstylestrategy/
---
## TxtLoadStyleStrategy enumeration

Gibt an, wie der Stil für geparste Werte angewendet wird, wenn ein Zeichenfolgenwert in eine Zahl oder ein Datum/Uhrzeit konvertiert wird.

```csharp
public enum TxtLoadStyleStrategy
```

### Werte

| Name | Wert | Beschreibung |
| --- | --- | --- |
| None | `0` | Setzt keinen Stil für den geparsten Wert. |
| BuiltIn | `1` | Setzen Sie den Stil als integrierte Zahl/Datum‑Uhrzeit, wenn der geparste Wert einfache numerische oder Datum‑Uhrzeit‑Werte ist. |
| ExactFormat | `2` | Legen Sie das genaue benutzerdefinierte Format für den geparsten Wert fest, damit der formatierte Wert dem ursprünglichen Eingabewert entspricht. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class TxtLoadStyleStrategyDemo
    {
        public static void TxtLoadStyleStrategyExample()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Definieren Sie einen Beispiel‑CSV‑Inhalt.
            string csvContent = "Name,Date,Value\nJohn,2023-01-01,100\nDoe,2023-01-02,200";

            // Speichern Sie den CSV‑Inhalt in einer temporären Datei.
            string tempCsvFilePath = "sample.csv";
            System.IO.File.WriteAllText(tempCsvFilePath, csvContent);

            // Erstellen Sie TxtLoadOptions und setzen Sie die LoadStyleStrategy.
            TxtLoadOptions loadOptions = new TxtLoadOptions();
            loadOptions.LoadStyleStrategy = TxtLoadStyleStrategy.ExactFormat;

            // Laden Sie die CSV‑Datei in die Arbeitsmappe.
            workbook = new Workbook(tempCsvFilePath, loadOptions);

            // Speichere die Arbeitsmappe in einer Excel‑Datei
            workbook.Save("TxtLoadStyleStrategyExample.xlsx");

            // Bereinigen Sie die temporäre CSV‑Datei.
            System.IO.File.Delete(tempCsvFilePath);

            Console.WriteLine("Workbook created and saved successfully.");
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


