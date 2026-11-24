---
title: "Worksheet.Replace"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Worksheet-Methode. Ersetzt den Text aller Zellen durch einen neuen String"
type: docs
url: /de/net/aspose.cells/worksheet/replace/
---
## Worksheet.Replace method

Ersetzt den Text aller Zellen durch eine neue Zeichenfolge.

```csharp
public int Replace(string oldString, string newString)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| oldString | String | Alter String-Wert. |
| newString | String | Neuer String-Wert. |

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodReplaceWithStringStringDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Zugriff auf das erste Arbeitsblatt
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Füge Beispieldaten zu Zellen hinzu
            worksheet.Cells["A1"].PutValue("Hello World");
            worksheet.Cells["A2"].PutValue("Hello Aspose");
            worksheet.Cells["A3"].PutValue("Hello Cells");
            
            // Textbox mit Beispieltext hinzufügen
            worksheet.TextBoxes.Add(5, 0, 100, 50);
            worksheet.TextBoxes[0].Text = "Hello TextBox";
            
            // Kopf- und Fußzeile festlegen
            worksheet.PageSetup.SetHeader(0, "Hello Header");
            worksheet.PageSetup.SetFooter(0, "Hello Footer");
            
            // Ersetze "Hello" durch "Hi" im gesamten Inhalt
            string findText = "Hello";
            string replaceText = "Hi";
            worksheet.Replace(findText, replaceText);
            
            // Ersetzen in Kopf-/Fußzeilen
            for (int i = 0; i < 3; i++)
            {
                if (worksheet.PageSetup.GetHeader(i) != null)
                    worksheet.PageSetup.SetHeader(i, worksheet.PageSetup.GetHeader(i).Replace(findText, replaceText));
                
                if (worksheet.PageSetup.GetFooter(i) != null)
                    worksheet.PageSetup.SetFooter(i, worksheet.PageSetup.GetFooter(i).Replace(findText, replaceText));
            }
            
            // Ersetzen in Textboxen
            foreach (Aspose.Cells.Drawing.TextBox textBox in worksheet.TextBoxes)
            {
                if (textBox.Text != null)
                {
                    textBox.Text = textBox.Text.Replace(findText, replaceText);
                }
            }
            
            // Speichere die Arbeitsmappe
            workbook.Save("ReplaceDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


