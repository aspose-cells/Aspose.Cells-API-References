---
title: "Enum DynamicFilterType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Aspose.Cells.DynamicFilterType enum. Tipo di filtro dinamico"
type: docs
url: /it/net/aspose.cells/dynamicfiltertype/
---
## DynamicFilterType enumeration

Tipo di filtro dinamico.

```csharp
public enum DynamicFilterType
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| AboveAverage | `0` | Mostra i valori sopra la media. |
| BelowAverage | `1` | Mostra i valori sotto la media. |
| LastMonth | `2` | Mostra le date del mese scorso. |
| LastQuarter | `3` | Mostra le date dell'ultimo trimestre. |
| LastWeek | `4` | Mostra le date della scorsa settimana. |
| LastYear | `5` | Mostra le date dell'anno scorso. |
| January | `6` | Mostra le date di gennaio, indipendentemente dall'anno. |
| October | `7` | Mostra le date che sono in ottobre, indipendentemente dall'anno. |
| November | `8` | Mostra le date che sono in novembre, indipendentemente dall'anno. |
| December | `9` | Mostra le date che sono in dicembre, indipendentemente dall'anno. |
| February | `10` | Mostra le date che sono in febbraio, indipendentemente dall'anno. |
| March | `11` | Mostra le date che sono in marzo, indipendentemente dall'anno. |
| April | `12` | Mostra le date che sono in aprile, indipendentemente dall'anno. |
| May | `13` | Mostra le date che sono in maggio, indipendentemente dall'anno. |
| June | `14` | Mostra le date che sono in giugno, indipendentemente dall'anno. |
| July | `15` | Mostra le date che sono in luglio, indipendentemente dall'anno. |
| August | `16` | Mostra le date che sono in agosto, indipendentemente dall'anno. |
| September | `17` | Mostra le date che sono in settembre, indipendentemente dall'anno. |
| NextMonth | `18` | Mostra le date del prossimo mese. |
| NextQuarter | `19` | Mostra le date del prossimo trimestre. |
| NextWeek | `20` | Mostra le date della prossima settimana. |
| NextYear | `21` | Mostra le date del prossimo anno. |
| None | `22` | Nessuno. |
| Quarter1 | `23` | Mostra le date che sono nel 1° trimestre, indipendentemente dall'anno. |
| Quarter2 | `24` | Mostra le date che sono nel 2° trimestre, indipendentemente dall'anno. |
| Quarter3 | `25` | Mostra le date che sono nel 3° trimestre, indipendentemente dall'anno. |
| Quarter4 | `26` | Mostra le date che sono nel 4° trimestre, indipendentemente dall'anno. |
| ThisMonth | `27` | Mostra le date di questo mese. |
| ThisQuarter | `28` | Mostra le date di questo trimestre. |
| ThisWeek | `29` | Mostra le date di questa settimana. |
| ThisYear | `30` | Mostra le date di quest'anno. |
| Today | `31` | Mostra le date di oggi. |
| Tomorrow | `32` | Mostra le date di domani. |
| YearToDate | `33` | Mostra le date tra l'inizio dell'anno e oggi, inclusi. |
| Yesterday | `34` | Mostra le date di ieri. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class DynamicFilterTypeDemo
    {
        public static void DynamicFilterTypeExample()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();

            // Aggiungi un nuovo foglio di lavoro alla cartella di lavoro
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio al foglio di lavoro
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

            // Applica il filtro automatico al foglio di lavoro
            worksheet.AutoFilter.SetRange(0, 0, 5);

            // Applica un filtro dinamico per mostrare solo le date di marzo
            worksheet.AutoFilter.DynamicFilter(0, DynamicFilterType.March);

            // Salva la cartella di lavoro
            workbook.Save("DynamicFilterTypeExample.xlsx");
            workbook.Save("DynamicFilterTypeExample.pdf");

            // Restituisci i risultati
            Console.WriteLine("Dynamic filter applied to show only dates in March.");
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


