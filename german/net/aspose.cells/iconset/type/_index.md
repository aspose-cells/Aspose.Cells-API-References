---
title: "IconSet.Type"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "IconSet-Eigenschaft. Gibt den anzuzeigenden Symbolsatztyp zurück oder setzt ihn. Das Festlegen des Typs prüft automatisch, ob die aktuelle Anzahl von Cfvoss mit dem neuen Typ übereinstimmt. Falls nicht, werden alte Cfvos bereinigt und Standard-Cfvos hinzugefügt."
type: docs
url: /de/net/aspose.cells/iconset/type/
---
## IconSet.Type property

Abrufen oder Festlegen des anzuzeigenden Symbolsettyps. Das Festlegen des Typs prüft automatisch, ob die aktuelle Anzahl der Cfvos mit dem neuen Typ übereinstimmt. Falls nicht, werden alte Cfvos bereinigt und Standard‑Cfvos hinzugefügt.

```csharp
public IconSetType Type { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class IconSetPropertyTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            int index = sheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = sheet.ConditionalFormattings[index];

            CellArea ca = new CellArea
            {
                StartRow = 0,
                EndRow = 2,
                StartColumn = 0,
                EndColumn = 0
            };
            fcs.AddArea(ca);

            int idx = fcs.AddCondition(FormatConditionType.IconSet);
            FormatCondition cond = fcs[idx];
            IconSet iconSet = cond.IconSet;

            // Demonstriere die Verwendung der Type‑Eigenschaft
            iconSet.Type = IconSetType.Arrows3;

            sheet.Cells["A1"].PutValue(10);
            sheet.Cells["A2"].PutValue(120);
            sheet.Cells["A3"].PutValue(260);

            workbook.Save("IconSetExample.xlsx");
        }
    }
}
```

### Siehe auch

* enum [IconSetType](../../iconsettype/)
* class [IconSet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


