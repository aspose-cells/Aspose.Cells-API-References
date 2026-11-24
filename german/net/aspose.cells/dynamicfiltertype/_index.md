---
title: "Aufzählung DynamicFilterType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.DynamicFilterType Aufzählung. Dynamischer Filtertyp"
type: docs
url: /de/net/aspose.cells/dynamicfiltertype/
---
## DynamicFilterType enumeration

Dynamischer Filtertyp.

```csharp
public enum DynamicFilterType
```

### Werte

| Name | Wert | Beschreibung |
| --- | --- | --- |
| AboveAverage | `0` | Zeigt Werte an, die über dem Durchschnitt liegen. |
| BelowAverage | `1` | Zeigt Werte an, die unter dem Durchschnitt liegen. |
| LastMonth | `2` | Zeigt die Daten des letzten Monats an. |
| LastQuarter | `3` | Zeigt die Daten des letzten Quartals an. |
| LastWeek | `4` | Zeigt die Daten der letzten Woche an. |
| LastYear | `5` | Zeigt die Daten des letzten Jahres an. |
| January | `6` | Zeigt die Daten an, die im Januar liegen, unabhängig vom Jahr. |
| October | `7` | Zeigt die Daten an, die im Oktober liegen, unabhängig vom Jahr. |
| November | `8` | Zeigt die Daten an, die im November liegen, unabhängig vom Jahr. |
| December | `9` | Zeigt die Daten an, die im Dezember liegen, unabhängig vom Jahr. |
| February | `10` | Zeigt die Daten an, die im Februar liegen, unabhängig vom Jahr. |
| March | `11` | Zeigt die Daten an, die im März liegen, unabhängig vom Jahr. |
| April | `12` | Zeigt die Daten an, die im April liegen, unabhängig vom Jahr. |
| May | `13` | Zeigt die Daten an, die im Mai liegen, unabhängig vom Jahr. |
| June | `14` | Zeigt die Daten an, die im Juni liegen, unabhängig vom Jahr. |
| July | `15` | Zeigt die Daten, die im Juli liegen, unabhängig vom Jahr. |
| August | `16` | Zeigt die Daten, die im August liegen, unabhängig vom Jahr. |
| September | `17` | Zeigt die Daten, die im September liegen, unabhängig vom Jahr. |
| NextMonth | `18` | Zeigt die Daten des nächsten Monats. |
| NextQuarter | `19` | Zeigt die Daten des nächsten Quartals. |
| NextWeek | `20` | Zeigt die Daten der nächsten Woche. |
| NextYear | `21` | Zeigt die Daten des nächsten Jahres. |
| None | `22` | Keine. |
| Quarter1 | `23` | Zeigt die Daten, die im 1. Quartal liegen, unabhängig vom Jahr. |
| Quarter2 | `24` | Zeigt die Daten, die im 2. Quartal liegen, unabhängig vom Jahr. |
| Quarter3 | `25` | Zeigt die Daten, die im 3. Quartal liegen, unabhängig vom Jahr. |
| Quarter4 | `26` | Zeigt die Daten, die im 4. Quartal liegen, unabhängig vom Jahr. |
| ThisMonth | `27` | Zeigt die Daten dieses Monats. |
| ThisQuarter | `28` | Zeigt die Daten dieses Quartals. |
| ThisWeek | `29` | Zeigt die Daten dieser Woche. |
| ThisYear | `30` | Zeigt die Daten dieses Jahres. |
| Today | `31` | Zeigt die Daten von heute. |
| Tomorrow | `32` | Zeigt die Daten von morgen. |
| YearToDate | `33` | Zeigt die Daten zwischen dem Beginn des Jahres und heute, inklusive. |
| Yesterday | `34` | Zeigt die Daten von gestern. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class DynamicFilterTypeDemo
    {
        public static void DynamicFilterTypeExample()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();

            // Ein neues Arbeitsblatt zur Arbeitsmappe hinzufügen
            Worksheet worksheet = workbook.Worksheets[0];

            // Beispieldaten zum Arbeitsblatt hinzufügen
            worksheet.Cells["A1"].PutValue("Date");
            worksheet.Cells["A2"].PutValue(new DateTime(2023, 1, 1));
            worksheet.Cells["A3"].PutValue(new DateTime(2023, 2, 1));
            worksheet.Cells["A4"].PutValue(new DateTime(2023, 3, 1));
            worksheet.Cells["A5"].PutValue(new DateTime(2023, 4, 1));
            worksheet.Cells["A6"].PutValue(new DateTime(2023, 5, 1));

            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);
            worksheet.Cells["B5"].PutValue(40);
            worksheet.Cells["B6"].PutValue(50);

            // Automatischen Filter auf das Arbeitsblatt anwenden
            worksheet.AutoFilter.SetRange(0, 0, 5);

            // Einen dynamischen Filter anwenden, um nur Daten im März anzuzeigen
            worksheet.AutoFilter.DynamicFilter(0, DynamicFilterType.March);

            // Speichere die Arbeitsmappe
            workbook.Save("DynamicFilterTypeExample.xlsx");
            workbook.Save("DynamicFilterTypeExample.pdf");

            // Ergebnisse ausgeben
            Console.WriteLine("Dynamic filter applied to show only dates in March.");
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


