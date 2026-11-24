---
title: "Name.R1C1RefersTo"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Name-Eigenschaft. Gibt eine R1C1-Referenz des Namens zurück oder legt sie fest"
type: docs
url: /de/net/aspose.cells/name/r1c1refersto/
---
## Name.R1C1RefersTo property

Gibt eine R1C1-Referenz des [`Name`](../) zurück oder legt sie fest.

```csharp
public string R1C1RefersTo { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class NamePropertyR1C1RefersToDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Fügen Sie einen neuen Namen zur Namenssammlung hinzu
            int nameIndex = workbook.Worksheets.Names.Add("TestRange");
            Name name = workbook.Worksheets.Names[nameIndex];
            
            // R1C1-Referenz für den Namen festlegen
            name.R1C1RefersTo = "'Sheet1'!R3C1:R9C4";
            
            // Überprüfen, ob die Referenz korrekt gesetzt wurde
            Console.WriteLine("Name refers to: " + name.RefersTo);
            
            // Speichere die Arbeitsmappe
            workbook.Save("NamePropertyR1C1RefersToDemo_Output.xlsx");
        }
    }
}
```

### Siehe auch

* class [Name](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


