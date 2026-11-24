---
title: "Validation.InCellDropDown"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Validierungseigenschaft. Gibt an, ob die Datenvalidierung eine Dropdown-Liste mit zulässigen Werten anzeigt"
type: docs
url: /de/net/aspose.cells/validation/incelldropdown/
---
## Validation.InCellDropDown property

Gibt an, ob die Datenvalidierung eine Dropdown-Liste anzeigt, die akzeptable Werte enthält.

```csharp
public bool InCellDropDown { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ValidationPropertyInCellDropDownDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Erstelle eine Validierung für Zelle A1
            Validation validation = worksheet.Cells["A1"].GetValidation();
            
            // Setze den Validierungstyp auf Liste mit Werten
            validation.Type = ValidationType.List;
            validation.Formula1 = "Option1,Option2,Option3";
            
            // Aktiviere In-Cell-Dropdown
            validation.InCellDropDown = true;

            // Erstelle eine weitere Validierung für Zelle B1 ohne Dropdown
            Validation validation2 = worksheet.Cells["B1"].GetValidation();
            validation2.Type = ValidationType.List;
            validation2.Formula1 = "Choice1,Choice2,Choice3";
            validation2.InCellDropDown = false;

            // Speichere die Arbeitsmappe
            workbook.Save("InCellDropDownDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Validation](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


