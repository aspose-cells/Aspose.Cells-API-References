---
title: "Cell.IsCheckBoxStyle"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Zelleneigenschaft. Gibt an, ob diese Zelle als Kontrollkästchen festgelegt wird"
type: docs
url: /de/net/aspose.cells/cell/ischeckboxstyle/
---
## Cell.IsCheckBoxStyle property

Gibt an, ob diese Zelle als Kontrollkästchen festgelegt ist.

```csharp
public bool IsCheckBoxStyle { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellPropertyIsCheckBoxStyleDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Greife auf das erste Arbeitsblatt zu
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Zugriff auf Zelle B1 und Festlegung des Checkbox-Stils
            Cell cell = worksheet.Cells["B1"];
            cell.IsCheckBoxStyle = true;
            cell.PutValue(true);
            
            // Zugriff auf Zelle A1 und Festlegung des Checkbox-Stils mit einem Wert
            cell = worksheet.Cells["A1"];
            cell.IsCheckBoxStyle = true;
            cell.PutValue(false);
            
            // Speichere die Arbeitsmappe
            workbook.Save("CheckBoxStyleDemo.xlsx");
            
            // Laden der gespeicherten Arbeitsmappe, um Eigenschaften zu überprüfen
            Workbook loadedWorkbook = new Workbook("CheckBoxStyleDemo.xlsx");
            worksheet = loadedWorkbook.Worksheets[0];
            
            // Überprüfen, ob B1 den Checkbox-Stil hat
            cell = worksheet.Cells["B1"];
            Console.WriteLine("Cell B1 IsCheckBoxStyle: " + cell.IsCheckBoxStyle);
            
            // B1 in Nicht-Checkbox-Stil ändern und speichern
            cell.IsCheckBoxStyle = false;
            loadedWorkbook.Save("CheckBoxStyleDemo_Modified.xlsx");
        }
    }
}
```

### Siehe auch

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


