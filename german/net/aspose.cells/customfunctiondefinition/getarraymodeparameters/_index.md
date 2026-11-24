---
title: "CustomFunctionDefinition.GetArrayModeParameters"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "CustomFunctionDefinition-Methode. Gibt die Indizes der angegebenen benutzerdefinierten Funktionsparameter zurück, die im Array-Modus berechnet werden müssen"
type: docs
url: /de/net/aspose.cells/customfunctiondefinition/getarraymodeparameters/
---
## CustomFunctionDefinition.GetArrayModeParameters method

Liest die Indizes der Parameter der angegebenen benutzerdefinierten Funktion, die im Arraymodus berechnet werden müssen.

```csharp
public virtual int[] GetArrayModeParameters(string functionName)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| functionName | String | Name der benutzerdefinierten Funktion. |

### Rückgabewert

Indizes der Parameter, die für die angegebene benutzerdefinierte Funktion im Array-Modus berechnet werden müssen. Standard ist null, es gibt keinen Parameter, der im Array-Modus für die benutzerdefinierte Funktion berechnet werden muss.

### Hinweise

Für einen Ausdruck, der berechnet werden muss, zum Beispiel A:A+B:B: Im Wertmodus wird er in der Regel zu einem einzelnen Wert basierend auf der aktuellen Zellenbasis berechnet. Im Array-Modus hingegen werden alle Werte von A1+B1, A2+B2, A3+B3, ... berechnet und für die Berechnung verwendet.

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CustomFunctionDefinitionMethodGetArrayModeParametersWithStringDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Eine Instanz von CustomFunctionDefinition erstellen
            CustomFunctionDefinition customFunction = new CustomFunctionDefinition();

            try
            {
                // Rufen Sie GetArrayModeParameters mit einem Funktionsnamen-Parameter auf
                string functionName = "SUM";
                int[] result = customFunction.GetArrayModeParameters(functionName);

                // Ergebnis anzeigen
                if (result != null)
                {
                    Console.WriteLine("Array mode parameters for function '{0}':", functionName);
                    foreach (int param in result)
                    {
                        Console.WriteLine(param);
                    }
                }
                else
                {
                    Console.WriteLine("No array mode parameters defined for function '{0}'", functionName);
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetArrayModeParameters method: {ex.Message}");
            }

            // Speichere die Arbeitsmappe
            workbook.Save("CustomFunctionDefinitionGetArrayModeParametersDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [CustomFunctionDefinition](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


