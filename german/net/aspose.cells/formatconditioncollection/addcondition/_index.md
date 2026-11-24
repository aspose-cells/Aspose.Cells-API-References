---
title: "FormatConditionCollection.AddCondition"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "FormatConditionCollection-Methode. Fügt eine Formatierungsbedingung hinzu"
type: docs
url: /de/net/aspose.cells/formatconditioncollection/addcondition/
---
## AddCondition(FormatConditionType, OperatorType, string, string) {#addcondition_1}

Fügt eine Formatierungsbedingung hinzu.

```csharp
public int AddCondition(FormatConditionType type, OperatorType operatorType, string formula1, 
    string formula2)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Typ | FormatConditionType | Der Typ der Formatierungsbedingung. |
| operatorType | OperatorType | Der Operator-Typ |
| formula1 | String | Der Wert oder Ausdruck, der mit der bedingten Formatierung verknüpft ist. Wenn der Eingabewert mit '=', beginnt, wird er als Formel behandelt. Andernfalls wird er als einfacher Wert (Text, Zahl, Bool) übernommen. Für Textwerte, die mit '=', beginnen, kann der Benutzer ihn im Format "=\"=...\"" als Formel eingeben. |
| formula2 | String | Der Wert oder Ausdruck, der mit der bedingten Formatierung verknüpft ist. Das Eingabeformat ist dasselbe wie bei formula1. |

### Rückgabewert

Index des Formatierungsbedingungsobjekts;

### Beispiele

```csharp
using System;
using System.Drawing;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FormatConditionCollectionMethodAddConditionWithFormatConditionTypeOperatorTypDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            int index = sheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = sheet.ConditionalFormattings[index];
            
            CellArea ca = new CellArea();
            ca.StartRow = 0;
            ca.EndRow = 10;
            ca.StartColumn = 0;
            ca.EndColumn = 10;
            fcs.AddArea(ca);
            
            int conditionIndex = fcs.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "-50", "-1");
            FormatCondition fc = fcs[conditionIndex];
            fc.Style.Font.Color = Color.Red;
            
            conditionIndex = fcs.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "0", "50");
            fc = fcs[conditionIndex];
            fc.Style.Font.Color = Color.Green;
            
            workbook.Save("output.xlsx");
        }
    }
}
```

### Siehe auch

* enum [FormatConditionType](../../formatconditiontype/)
* enum [OperatorType](../../operatortype/)
* class [FormatConditionCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## AddCondition(FormatConditionType) {#addcondition}

Füge eine Formatbedingung hinzu.

```csharp
public int AddCondition(FormatConditionType type)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Typ | FormatConditionType | Typ der Formatierungsbedingung. |

### Rückgabewert

Index des Formatierungsbedingungsobjekts;

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FormatConditionCollectionMethodAddConditionWithFormatConditionTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Formatbedingungen erstellen
            int formatIndex = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection conditions = worksheet.ConditionalFormattings[formatIndex];
            
            // Bereich hinzufügen
            CellArea area = new CellArea
            {
                StartRow = 0,
                StartColumn = 0,
                EndRow = 5,
                EndColumn = 5
            };
            conditions.AddArea(area);

            // Bedingungen hinzufügen (gibt int-Index zurück)
            conditions.AddCondition(FormatConditionType.ColorScale);
            conditions.AddCondition(FormatConditionType.IconSet);
            conditions.AddCondition(FormatConditionType.DataBar);

            workbook.Save("ConditionalFormattingDemo.xlsx");
        }
    }
}
```

### Siehe auch

* enum [FormatConditionType](../../formatconditiontype/)
* class [FormatConditionCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


