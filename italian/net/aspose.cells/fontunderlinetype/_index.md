---
title: "Enum FontUnderlineType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Aspose.Cells.FontUnderlineType enum. Elenca i tipi di sottolineatura del carattere"
type: docs
url: /it/net/aspose.cells/fontunderlinetype/
---
## FontUnderlineType enumeration

Enumera i tipi di sottolineatura del carattere.

```csharp
public enum FontUnderlineType
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| None | `0` | Rappresenta nessuna sottolineatura. |
| Single | `1` | Rappresenta una singola sottolineatura. |
| Double | `2` | Rappresenta una doppia sottolineatura. |
| Accounting | `3` | Rappresenta una singola sottolineatura contabile. |
| DoubleAccounting | `4` | Rappresenta una doppia sottolineatura contabile. |
| Dash | `5` | Rappresenta una sottolineatura tratteggiata |
| DashDotDotHeavy | `6` | Rappresenta una sottolineatura spessa tratto-punto-punto |
| DashDotHeavy | `7` | Rappresenta una sottolineatura spessa tratto-punto |
| DashedHeavy | `8` | Rappresenta una sottolineatura spessa tratteggiata |
| DashLong | `9` | Rappresenta una sottolineatura lunga tratteggiata |
| DashLongHeavy | `10` | Rappresenta una sottolineatura spessa lunga tratteggiata |
| DotDash | `11` | Rappresenta una sottolineatura tratto-punto |
| DotDotDash | `12` | Rappresenta una sottolineatura tratto-punto-punto |
| Dotted | `13` | Rappresenta una sottolineatura puntinata |
| DottedHeavy | `14` | Rappresenta una sottolineatura spessa puntinata |
| Heavy | `15` | Rappresenta una sottolineatura spessa |
| Wave | `16` | Rappresenta la sottolineatura ondulata |
| WavyDouble | `17` | Rappresenta la doppia sottolineatura ondulata |
| WavyHeavy | `18` | Rappresenta la sottolineatura ondulata pesante |
| Words | `19` | Rappresenta la sottolineatura dei caratteri non spazi. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class FontUnderlineTypeDemo
    {
        public static void FontUnderlineTypeExample()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Ottieni il riferimento del primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Accedere alla cella "A1" dal foglio di lavoro
            Cell cell = worksheet.Cells["A1"];
            
            // Aggiungere un valore alla cella "A1"
            cell.PutValue("Hello Aspose!");

            // Ottieni lo stile della cella
            Style style = cell.GetStyle();
            
            // Imposta il tipo di sottolineatura del carattere su singola sottolineatura
            style.Font.Underline = FontUnderlineType.Single;
            
            // Applica lo stile alla cella
            cell.SetStyle(style);

            // Salva la cartella di lavoro
            workbook.Save("FontUnderlineTypeExample.xlsx");
            workbook.Save("FontUnderlineTypeExample.pdf");
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


