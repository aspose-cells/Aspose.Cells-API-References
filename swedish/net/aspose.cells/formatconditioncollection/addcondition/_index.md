---
title: "FormatConditionCollection.AddCondition"
second_title: "Aspose.Cells för .NET API‑referens"
description: "FormatConditionCollection‑metod. Lägger till ett formateringsvillkor"
type: docs
url: /sv/net/aspose.cells/formatconditioncollection/addcondition/
---
## AddCondition(FormatConditionType, OperatorType, string, string) {#addcondition_1}

Lägger till ett formateringsvillkor.

```csharp
public int AddCondition(FormatConditionType type, OperatorType operatorType, string formula1, 
    string formula2)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| typ | FormatConditionType | Typen av formateringsvillkor. |
| operatorType | OperatorType | Operatorns typ |
| formula1 | String | Värdet eller uttrycket som är kopplat till villkorsstyrd formatering. Om inmatningsvärdet börjar med '=', tas det som en formel. Annars tas det som ett vanligt värde (text, nummer, bool). För textvärden som börjar med '=', kan användaren ange det som formel i formatet: "=\"=...\"". |
| formula2 | String | Värdet eller uttrycket som är kopplat till villkorsstyrd formatering. Indataformatet är samma som för formula1. |

### Returvärde

Index för formateringsvillkorsobjekt;

### Exempel

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

### Se även

* enum [FormatConditionType](../../formatconditiontype/)
* enum [OperatorType](../../operatortype/)
* class [FormatConditionCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## AddCondition(FormatConditionType) {#addcondition}

Lägg till ett formatvillkor.

```csharp
public int AddCondition(FormatConditionType type)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| typ | FormatConditionType | Typ av formateringsvillkor. |

### Returvärde

Index för formateringsvillkorsobjekt;

### Exempel

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

            // Skapa formateringsvillkor
            int formatIndex = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection conditions = worksheet.ConditionalFormattings[formatIndex];
            
            // Lägg till intervall
            CellArea area = new CellArea
            {
                StartRow = 0,
                StartColumn = 0,
                EndRow = 5,
                EndColumn = 5
            };
            conditions.AddArea(area);

            // Lägg till villkor (returnerar int‑index)
            conditions.AddCondition(FormatConditionType.ColorScale);
            conditions.AddCondition(FormatConditionType.IconSet);
            conditions.AddCondition(FormatConditionType.DataBar);

            workbook.Save("ConditionalFormattingDemo.xlsx");
        }
    }
}
```

### Se även

* enum [FormatConditionType](../../formatconditiontype/)
* class [FormatConditionCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


