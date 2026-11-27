---
title: "Worksheet.Replace"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Worksheet method. Ersätter all celltext med en ny sträng"
type: docs
url: /sv/net/aspose.cells/worksheet/replace/
---
## Worksheet.Replace method

Ersätter all celltext med en ny sträng.

```csharp
public int Replace(string oldString, string newString)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| oldString | String | Gammalt strängvärde. |
| newString | String | Nytt strängvärde. |

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodReplaceWithStringStringDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Kom åt första arbetsbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata i celler
            worksheet.Cells["A1"].PutValue("Hello World");
            worksheet.Cells["A2"].PutValue("Hello Aspose");
            worksheet.Cells["A3"].PutValue("Hello Cells");
            
            // Lägg till textbox med exempeltext
            worksheet.TextBoxes.Add(5, 0, 100, 50);
            worksheet.TextBoxes[0].Text = "Hello TextBox";
            
            // Ställ in sidhuvud och sidfot
            worksheet.PageSetup.SetHeader(0, "Hello Header");
            worksheet.PageSetup.SetFooter(0, "Hello Footer");
            
            // Ersätt "Hello" med "Hi" i allt innehåll
            string findText = "Hello";
            string replaceText = "Hi";
            worksheet.Replace(findText, replaceText);
            
            // Ersätt i sidhuvuden/sidfötter
            for (int i = 0; i < 3; i++)
            {
                if (worksheet.PageSetup.GetHeader(i) != null)
                    worksheet.PageSetup.SetHeader(i, worksheet.PageSetup.GetHeader(i).Replace(findText, replaceText));
                
                if (worksheet.PageSetup.GetFooter(i) != null)
                    worksheet.PageSetup.SetFooter(i, worksheet.PageSetup.GetFooter(i).Replace(findText, replaceText));
            }
            
            // Ersätt i textrutor
            foreach (Aspose.Cells.Drawing.TextBox textBox in worksheet.TextBoxes)
            {
                if (textBox.Text != null)
                {
                    textBox.Text = textBox.Text.Replace(findText, replaceText);
                }
            }
            
            // Spara arbetsboken
            workbook.Save("ReplaceDemo.xlsx");
        }
    }
}
```

### Se även

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


