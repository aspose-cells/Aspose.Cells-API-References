---
title: "CellsHelper.AddAddInFunction"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "CellsHelper-Methode. Add-In-Funktion hinzufügen"
type: docs
url: /de/net/aspose.cells/cellshelper/addaddinfunction/
---
## CellsHelper.AddAddInFunction method

Add-In-Funktion hinzufügen.

```csharp
[Obsolete("Use WorksheetCollection.RegisterAddInFunction() methods instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public static void AddAddInFunction(string function, int minCountOfParameters, 
    int maxCountOfParameters, ParameterType[] paramersType, ParameterType functionValueType)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Funktion | String | Der Funktionsname. |
| minCountOfParameters | Int32 | Mindestanzahl von Parametern, die diese Funktion erfordert |
| maxCountOfParameters | Int32 | Maximale Anzahl von Parametern, die diese Funktion zulässt. |
| paramersType | ParameterType[] | Der erwartete Parametertyp der Funktion. |
| functionValueType | ParameterType | Der Typ des Funktionswerts. |

### Hinweise

HINWEIS: Dieses Mitglied ist jetzt veraltet. Verwenden Sie stattdessen die Methoden WorksheetCollection.RegisterAddInFunction(). Diese Methode wird 12 Monate nach Januar 2022 entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie möglicherweise erlebt haben.

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsHelperMethodAddAddInFunctionWithStringInt32Int32ParameterTypeDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Parameter für AddAddInFunction definieren
                string functionName = "CUSTOMFUNCTION";
                int minParams = 2;
                int maxParams = 4;
                ParameterType[] paramTypes = new ParameterType[] { ParameterType.Value, ParameterType.Reference };
                ParameterType returnType = ParameterType.Value;

                // Rufen Sie die Methode AddAddInFunction auf
                CellsHelper.AddAddInFunction(functionName, minParams, maxParams, paramTypes, returnType);

                // Verwenden Sie die benutzerdefinierte Funktion in einer Zelle
                worksheet.Cells["A1"].Formula = "=CUSTOMFUNCTION(5,B2)";
                worksheet.Cells["B2"].Value = 10;

                // Formeln berechnen
                workbook.CalculateFormula();

                Console.WriteLine("AddAddInFunction executed successfully. Custom function added and used in A1.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing AddAddInFunction method: {ex.Message}");
            }

            // Ergebnis speichern
            workbook.Save("AddAddInFunctionDemo.xlsx");
        }
    }
}
```

### Siehe auch

* enum [ParameterType](../../parametertype/)
* class [CellsHelper](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


