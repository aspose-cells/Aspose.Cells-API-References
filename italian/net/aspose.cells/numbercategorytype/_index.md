---
title: "Enum NumberCategoryType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Aspose.Cells.NumberCategoryType enum. Rappresenta il tipo di categoria della formattazione numerica delle celle"
type: docs
url: /it/net/aspose.cells/numbercategorytype/
---
## NumberCategoryType enumeration

Rappresenta il tipo di categoria della formattazione numerica della cella.

```csharp
public enum NumberCategoryType
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| General | `0` | Generale |
| Text | `1` | Testo |
| Number | `2` | Numero |
| Date | `3` | Data o Data e ora |
| Time | `4` | Ora |
| Fraction | `5` | Frazione |
| Scientific | `6` | Scientifica |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class NumberCategoryTypeDemo
    {
        public static void NumberCategoryTypeExample()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();

            // Aggiungi un nuovo foglio di lavoro alla cartella di lavoro
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio al foglio di lavoro
            worksheet.Cells["A1"].PutValue("General");
            worksheet.Cells["A2"].PutValue("Text");
            worksheet.Cells["A3"].PutValue(12345);
            worksheet.Cells["A4"].PutValue(DateTime.Now);
            worksheet.Cells["A5"].PutValue(TimeSpan.FromHours(1.5));
            worksheet.Cells["A6"].PutValue(0.75);
            worksheet.Cells["A7"].PutValue(1.23E+3);

            // Imposta i formati numerici per le celle
            worksheet.Cells["A1"].SetStyle(CreateStyle(workbook, NumberCategoryType.General));
            worksheet.Cells["A2"].SetStyle(CreateStyle(workbook, NumberCategoryType.Text));
            worksheet.Cells["A3"].SetStyle(CreateStyle(workbook, NumberCategoryType.Number));
            worksheet.Cells["A4"].SetStyle(CreateStyle(workbook, NumberCategoryType.Date));
            worksheet.Cells["A5"].SetStyle(CreateStyle(workbook, NumberCategoryType.Time));
            worksheet.Cells["A6"].SetStyle(CreateStyle(workbook, NumberCategoryType.Fraction));
            worksheet.Cells["A7"].SetStyle(CreateStyle(workbook, NumberCategoryType.Scientific));

            // Restituisci i tipi di categoria numerica
            Console.WriteLine("Cell A1 Number Category Type: " + worksheet.Cells["A1"].NumberCategoryType);
            Console.WriteLine("Cell A2 Number Category Type: " + worksheet.Cells["A2"].NumberCategoryType);
            Console.WriteLine("Cell A3 Number Category Type: " + worksheet.Cells["A3"].NumberCategoryType);
            Console.WriteLine("Cell A4 Number Category Type: " + worksheet.Cells["A4"].NumberCategoryType);
            Console.WriteLine("Cell A5 Number Category Type: " + worksheet.Cells["A5"].NumberCategoryType);
            Console.WriteLine("Cell A6 Number Category Type: " + worksheet.Cells["A6"].NumberCategoryType);
            Console.WriteLine("Cell A7 Number Category Type: " + worksheet.Cells["A7"].NumberCategoryType);

            // Salva la cartella di lavoro
            workbook.Save("NumberCategoryTypeExample.xlsx");
        }

        private static Style CreateStyle(Workbook workbook, NumberCategoryType numberCategoryType)
        {
            Style style = workbook.CreateStyle();
            switch (numberCategoryType)
            {
                case NumberCategoryType.General:
                    style.Number = 0;
                    break;
                case NumberCategoryType.Text:
                    style.Number = 49;
                    break;
                case NumberCategoryType.Number:
                    style.Number = 1;
                    break;
                case NumberCategoryType.Date:
                    style.Number = 14;
                    break;
                case NumberCategoryType.Time:
                    style.Number = 21;
                    break;
                case NumberCategoryType.Fraction:
                    style.Number = 9;
                    break;
                case NumberCategoryType.Scientific:
                    style.Number = 11;
                    break;
            }
            return style;
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


