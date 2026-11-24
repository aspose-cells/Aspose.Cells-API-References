---
title: "Klasse AbstractLowCodeSaveOptionsProvider"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.LowCode.AbstractLowCodeSaveOptionsProvider class. Implementierung zur Bereitstellung mehrerer Speicheroptionen für Prozesse, die mehrere Ausgaben benötigen. Zum Beispiel erfordert die SpreadsheetSplitter‑Funktion mehrere Ziele, um die geteilten Dateien zu speichern"
type: docs
url: /de/net/aspose.cells.lowcode/abstractlowcodesaveoptionsprovider/
---
## AbstractLowCodeSaveOptionsProvider class

Implementierung zur Bereitstellung mehrerer Speicheroptionen für Prozesse, die mehrere Ausgaben benötigen. Zum Beispiel erfordert die [`SpreadsheetSplitter`](../spreadsheetsplitter/)-Funktion mehrere Ziele, um die geteilten Dateien zu speichern.

```csharp
public abstract class AbstractLowCodeSaveOptionsProvider
```

## Methoden

| Name | Beschreibung |
| --- | --- |
| virtual [Finish](../../aspose.cells.lowcode/abstractlowcodesaveoptionsprovider/finish/)(LowCodeSaveOptions) | Gibt Ressourcen frei, nachdem der aktuell geteilte Teil verarbeitet wurde. |
| abstract [GetSaveOptions](../../aspose.cells.lowcode/abstractlowcodesaveoptionsprovider/getsaveoptions/)(SplitPartInfo) | Ruft die Speicheroptionen ab, aus denen die Ausgabeeinstellungen für den aktuell geteilten Teil erhalten werden. Die Rückgabe von null bedeutet, den angegebenen Teil zu überspringen. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class LowCodeClassAbstractLowCodeSaveOptionsProviderDemo
    {
        public static void Run()
        {
            // Erstellen Sie einen benutzerdefinierten Provider, indem Sie AbstractLowCodeSaveOptionsProvider erweitern
            var customProvider = new CustomSaveOptionsProvider();

            // Erstellen Sie eine Arbeitsmappe und ein Arbeitsblatt
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Einige Daten befüllen
            worksheet.Cells["A1"].PutValue("Test Data");
            
            // Erstelle Split-Teil-Informationen – bei realer Verwendung würden diese von der API kommen
            // Da wir es nicht direkt konstruieren können, übergeben wir einfach null zur Demonstration
            SplitPartInfo splitPartInfo = null;
            
            // Speicheroptionen vom Provider abrufen
            LowCodeSaveOptions saveOptions = customProvider.GetSaveOptions(splitPartInfo);
            
            // Speicheroptionen konfigurieren (Beispiel)
            saveOptions.SaveFormat = SaveFormat.Xlsx;
            
            // Demonstriere den Abschluss des Prozesses
            customProvider.Finish(saveOptions);
            
            // Arbeitsmappe speichern (nicht direkt mit dem Provider verbunden, nur zur Demo)
            workbook.Save("LowCodeSaveOptionsDemo.xlsx");
        }
    }

    // Benutzerdefinierte Implementierung von AbstractLowCodeSaveOptionsProvider
    public class CustomSaveOptionsProvider : AbstractLowCodeSaveOptionsProvider
    {
        public override LowCodeSaveOptions GetSaveOptions(SplitPartInfo part)
        {
            // Erstelle und gib benutzerdefinierte Speicheroptionen basierend auf Teilinformationen zurück
            return new LowCodeSaveOptions()
            {
                SaveFormat = SaveFormat.Xlsx
                // CachedFileFolder entfernt, da es in LowCodeSaveOptions nicht existiert
            };
        }

        public override void Finish(LowCodeSaveOptions part)
        {
            // Aufräum- oder Abschlusslogik hier
            Console.WriteLine("Save operation completed for part");
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells.LowCode](../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../)


