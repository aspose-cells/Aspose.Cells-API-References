---
title: "ExternalLink.AddExternalName"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ExternalLink-Methode. Fügt einen externen Namen hinzu"
type: docs
url: /de/net/aspose.cells/externallink/addexternalname/
---
## ExternalLink.AddExternalName method

Fügt einen externen Namen hinzu.

```csharp
public void AddExternalName(string text, string referTo)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Text | String | Der Text des externen Namens. Wenn der externe Name zu einem Arbeitsblatt gehört, sollte der Text wie Sheet1!Text sein. |
| referTo | String | Der referTo des externen Namens. Er muss eine Zelle oder ein Bereich sein. |

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ExternalLinkMethodAddExternalNameWithStringStringDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Erstelle ein Beispiel für eine externe Arbeitsmappe
            Workbook externalWorkbook = new Workbook();
            Worksheet externalSheet = externalWorkbook.Worksheets[0];
            externalSheet.Cells["B2"].PutValue(67);
            
            // Füge einen externen Link zur Hauptarbeitsmappe hinzu
            string[] sheetNames = new string[] { externalSheet.Name };
            int index = workbook.Worksheets.ExternalLinks.Add("ExternalWorkbook.xlsx", sheetNames);
            ExternalLink externalLink = workbook.Worksheets.ExternalLinks[index];
            
            // Füge einen externen Namen hinzu
            externalLink.AddExternalName("Test", "=Sheet1!$B$2");
            
            // Verwende den externen Namen in einer Formel
            Worksheet sheet = workbook.Worksheets[0];
            sheet.Cells["A1"].Formula = "=[ExternalWorkbook.xlsx]!Test";
            
            // Formel berechnen
            workbook.CalculateFormula();
            
            // Gib das Ergebnis aus
            Console.WriteLine("Value from external reference: " + sheet.Cells["A1"].DoubleValue);
        }
    }
}
```

### Siehe auch

* class [ExternalLink](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


