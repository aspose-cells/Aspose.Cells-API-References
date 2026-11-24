---
title: "Enum LoadDataFilterOptions"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.LoadDataFilterOptions-Enum. Repräsentiert die Optionen zum Filtern von Daten beim Laden einer Arbeitsmappe aus einer Vorlage"
type: docs
url: /de/net/aspose.cells/loaddatafilteroptions/
---
## LoadDataFilterOptions enumeration

Stellt die Optionen zum Filtern von Daten beim Laden einer Arbeitsmappe aus einer Vorlage dar.

```csharp
public enum LoadDataFilterOptions
```

### Werte

| Name | Wert | Beschreibung |
| --- | --- | --- |
| None | `0` | Lade keine Daten für das Tabellenblatt |
| All | `2147483647` | Alle laden |
| CellBlank | `1` | Lade Zellen, deren Wert leer ist |
| CellString | `2` | Lade Zellen, deren Wert ein Text ist |
| CellNumeric | `4` | Lade Zellen, deren Wert numerisch ist (einschließlich Datum/Zeit) |
| CellError | `8` | Lade Zellen, deren Wert ein Fehler ist |
| CellBool | `16` | Lade Zellen, deren Wert bool ist |
| CellValue | `31` | Lade nur Zellenwerte (alle Werttypen) |
| Formula | `32` | Lade Zellformeln. |
| CellData | `67108927` | Lade Zellendaten einschließlich Werte, Formeln und Formatierung |
| Chart | `256` | Lade Diagramme |
| Shape | `402653696` | Lade Formen |
| Drawing | `402653952` | Zeichenobjekte (einschließlich Chart, Picture, OleObject und aller anderen Zeichenobjekte) |
| MergedArea | `1024` | Lade zusammengeführte Zellen |
| ConditionalFormatting | `2048` | Lade bedingte Formatierung |
| DataValidation | `4096` | Lade Datenüberprüfungen |
| PivotTable | `8192` | Lade Pivot-Tabellen |
| Table | `16384` | Lade Tabellen |
| Hyperlinks | `32768` | Lade Hyperlinks |
| SheetSettings | `65536` | Lade Einstellungen für das Arbeitsblatt |
| SheetData | `403701759` | Lade alle Daten des Arbeitsblatts, wie Zellen-Daten, Einstellungen, Objekte, ...etc. |
| BookSettings | `1048576` | Lade Einstellungen für die Arbeitsmappe |
| Settings | `1114112` | Lade Einstellungen für Arbeitsmappe und Arbeitsblatt |
| XmlMap | `2097152` | Lade XmlMap |
| Structure | `4194304` | Lade Struktur der Arbeitsmappe |
| DocumentProperties | `8388608` | Lade Dokumenteigenschaften |
| DefinedNames | `16777216` | Lade definierte Namensobjekte |
| VBA | `33554432` | Lade VBA-Projekte |
| Style | `67108864` | Lade Stile für die Zellformatierung |
| Picture | `134217728` | Bilder laden |
| OleObject | `268435456` | OleObjects laden |
| Revision | `536870912` | Versionsprotokolle laden |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class LoadDataFilterOptionsDemo
    {
        public static void LoadDataFilterOptionsExample()
        {
            // Eine neue LoadOptions-Instanz erstellen
            LoadOptions loadOptions = new LoadOptions();

            // Eine benutzerdefinierte LoadFilter-Implementierung erstellen
            loadOptions.LoadFilter = new CustomLoadFilter();

            // Lade die Arbeitsmappe mit den angegebenen Ladeoptionen
            Workbook workbook = new Workbook("LoadDataFilterOptionsExample_original.xlsx", loadOptions);

            // Die Arbeitsmappe speichern, um die geladenen Daten zu überprüfen
            workbook.Save("LoadDataFilterOptionsExample.xlsx");
        }

        // Benutzerdefinierte LoadFilter-Implementierung
        private class CustomLoadFilter : LoadFilter
        {
            public override void StartSheet(Worksheet sheet)
            {
                // Unterschiedliche Filteroptionen basierend auf dem Blattnamen anwenden
                if (sheet.Name == "Sheet1")
                {
                    LoadDataFilterOptions = LoadDataFilterOptions.All;
                }
                else
                {
                    LoadDataFilterOptions = LoadDataFilterOptions.Structure;
                }
            }
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


