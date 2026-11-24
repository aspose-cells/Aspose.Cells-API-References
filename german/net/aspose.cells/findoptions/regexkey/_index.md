---
title: "FindOptions.RegexKey"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "FindOptions-Eigenschaft. Gibt an, ob der gesuchte Schlüssel ein Regex ist. Wenn true, wird der gesuchte Schlüssel als Regex behandelt und geparst. Andernfalls wird der Schlüssel gemäß den Regeln in MS Excel geparst."
type: docs
url: /de/net/aspose.cells/findoptions/regexkey/
---
## FindOptions.RegexKey property

Gibt an, ob der gesuchte Schlüssel ein Regex ist. Wenn true, wird der gesuchte Schlüssel als Regex behandelt und geparst. Andernfalls wird der Schlüssel gemäß den Regeln in MS Excel geparst.

```csharp
public bool RegexKey { get; set; }
```

### Hinweise

Obwohl der Suchschlüssel als Regex angegeben wurde, kann er gemäß dem angegebenen [`LookAtType`](../lookattype/) umformuliert werden. Zum Beispiel werden, wenn der Typ Contains ist (dies ist der Standardwert für diese Optionen), Wildcards automatisch am Anfang und Ende des Suchschlüssels hinzugefügt, um sicherzustellen, dass die Übereinstimmung als "contains" geprüft wird. In diesem Fall werden die regulären Ausdrücke komplexer und die Leistung sinkt ebenfalls. Daher, aus Leistungsgründen, wenn der Benutzer die genaue Regel für das Regex angegeben hat, ist es nicht nötig, [`LookAtType`](../lookattype/) als zusätzliche Einschränkung zu verwenden, und der Benutzer kann es auf EntireContent setzen, um bessere Leistung zu erzielen.

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FindOptionsPropertyRegexKeyDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Testdaten mit Musterabgleich-Zeichenketten festlegen
            worksheet.Cells["A1"].PutValue("[hello]");
            worksheet.Cells["A2"].PutValue("Regular text");
            worksheet.Cells["A3"].PutValue("[another_example]");

            // Find-Optionen mit aktivierter Regex erstellen
            FindOptions options = new FindOptions();
            options.RegexKey = true;
            options.LookInType = LookInType.Values;
            options.LookAtType = LookAtType.Contains;

            // Zellen suchen, die dem Regex-Muster entsprechen
            string regEx = "\\[[a-zA-Z0-9_]+\\]";
            Cell foundCell = worksheet.Cells.Find(regEx, null, options);

            // Gib das Ergebnis aus
            if (foundCell != null)
            {
                Console.WriteLine("Found cell: " + foundCell.Name + " with value: " + foundCell.StringValue);
            }
            else
            {
                Console.WriteLine("No matching cells found");
            }
        }
    }
}
```

### Siehe auch

* class [FindOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


