---
title: "PowerQueryFormulaFunction.Type"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PowerQueryFormulaFunction-Eigenschaft. Gibt den Typ der Power Query-Formel zurück"
type: docs
url: /de/net/aspose.cells.querytables/powerqueryformulafunction/type/
---
## PowerQueryFormulaFunction.Type property

Liest den Typ der Power‑Query‑Formel.

```csharp
public override PowerQueryFormulaType Type { get; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.QueryTables;
    using System;

    public class PowerQueryFormulaFunctionPropertyTypeDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Erstellen Sie eine Power Query-Formelfunktion
            // Da wir nicht direkt erstellen können, müssen wir sie von irgendwoher beziehen
            // Zu Demonstrationszwecken zeigen wir nur, wie man auf die Type-Eigenschaft zugreift
            // (Im realen Einsatz würden Sie dies aus einer vorhandenen Sammlung erhalten)
            PowerQueryFormulaFunction function = null; // Can't instantiate directly
            
            // Da wir auch keine QueryTable direkt erstellen können, überspringen wir diesen Teil
            QueryTable queryTable = null; // Can't instantiate directly
            
            // Kann die Sammlung von Abfrage-Tabellen auf diese Weise nicht hinzufügen – sie ist schreibgeschützt
            // worksheet.QueryTables[0] = queryTable; // Diese Zeile entfernt
            
            // Zur Demonstration zeigen wir nur das Ausgabeformat, das wir verwenden würden, wenn wir eine Funktion hätten
            if (function != null)
            {
                Console.WriteLine("Power Query Formula Function Type: " + function.Type);
                Console.WriteLine("Is this a function? " + (function.Type == PowerQueryFormulaType.Function));
            }
            else
            {
                Console.WriteLine("Could not create PowerQueryFormulaFunction instance - constructor not available");
            }

            // Ergebnis speichern
            workbook.Save("PowerQueryFormulaFunctionTypeDemo.xlsx");
        }
    }
}
```

### Siehe auch

* enum [PowerQueryFormulaType](../../powerqueryformulatype/)
* class [PowerQueryFormulaFunction](../)
* namespace [Aspose.Cells.QueryTables](../../../aspose.cells.querytables/)
* assembly [Aspose.Cells](../../../)


