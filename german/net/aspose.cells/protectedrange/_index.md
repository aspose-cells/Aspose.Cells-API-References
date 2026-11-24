---
title: "Klasse ProtectedRange"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.ProtectedRange‑Klasse. Ein bestimmter Bereich, der bearbeitet werden darf, wenn der Blattschutz aktiviert ist."
type: docs
url: /de/net/aspose.cells/protectedrange/
---
## ProtectedRange class

Ein bestimmter Bereich, der bearbeitet werden darf, wenn der Blattschutz aktiviert ist.

```csharp
public class ProtectedRange
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [CellArea](../../aspose.cells/protectedrange/cellarea/) { get; } | Ruft das [`CellArea`](./cellarea/)‑Objekt ab, das den zu schützenden Zellbereich darstellt. |
| [IsProtectedWithPassword](../../aspose.cells/protectedrange/isprotectedwithpassword/) { get; } | Gibt an, ob das Arbeitsblatt mit einem Passwort geschützt ist. |
| [Name](../../aspose.cells/protectedrange/name/) { get; set; } | Ruft den Titel des Bereichs ab. Dieser wird als Bezeichner verwendet, nicht als Definition eines benannten Bereichs. |
| [Password](../../aspose.cells/protectedrange/password/) { get; set; } | Stellt das Passwort dar, um den Bereich zu schützen. |
| [SecurityDescriptor](../../aspose.cells/protectedrange/securitydescriptor/) { get; set; } | Der Sicherheitsdeskriptor definiert Benutzerkonten, die diesen Bereich bearbeiten dürfen, ohne ein Passwort zur Zugriffserlangung angeben zu müssen. |

## Methoden

| Name | Beschreibung |
| --- | --- |
| [AddArea](../../aspose.cells/protectedrange/addarea/)(int, int, int, int) | Fügt diesem einen referenzierten Bereich hinzu. |
| [GetAreas](../../aspose.cells/protectedrange/getareas/)() | Ruft alle referenzierten Bereiche ab. |

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassProtectedRangeDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Greife auf das erste Arbeitsblatt zu
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Abrufen Sie die Sammlung geschützter Bereiche
            ProtectedRangeCollection protectedRanges = worksheet.AllowEditRanges;
            
            // Fügen Sie einen neuen geschützten Bereich (A1:J10) hinzu
            int index = protectedRanges.Add("MyProtectedRange", 0, 0, 10, 10);
            
            // Abrufen Sie den geschützten Bereich
            ProtectedRange protectedRange = protectedRanges[index];
            
            // Setzen Sie den Sicherheitsdeskriptor fest
            string securityDescriptor = "O:WDG:WDD:(D;;CC;;;S-1-5-21-2854911246-2539335229-2923752399-1000)(A;;CC;;;S-1-5-21-2854911246-2539335229-2923752399-1013)";
            protectedRange.SecurityDescriptor = securityDescriptor;
            
            // Speichere die Arbeitsmappe
            workbook.Save("ProtectedRangeDemo.xlsx");
            
            Console.WriteLine("Protected range demo completed successfully.");
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


