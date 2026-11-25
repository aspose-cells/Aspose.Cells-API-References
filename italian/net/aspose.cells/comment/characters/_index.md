---
title: "Comment.Characters"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Comment. Restituisce un oggetto Characters che rappresenta un intervallo di caratteri nel testo del commento"
type: docs
url: /it/net/aspose.cells/comment/characters/
---
## Comment.Characters method

Restituisce un oggetto Characters che rappresenta un intervallo di caratteri all'interno del testo del commento.

```csharp
public FontSetting Characters(int startIndex, int length)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| startIndex | Int32 | L'indice dell'inizio del carattere. |
| lunghezza | Int32 | Il numero di caratteri. |

### Valore di ritorno

Oggetto Characters.

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CommentMethodCharactersWithInt32Int32Demo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi un commento alla cella A1
            int commentIndex = worksheet.Comments.Add("A1");
            Comment comment1 = worksheet.Comments[commentIndex];
            comment1.Note = "This is a sample comment";
            
            // Ottieni l'impostazione del font per i primi 4 caratteri
            FontSetting fontSetting = comment1.Characters(0, 4);
            
            // Modifica le impostazioni del font
            fontSetting.Font.Color = System.Drawing.Color.Red;
            fontSetting.Font.IsBold = true;
            
            // Salva la cartella di lavoro
            workbook.Save("CommentFontSettingDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [FontSetting](../../fontsetting/)
* class [Comment](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


