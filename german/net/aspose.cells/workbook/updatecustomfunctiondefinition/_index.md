---
title: "Workbook.UpdateCustomFunctionDefinition"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Workbook-Methode. Aktualisiert die Definition benutzerdefinierter Funktionen"
type: docs
url: /de/net/aspose.cells/workbook/updatecustomfunctiondefinition/
---
## Workbook.UpdateCustomFunctionDefinition method

Aktualisiert die Definition benutzerdefinierter Funktionen.

```csharp
public void UpdateCustomFunctionDefinition(CustomFunctionDefinition definition)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Definition | CustomFunctionDefinition | Spezielle Definition benutzerdefinierter Funktionen für die besonderen Anforderungen des Benutzers. |

### Hinweise

Diese Methode kann für einige spezielle Szenarien verwendet werden. Zum Beispiel, wenn der Benutzer einige Parameter benutzerdefinierter Funktionen im Array‑Modus berechnen muss, kann der Benutzer seine eigene Definition mit implementiertem [`GetArrayModeParameters`](../../customfunctiondefinition/getarraymodeparameters/) für diese Funktionen bereitstellen. Nachdem die Formeldaten aktualisiert wurden, werden die angegebenen Parameter im Array‑Modus automatisch berechnet, wenn die entsprechenden benutzerdefinierten Funktionen ausgewertet werden.

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodUpdateCustomFunctionDefinitionWithCustomFunctionDDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            
            // Fügen Sie Beispieldaten hinzu
            sheet.Cells["B1"].PutValue(1);
            sheet.Cells["C1"].PutValue(2);
            sheet.Cells["B2"].PutValue(4);
            sheet.Cells["C2"].PutValue(8);

            // Erstelle eine benutzerdefinierte Berechnungs-Engine
            var customEngine = new MyCustomCalculationEngine();
            
            // Setzen Sie die Berechnungsoptionen mit benutzerdefinierter Engine
            CalculationOptions options = new CalculationOptions
            {
                CustomEngine = customEngine
            };

            // Aktualisiere die Definition der benutzerdefinierten Funktion
            wb.UpdateCustomFunctionDefinition(new MyCustomFunctionDefinition());

            // Formel mit benutzerdefinierter Funktion festlegen
            sheet.Cells["A1"].Formula = "=MYFUNC(B:B+C:C)";
            
            // Formeln berechnen
            wb.CalculateFormula(options);

            // Gib das Ergebnis aus
            Console.WriteLine("Custom function result: " + sheet.Cells["A1"].Value);
        }
    }

    public class MyCustomFunctionDefinition : CustomFunctionDefinition
    {
        public override int[] GetArrayModeParameters(string functionName)
        {
            // Gib die Parameterindizes zurück, die im Array‑Modus verarbeitet werden sollen
            return new int[] { 0 }; // First parameter is array mode
        }
    }

    public class MyCustomCalculationEngine : AbstractCalculationEngine
    {
        public override void Calculate(CalculationData data)
        {
            if (data.FunctionName == "MYFUNC")
            {
                double sum = 0;
                var paramValue = data.GetParamValue(0);
                
                if (paramValue is object[,] arrayValue)
                {
                    foreach (var val in arrayValue)
                    {
                        if (val != null)
                        {
                            sum += Convert.ToDouble(val);
                        }
                    }
                }
                else
                {
                    sum += Convert.ToDouble(paramValue);
                }
                data.CalculatedValue = sum * 2; // Custom calculation logic
            }
        }
    }
}
```

### Siehe auch

* class [CustomFunctionDefinition](../../customfunctiondefinition/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


