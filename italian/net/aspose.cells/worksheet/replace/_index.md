---
title: "Worksheet.Replace"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Worksheet method. Sostituisce tutto il testo delle celle con una nuova stringa"
type: docs
url: /it/net/aspose.cells/worksheet/replace/
---
## Worksheet.Replace method

Sostituisce il testo di tutte le celle con una nuova stringa.

```csharp
public int Replace(string oldString, string newString)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| oldString | String | Valore della vecchia stringa. |
| newString | String | Valore della nuova stringa. |

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodReplaceWithStringStringDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi dati di esempio alle celle
            worksheet.Cells["A1"].PutValue("Hello World");
            worksheet.Cells["A2"].PutValue("Hello Aspose");
            worksheet.Cells["A3"].PutValue("Hello Cells");
            
            // Aggiungi una casella di testo con testo di esempio
            worksheet.TextBoxes.Add(5, 0, 100, 50);
            worksheet.TextBoxes[0].Text = "Hello TextBox";
            
            // Imposta intestazione e piè di pagina
            worksheet.PageSetup.SetHeader(0, "Hello Header");
            worksheet.PageSetup.SetFooter(0, "Hello Footer");
            
            // Sostituisci "Hello" con "Hi" in tutto il contenuto
            string findText = "Hello";
            string replaceText = "Hi";
            worksheet.Replace(findText, replaceText);
            
            // Sostituisci nelle intestazioni/piè di pagina
            for (int i = 0; i < 3; i++)
            {
                if (worksheet.PageSetup.GetHeader(i) != null)
                    worksheet.PageSetup.SetHeader(i, worksheet.PageSetup.GetHeader(i).Replace(findText, replaceText));
                
                if (worksheet.PageSetup.GetFooter(i) != null)
                    worksheet.PageSetup.SetFooter(i, worksheet.PageSetup.GetFooter(i).Replace(findText, replaceText));
            }
            
            // Sostituisci nelle caselle di testo
            foreach (Aspose.Cells.Drawing.TextBox textBox in worksheet.TextBoxes)
            {
                if (textBox.Text != null)
                {
                    textBox.Text = textBox.Text.Replace(findText, replaceText);
                }
            }
            
            // Salva la cartella di lavoro
            workbook.Save("ReplaceDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


