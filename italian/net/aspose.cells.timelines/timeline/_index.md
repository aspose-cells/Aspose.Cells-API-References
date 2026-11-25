---
title: "Classe Timeline"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.Timelines.Timeline. Descrizione sommaria della Vista Timeline. Poiché MS Excel 2003 non supporta Timeline"
type: docs
url: /it/net/aspose.cells.timelines/timeline/
---
## Timeline class

Descrizione sommaria della visualizzazione della linea temporale. A causa di MS Excel, Excel 2003 non supporta le linee temporali

```csharp
public class Timeline
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [Caption](../../aspose.cells.timelines/timeline/caption/) { get; set; } | Ottiene o imposta la didascalia di questa Timeline. |
| [CurrentLevel](../../aspose.cells.timelines/timeline/currentlevel/) { get; set; } | Il livello temporale corrente della Timeline. |
| [HeightPixel](../../aspose.cells.timelines/timeline/heightpixel/) { get; set; } | (**Obsolete.**) Restituisce o imposta l'altezza della timeline specificata, in pixel. |
| [LeftPixel](../../aspose.cells.timelines/timeline/leftpixel/) { get; set; } | (**Obsolete.**) Restituisce o imposta lo spostamento orizzontale della forma della timeline dalla sua colonna sinistra, in pixel. |
| [Name](../../aspose.cells.timelines/timeline/name/) { get; set; } | Restituisce o imposta il nome della Timeline specificata |
| [SelectionLevel](../../aspose.cells.timelines/timeline/selectionlevel/) { get; set; } | Ottiene e imposta il livello temporale al quale è stata effettuata la selezione corrente per la Timeline. |
| [Shape](../../aspose.cells.timelines/timeline/shape/) { get; } | Restituisce l'oggetto [`TimelineShape`](../../aspose.cells.drawing/timelineshape/) associato a questa Timeline. |
| [ShowHeader](../../aspose.cells.timelines/timeline/showheader/) { get; set; } | Indica se visualizzare l'intestazione di questa timeline. |
| [ShowHorizontalScrollbar](../../aspose.cells.timelines/timeline/showhorizontalscrollbar/) { get; set; } | Indica se visualizzare la barra di scorrimento orizzontale. |
| [ShowSelectionLabel](../../aspose.cells.timelines/timeline/showselectionlabel/) { get; set; } | Indica se visualizzare l'etichetta di selezione. |
| [ShowTimeLevel](../../aspose.cells.timelines/timeline/showtimelevel/) { get; set; } | Indica se visualizzare la casella a discesa di selezione del livello temporale. |
| [StartDate](../../aspose.cells.timelines/timeline/startdate/) { get; set; } | Ottiene e imposta la data di inizio della posizione di scorrimento dell'intervallo di tempo di questo `Timeline`. |
| [TopPixel](../../aspose.cells.timelines/timeline/toppixel/) { get; set; } | (**Obsolete.**) Restituisce o imposta lo spostamento verticale della forma della timeline dalla sua riga superiore, in pixel. |
| [WidthPixel](../../aspose.cells.timelines/timeline/widthpixel/) { get; set; } | (**Obsolete.**) Restituisce o imposta la larghezza della timeline specificata, in pixel. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [GetSelectedDateTimeRange](../../aspose.cells.timelines/timeline/getselecteddatetimerange/)() | Ottiene l'intervallo selezionato di data e ora. |
| [Select](../../aspose.cells.timelines/timeline/select/)(DateTime, DateTime, bool) | Seleziona l'elemento tra le date e le ore. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using Aspose.Cells.Timelines;
    using System;

    public class TimelineDemo
    {
        public static void TimelineExample()
        {
            // Crea una nuova cartella di lavoro e ottieni il primo foglio di lavoro
            Workbook book = new Workbook();
            Worksheet sheet = book.Worksheets[0];
            Cells cells = sheet.Cells;

            // Popola il foglio di lavoro con dati di esempio
            cells[0, 0].Value = "fruit";
            cells[1, 0].Value = "grape";
            cells[2, 0].Value = "blueberry";
            cells[3, 0].Value = "kiwi";
            cells[4, 0].Value = "cherry";

            // Crea lo stile data
            Style dateStyle = new CellsFactory().CreateStyle();
            dateStyle.Custom = "m/d/yyyy";
            cells[0, 1].Value = "date";
            cells[1, 1].Value = new DateTime(2021, 2, 5);
            cells[2, 1].Value = new DateTime(2022, 3, 8);
            cells[3, 1].Value = new DateTime(2023, 4, 10);
            cells[4, 1].Value = new DateTime(2024, 5, 16);
            // Imposta lo stile data
            cells[1, 1].SetStyle(dateStyle);
            cells[2, 1].SetStyle(dateStyle);
            cells[3, 1].SetStyle(dateStyle);
            cells[4, 1].SetStyle(dateStyle);

            cells[0, 2].Value = "amount";
            cells[1, 2].Value = 50;
            cells[2, 2].Value = 60;
            cells[3, 2].Value = 70;
            cells[4, 2].Value = 80;

            // Aggiungi una PivotTable
            PivotTableCollection pivots = sheet.PivotTables;
            int pivotIndex = pivots.Add("=Sheet1!A1:C5", "A12", "TestPivotTable");
            PivotTable pivot = pivots[pivotIndex];
            pivot.AddFieldToArea(PivotFieldType.Row, "fruit");
            pivot.AddFieldToArea(PivotFieldType.Column, "date");
            pivot.AddFieldToArea(PivotFieldType.Data, "amount");
            pivot.PivotTableStyleType = PivotTableStyleType.PivotTableStyleMedium10;

            // Aggiorna i dati della PivotTable
            pivot.RefreshData();
            pivot.CalculateData();

            // Aggiungi una nuova Timeline utilizzando la PivotTable come origine dati
            sheet.Timelines.Add(pivot, 10, 5, "date");

            // Ottieni l'oggetto Timeline
            Timeline timelineObj = sheet.Timelines[0];

            // Imposta le proprietà della Timeline
            timelineObj.Caption = "timeline caption test";
            timelineObj.Name = "timeline name test";
            timelineObj.LeftPixel = 100;
            timelineObj.TopPixel = 50;
            timelineObj.WidthPixel = 300;
            timelineObj.HeightPixel = 100;

            // Salva la cartella di lavoro
            book.Save("TimelineExample.xlsx");
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells.Timelines](../../aspose.cells.timelines/)
* assembly [Aspose.Cells](../../)


