---
title: "Name.RefersTo"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Name-Eigenschaft. Gibt die Formel zurück oder legt sie fest, auf die der Name definiert ist und die mit einem Gleichheitszeichen beginnt"
type: docs
url: /de/net/aspose.cells/name/refersto/
---
## Name.RefersTo property

Liest oder setzt die Formel, auf die der Name definiert ist, beginnend mit einem Gleichheitszeichen.

```csharp
public string RefersTo { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class NamePropertyRefersToDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Zugriff auf das erste Arbeitsblatt
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Name = "Sheet1";

            // Benannte Bereiche mit RefersTo hinzufügen
            int index1 = workbook.Worksheets.Names.Add("NamedRange1");
            workbook.Worksheets.Names[index1].RefersTo = "=Sheet1!$6:$8";
            
            int index2 = workbook.Worksheets.Names.Add("NamedRange2");
            workbook.Worksheets.Names[index2].RefersTo = "=Sheet1!$C:$D";

            // RefersTo-Eigenschaft benannter Bereiche anzeigen
            Console.WriteLine("NamedRange1 RefersTo: " + workbook.Worksheets.Names[0].RefersTo);
            Console.WriteLine("NamedRange2 RefersTo: " + workbook.Worksheets.Names[1].RefersTo);
        }
    }
}
```

### Siehe auch

* class [Name](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


