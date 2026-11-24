---
title: "FormatCondition.Type"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "FormatCondition-Eigenschaft. Ruft ab und legt fest, ob der Typ der bedingten Formatierung verwendet wird."
type: docs
url: /de/net/aspose.cells/formatcondition/type/
---
## FormatCondition.Type property

Liest und setzt, ob der Typ der bedingten Formatierung gesetzt ist.

```csharp
public FormatConditionType Type { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FormatConditionPropertyTypeDemo
    {
        public static void Run()
        {
            // Erstelle eine Arbeitsmappe
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Fügen Sie Beispieldaten hinzu
            sheet.Cells["A1"].PutValue(10);
            sheet.Cells["A2"].PutValue(20);
            sheet.Cells["A3"].PutValue(30);

            // Bedingte Formatierung erstellen
            int index = sheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = sheet.ConditionalFormattings[index];
            
            // Fügen Sie eine Formatbedingung mit Ausdruckstyp hinzu (korrigierte Parameter)
            int conditionIndex = fcs.AddCondition(FormatConditionType.Expression, OperatorType.None, "=A1>5", null);
            FormatCondition fc = fcs[conditionIndex];
            
            // Legen Sie den Stil für die Bedingung fest
            Style style = workbook.CreateStyle();
            style.Font.Color = System.Drawing.Color.Red;
            fc.Style = style;

            // Demonstriere die Verwendung der Type‑Eigenschaft
            Console.WriteLine("Format Condition Type: " + fc.Type);
            
            // Speichere die Arbeitsmappe
            workbook.Save("FormatConditionPropertyTypeDemo.xlsx");
        }
    }
}
```

### Siehe auch

* enum [FormatConditionType](../../formatconditiontype/)
* class [FormatCondition](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


