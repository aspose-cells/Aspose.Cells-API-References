---
title: "Klasse IndividualFontConfigs"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.IndividualFontConfigs-Klasse. Schriftkonfigurationen für jedes Workbook-Objekt"
type: docs
url: /de/net/aspose.cells/individualfontconfigs/
---
## IndividualFontConfigs class

Schriftkonfigurationen für jedes [`Workbook`](../workbook/) Objekt.

```csharp
public class IndividualFontConfigs
```

## Konstruktoren

| Name | Beschreibung |
| --- | --- |
| [IndividualFontConfigs](individualfontconfigs/)() | Ctor. |

## Methoden

| Name | Beschreibung |
| --- | --- |
| [GetFontSources](../../aspose.cells/individualfontconfigs/getfontsources/)() | Gibt eine Kopie des Arrays zurück, das die Liste der Quellen enthält |
| [GetFontSubstitutes](../../aspose.cells/individualfontconfigs/getfontsubstitutes/)(string) | Gibt ein Array zurück, das Schriftart-Ersatznamen enthält, die verwendet werden, wenn die Originalschriftart nicht vorhanden ist. |
| [SetFontFolder](../../aspose.cells/individualfontconfigs/setfontfolder/)(string, bool) | Legt den Schriftartenordner fest |
| [SetFontFolders](../../aspose.cells/individualfontconfigs/setfontfolders/)(string[], bool) | Legt die Schriftordner fest |
| [SetFontSources](../../aspose.cells/individualfontconfigs/setfontsources/)(FontSourceBase[]) | Legt die Schriftquellen fest. |
| [SetFontSubstitutes](../../aspose.cells/individualfontconfigs/setfontsubstitutes/)(string, string[]) | Legt Schriftart-Ersatznamen für einen gegebenen Originalschriftartnamen fest. |

### Beispiele

```csharp
using System;
using System.IO;
using System.Text;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassIndividualFontConfigsDemo
    {
        public static void Run()
        {
            // Erstelle temporäre Verzeichnisse für Schriftquellen
            string tempFontFolder1 = Path.Combine(Path.GetTempPath(), "FontFolder1_" + Guid.NewGuid().ToString());
            string tempFontFolder2 = Path.Combine(Path.GetTempPath(), "FontFolder2_" + Guid.NewGuid().ToString());
            Directory.CreateDirectory(tempFontFolder1);
            Directory.CreateDirectory(tempFontFolder2);

            // Erstelle Beispiel-CSV-Datei
            string csvFilePath = "sample_data.csv";
            File.WriteAllText(csvFilePath, "Name,Age\nJohn,30\nAlice,25", Encoding.UTF8);

            try
            {
                // Initialisiere Schriftkonfiguration
                IndividualFontConfigs fontConfigs = new IndividualFontConfigs();

                // Setze Schriftart-Ersatz für Arial
                fontConfigs.SetFontSubstitutes("Arial", new string[] { "Times New Roman", "Verdana" });

                // Konfiguriere Schriftverzeichnisse
                fontConfigs.SetFontFolder(tempFontFolder1, false);
                fontConfigs.SetFontFolders(new string[] { tempFontFolder1, tempFontFolder2 }, true);

                // Schriftquellen konfigurieren
                FontSourceBase[] fontSources = {
                    new FolderFontSource(tempFontFolder1, false),
                    new FolderFontSource(tempFontFolder2, true)
                };
                fontConfigs.SetFontSources(fontSources);

                // Textladeoptionen mit Schriftkonfigurationen erstellen
                TxtLoadOptions loadOptions = new TxtLoadOptions(LoadFormat.Csv)
                {
                    FontConfigs = fontConfigs
                };

                // Arbeitsmappe mit konfigurierten Optionen laden
                using (Workbook workbook = new Workbook(csvFilePath, loadOptions))
                {
                    // Als Excel-Datei speichern
                    workbook.Save("output_with_font_config.xlsx");
                }
            }
            finally
            {
                // Temporäre Ressourcen bereinigen
                if (Directory.Exists(tempFontFolder1)) Directory.Delete(tempFontFolder1, true);
                if (Directory.Exists(tempFontFolder2)) Directory.Delete(tempFontFolder2, true);
                if (File.Exists(csvFilePath)) File.Delete(csvFilePath);
            }
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


