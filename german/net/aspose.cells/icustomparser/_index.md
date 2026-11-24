---
title: "Schnittstelle ICustomParser"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.ICustomParser Schnittstelle. Ermöglicht Benutzern, ihren eigenen Wertparser hinzuzufügen, um Zeichenkettenwerte in andere geeignete Zellwertobjekte zu parsen."
type: docs
url: /de/net/aspose.cells/icustomparser/
---
## ICustomParser interface

Ermöglicht Benutzern, ihren eigenen Wertparser hinzuzufügen, um Zeichenkettenwerte in andere geeignete Zellwertobjekte zu konvertieren.

```csharp
public interface ICustomParser
```

## Methoden

| Name | Beschreibung |
| --- | --- |
| [GetFormat](../../aspose.cells/icustomparser/getformat/)() | Gibt das Formatierungsmuster zurück, das dem zuletzt mit [`ParseObject`](./parseobject/) aufgerufenen geparsten Wert entspricht. |
| [ParseObject](../../aspose.cells/icustomparser/parseobject/)(string) | Parst die gegebene Zeichenkette in ein geeignetes Wertobjekt. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ICustomParserDemo
    {
        public static void ICustomParserExample()
        {
            // Benutzerdefinierte Parser-Implementierung
            ICustomParser customParser = new CustomParser();

            // Beispielhafte Verwendung der ParseObject‑Methode
            string valueToParse = "123.45";
            object parsedValue = customParser.ParseObject(valueToParse);
            Console.WriteLine($"Parsed Value: {parsedValue}");

            // Beispielhafte Verwendung der GetFormat‑Methode
            string format = customParser.GetFormat();
            Console.WriteLine($"Format: {format}");
        }
    }

    // Benutzerdefinierte Implementierung von ICustomParser
    public class CustomParser : ICustomParser
    {
        private string lastFormat;

        public object ParseObject(string value)
        {
            // Beispielhafte Parsing‑Logik
            if (double.TryParse(value, out double result))
            {
                lastFormat = "0.00"; // Example format
                return result;
            }
            lastFormat = null;
            return null;
        }

        public string GetFormat()
        {
            return lastFormat;
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


