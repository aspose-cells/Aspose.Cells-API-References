---
title: "Klasse LoadFilter"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.LoadFilter Klasse. Stellt den Filter dar, der Optionen zum Laden von Daten beim Laden einer Arbeitsmappe aus einer Vorlage bietet"
type: docs
url: /de/net/aspose.cells/loadfilter/
---
## LoadFilter class

Stellt den Filter dar, der Optionen zum Laden von Daten beim Laden einer Arbeitsmappe aus einer Vorlage bietet.

```csharp
public class LoadFilter
```

## Konstruktoren

| Name | Beschreibung |
| --- | --- |
| [LoadFilter](loadfilter/#constructor)() | Erstellt einen LoadFilter mit den Standardfilteroptionen LoadDataFilterOptions.All. |
| [LoadFilter](loadfilter/#constructor_1)(LoadDataFilterOptions) | Erstellt einen LoadFilter mit den angegebenen Filteroptionen. |

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [LoadDataFilterOptions](../../aspose.cells/loadfilter/loaddatafilteroptions/) { get; set; } | Die Filteroptionen, die angeben, welche Daten geladen werden sollen. |
| virtual [SheetsInLoadingOrder](../../aspose.cells/loadfilter/sheetsinloadingorder/) { get; } | Gibt die zu ladenden Blätter (Indizes) und deren Reihenfolge an. Standard ist null, was bedeutet, dass alle Blätter in der Standardreihenfolge der Vorlagendatei geladen werden. Wenn nicht null und ein Blattindex nicht im zurückgegebenen Array enthalten ist, wird dieses Blatt nicht geladen. |

## Methoden

| Name | Beschreibung |
| --- | --- |
| virtual [StartSheet](../../aspose.cells/loadfilter/startsheet/)(Worksheet) | Bereitet die Filteroptionen vor dem Laden des angegebenen Arbeitsblatts vor. Die Implementierung von LoadFilter durch den Benutzer kann hier die LoadDataFilterOptions ändern, um festzulegen, wie Daten für dieses Arbeitsblatt geladen werden. |

### Hinweise

Der Benutzer kann die Filteroptionen angeben oder sein eigenes LoadFilter implementieren, um festzulegen, wie Daten geladen werden.

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class LoadFilterDemo
    {
        public static void LoadFilterExample()
        {
            // Erstelle LoadOptions und setze LoadFilter
            LoadOptions opts = new LoadOptions();
            opts.LoadFilter = new CustomLoadFilter();

            // Lade die Arbeitsmappe mit den angegebenen LoadOptions
            Workbook wb = new Workbook("LoadFilterExample_original.xlsx", opts);

            // Speichere die Arbeitsmappe, um die Wirkung des LoadFilter zu sehen
            wb.Save("LoadFilterExample.xlsx");
        }

        // Benutzerdefinierte LoadFilter-Implementierung
        public class CustomLoadFilter : LoadFilter
        {
            public override void StartSheet(Worksheet sheet)
            {
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


