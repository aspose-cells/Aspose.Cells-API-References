---
title: "Schnittstelle IFilePathProvider"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.IFilePathProvider Schnittstelle. Stellt den Anbieter des exportierten Dateipfads dar"
type: docs
url: /de/net/aspose.cells/ifilepathprovider/
---
## IFilePathProvider interface

Stellt den Anbieter für den exportierten Dateipfad dar.

```csharp
public interface IFilePathProvider
```

## Methoden

| Name | Beschreibung |
| --- | --- |
| [GetFullName](../../aspose.cells/ifilepathprovider/getfullname/)(string) | Ermittelt den vollständigen Pfad der Datei anhand des Arbeitsblattnamens, wenn das Arbeitsblatt separat nach HTML exportiert wird. So können die Verweise zwischen den Arbeitsblättern korrekt exportiert werden. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class IFilePathProviderDemo : IFilePathProvider
    {
        // Implementierung der GetFullName-Methode aus der IFilePathProvider‑Schnittstelle
        public string GetFullName(string sheetName)
        {
            // Zur Demonstration wird ein einfacher Dateipfad basierend auf dem Blattnamen zurückgegeben
            return $"{sheetName}.html";
        }

        public static void IFilePathProviderExample()
        {
            // Erstelle eine neue Arbeitsmappe und füge einige Daten hinzu
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Hello");
            worksheet.Cells["A2"].PutValue("World");

            // Erstelle HtmlSaveOptions und setze den FilePathProvider
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            saveOptions.FilePathProvider = new IFilePathProviderDemo();

            // Speichere das Arbeitsbuch im HTML‑Format
            workbook.Save("IFilePathProviderExample.html", saveOptions);

            Console.WriteLine("Workbook saved to HTML with custom file paths.");
        }
    }


}
```

### Siehe auch

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


