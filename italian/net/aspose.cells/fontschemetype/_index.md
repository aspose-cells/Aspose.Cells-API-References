---
title: "Enum FontSchemeType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Enum Aspose.Cells.FontSchemeType. Rappresenta il tipo di schema del carattere"
type: docs
url: /it/net/aspose.cells/fontschemetype/
---
## FontSchemeType enumeration

Rappresenta il tipo di schema del carattere.

```csharp
public enum FontSchemeType
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| None | `0` | Nessuno |
| Major | `1` | Schema principale. |
| Minor | `2` | Schema secondario. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class FontSchemeTypeDemo
    {
        public static void FontSchemeTypeExample()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            // Ottieni il riferimento del primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            // Accedere alla cella "A1" dal foglio di lavoro
            Cell cell = worksheet.Cells["A1"];
            // Aggiungere un valore alla cella "A1"
            cell.PutValue("Hello Aspose!");

            // Accedi al carattere dello stile della cella
            Aspose.Cells.Font font = cell.GetStyle().Font;

            // Impostazione del tipo di schema del carattere su Principale
            font.SchemeType = FontSchemeType.Major;

            // Impostazione di altre proprietà del carattere a scopo dimostrativo
            font.Name = "Arial";
            font.Size = 14;
            font.Color = System.Drawing.Color.Blue;

            // Salva la cartella di lavoro
            workbook.Save("FontSchemeTypeExample.xlsx");
            workbook.Save("FontSchemeTypeExample.pdf");
            return;
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


