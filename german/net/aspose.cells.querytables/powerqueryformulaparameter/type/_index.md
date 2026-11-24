---
title: "PowerQueryFormulaParameter.Type"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PowerQueryFormulaParameter-Eigenschaft. Gibt den Typ der Power‑Query‑Formel zurück"
type: docs
url: /de/net/aspose.cells.querytables/powerqueryformulaparameter/type/
---
## PowerQueryFormulaParameter.Type property

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

    public class PowerQueryFormulaParameterPropertyTypeDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            try
            {
                // Da wir nicht direkt ein PowerQueryFormulaParameter erstellen können, ohne die erforderlichen Konstruktorparameter zu kennen,
                // zeigen wir, wie man über die Parameter einer vorhandenen Abfrage‑Tabelle auf die Type‑Eigenschaft zugreift
                Console.WriteLine("This demo shows how to access the Type property of PowerQueryFormulaParameter.");
                
                // In einem realen Szenario würden Sie dies von einer vorhandenen Abfrage‑Tabelle aus zugreifen
                // Zu Demonstrationszwecken zeigen wir, wie man den Typ prüft, wenn Sie eine Instanz hätten
                PowerQueryFormulaParameter parameter = null; // This would normally come from a query table
                
                if (parameter != null)
                {
                    // Zeigen Sie den Wert der Type‑Eigenschaft an (schreibgeschützte Eigenschaft)
                    Console.WriteLine($"PowerQueryFormulaParameter Type: {parameter.Type}");
                    
                    // Mögliche Enum‑Werte anzeigen
                    Console.WriteLine("Possible PowerQueryFormulaType values:");
                    foreach (PowerQueryFormulaType type in Enum.GetValues(typeof(PowerQueryFormulaType)))
                    {
                        Console.WriteLine($"- {type}");
                    }
                }
                else
                {
                    Console.WriteLine("No PowerQueryFormulaParameter instance available for demonstration.");
                }
                
                // Speichere die Arbeitsmappe
                workbook.Save("TypeDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Siehe auch

* enum [PowerQueryFormulaType](../../powerqueryformulatype/)
* class [PowerQueryFormulaParameter](../)
* namespace [Aspose.Cells.QueryTables](../../../aspose.cells.querytables/)
* assembly [Aspose.Cells](../../../)


