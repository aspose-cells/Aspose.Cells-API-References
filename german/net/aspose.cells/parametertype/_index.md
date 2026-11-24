---
title: "Enum ParameterType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.ParameterType-Enum. Stellt alle Parametertypen oder Rückgabetypen einer Funktion dar"
type: docs
url: /de/net/aspose.cells/parametertype/
---
## ParameterType enumeration

Stellt den Typ aller Parameter oder den Rückgabewerttyp einer Funktion dar.

```csharp
public enum ParameterType
```

### Werte

| Name | Wert | Beschreibung |
| --- | --- | --- |
| Reference | `0` |  |
| Value | `1` |  |
| Array | `2` |  |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ParameterTypeDemo
    {
        public static void ParameterTypeExample()
        {
            // Erstellen einer Arbeitsmappe und eines Arbeitsblatts, um die Verwendung zu demonstrieren
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Beispielhafte Verwendung des ParameterType-Enums in einer Formelfunktion
            // Angenommen, wir definieren eine benutzerdefinierte Funktion mit spezifischen Parametertypen

            // Definieren Sie ein Array von Parametertypen
            ParameterType[] parameterTypes = new ParameterType[]
            {
                ParameterType.Reference,
                ParameterType.Value,
                ParameterType.Array
            };

            // Beispielhafte Funktion, die diese Parametertypen verwendet
            // Zum Beispiel das Festlegen einer hypothetischen benutzerdefinierten Funktion mit definierten Parametertypen
            // (Hinweis: Die Handhabung benutzerdefinierter Funktionen hängt von den Fähigkeiten der Aspose.Cells-API ab)

            // Speichern Sie die Arbeitsmappe, um die Änderungen zu demonstrieren
            workbook.Save("ParameterTypeExample.xlsx");
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


