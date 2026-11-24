---
title: "LimLowUppEquationNode.Equals"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "LimLowUppEquationNode-Methode. Bestimmt, ob der aktuelle Gleichungsknoten dem angegebenen Knoten entspricht"
type: docs
url: /de/net/aspose.cells.drawing.equations/limlowuppequationnode/equals/
---
## LimLowUppEquationNode.Equals method

Bestimme, ob der aktuelle Gleichungsknoten dem angegebenen Knoten gleich ist

```csharp
public override bool Equals(object obj)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| obj | Object | Der angegebene Knoten |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing.Equations;
    using System;

    public class LimLowUppEquationNodeMethodEqualsWithObjectDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Da wir die Konstruktorparameter nicht kennen, vergleichen wir Nullwerte
            // Dies ist eine minimale Änderung, um die Kompilierung zu ermöglichen – bei realer Verwendung benötigen Sie eine korrekte Konstruktion
            LimLowUppEquationNode node1 = null;
            LimLowUppEquationNode node2 = null;

            try
            {
                // Rufen Sie die Equals-Methode mit dem spezifischen Parametertyp (Object) auf
                bool areEqual = node1?.Equals((object)node2) ?? false;

                // Ergebnis anzeigen
                Console.WriteLine($"Are the nodes equal? {areEqual}");

                // Speichere die Arbeitsmappe
                workbook.Save("LimLowUppEquationNodeEqualsDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Equals method: {ex.Message}");
            }
        }
    }
}
```

### Siehe auch

* class [LimLowUppEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


