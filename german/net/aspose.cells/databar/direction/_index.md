---
title: "DataBar.Direction"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "DataBar-Eigenschaft. Gibt die Richtung zurück, in der der Datenbalken angezeigt wird, oder legt sie fest"
type: docs
url: /de/net/aspose.cells/databar/direction/
---
## DataBar.Direction property

Liest oder legt die Richtung fest, in der der Datenbalken angezeigt wird.

```csharp
public TextDirectionType Direction { get; set; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class DataBarPropertyDirectionDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Beispieldaten hinzufügen, um Datenbalken zu demonstrieren
            for (int i = 0; i < 10; i++)
            {
                worksheet.Cells[i, 0].Value = i + 1;  // Values from 1 to 10 in column A
            }

            // Bedingte Formatierung für Datenbalken hinzufügen
            ConditionalFormattingCollection conditionalFormattings = worksheet.ConditionalFormattings;
            int index = conditionalFormattings.Add();
            FormatConditionCollection conditionalFormatting = conditionalFormattings[index];
            
            // Zellbereich für die Formatierungsbedingung definieren
            CellArea cellArea = new CellArea
            {
                StartRow = 0,
                StartColumn = 0,
                EndRow = 9,
                EndColumn = 0
            };
            conditionalFormatting.AddArea(cellArea);

            // DataBar-Bedingung hinzufügen und Referenz erhalten
            int conditionIndex = conditionalFormatting.AddCondition(FormatConditionType.DataBar);
            FormatCondition condition = conditionalFormatting[conditionIndex];

            DataBar dataBar = condition.DataBar;

            // Aktuellen Direction-Wert anzeigen
            Console.WriteLine("Initial DataBar Direction: " + dataBar.Direction);

            // Richtung zu RightToLeft ändern und demonstrieren
            dataBar.Direction = TextDirectionType.RightToLeft;

            // Zusätzliche Konfiguration für bessere Visualisierung
            dataBar.Color = System.Drawing.Color.LightGreen;
            dataBar.MinCfvo.Type = FormatConditionValueType.Min;
            dataBar.MaxCfvo.Type = FormatConditionValueType.Max;

            // Arbeitsmappe speichern, um den Effekt zu zeigen
            workbook.Save("DataBarDirectionDemo.xlsx");
        }
    }
}
```

### Siehe auch

* enum [TextDirectionType](../../textdirectiontype/)
* class [DataBar](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


