---
title: "Klasse IconSet"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.IconSet Klasse. Beschreibe die IconSet-Bedingte-Formatierungsregel. Diese bedingte Formatierungsregel wendet Symbole auf Zellen basierend auf deren Werten an."
type: docs
url: /de/net/aspose.cells/iconset/
---
## IconSet class

Beschreibt die bedingte Formatierungsregel IconSet. Diese bedingte Formatierungsregel wendet Symbole auf Zellen basierend auf deren Werten an.

```csharp
public class IconSet
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [CfIcons](../../aspose.cells/iconset/cficons/) { get; } | Abrufen des[`ConditionalFormattingIcon`](../conditionalformattingicon/) aus der Sammlung |
| [Cfvos](../../aspose.cells/iconset/cfvos/) { get; } | Abrufen der CFValueObjects-Instanz. |
| [IsCustom](../../aspose.cells/iconset/iscustom/) { get; } | Gibt an, ob das Symbolset benutzerdefiniert ist. Standardwert ist false. |
| [Reverse](../../aspose.cells/iconset/reverse/) { get; set; } | Abrufen oder Festlegen des Flags, das angibt, ob die Standardreihenfolge der Symbole in diesem Symbolset umgekehrt wird. Standardwert ist false. |
| [ShowValue](../../aspose.cells/iconset/showvalue/) { get; set; } | Abrufen oder Festlegen des Flags, das angibt, ob die Werte der Zellen angezeigt werden, auf die dieses Symbolset angewendet wird. Standardwert ist true. |
| [Type](../../aspose.cells/iconset/type/) { get; set; } | Abrufen oder Festlegen des anzuzeigenden Symbolsettyps. Das Festlegen des Typs prüft automatisch, ob die aktuelle Anzahl der Cfvos mit dem neuen Typ übereinstimmt. Falls nicht, werden alte Cfvos bereinigt und Standard‑Cfvos hinzugefügt. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class IconSetDemo
    {
        public static void IconSetExample()
        {
            // Instanziieren eines Workbook-Objekts
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Fügt eine leere bedingte Formatierung hinzu
            int index = sheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = sheet.ConditionalFormattings[index];

            // Setzt den Bereich der bedingten Formatierung
            CellArea ca = new CellArea
            {
                StartRow = 0,
                EndRow = 2,
                StartColumn = 0,
                EndColumn = 0
            };
            fcs.AddArea(ca);

            // Fügt Bedingung hinzu
            int idx = fcs.AddCondition(FormatConditionType.IconSet);
            FormatCondition cond = fcs[idx];

            // Symbolset abrufen
            IconSet iconSet = cond.IconSet;

            // Symboltyp festlegen
            iconSet.Type = IconSetType.Arrows3;

            // Zusätzliche Eigenschaften festlegen
            iconSet.ShowValue = true;
            iconSet.Reverse = false;

            // Zellwerte einfügen
            sheet.Cells["A1"].PutValue(10);
            sheet.Cells["A2"].PutValue(120);
            sheet.Cells["A3"].PutValue(260);

            // Die Excel-Datei speichern
            workbook.Save("IconSetExample.xlsx");
            workbook.Save("IconSetExample.pdf");
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


