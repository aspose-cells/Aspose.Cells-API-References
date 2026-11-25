---
title: "Classe AutoFilter"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.AutoFilter. Rappresenta il filtro automatico per il foglio di lavoro specificato"
type: docs
url: /it/net/aspose.cells/autofilter/
---
## AutoFilter class

Rappresenta l'autofiltro per il foglio di lavoro specificato.

```csharp
public class AutoFilter
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [FilterColumns](../../aspose.cells/autofilter/filtercolumns/) { get; } | Ottiene la raccolta delle colonne filtro. |
| [Range](../../aspose.cells/autofilter/range/) { get; set; } | Rappresenta l'intervallo a cui si applica l'AutoFilter specificato. |
| [ShowFilterButton](../../aspose.cells/autofilter/showfilterbutton/) { get; set; } | Indica se il pulsante AutoFilter per questa colonna è visibile. |
| [Sorter](../../aspose.cells/autofilter/sorter/) { get; } | Ottiene l'ordinatore dei dati. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [AddDateFilter](../../aspose.cells/autofilter/adddatefilter/)(int, DateTimeGroupingType, int, int, int, int, int, int) | Aggiunge un filtro data. |
| [AddFillColorFilter](../../aspose.cells/autofilter/addfillcolorfilter/)(int, BackgroundType, CellsColor, CellsColor) | Aggiunge un filtro di colore di riempimento. |
| [AddFilter](../../aspose.cells/autofilter/addfilter/)(int, string) | Aggiunge un filtro per una colonna filtro. |
| [AddFontColorFilter](../../aspose.cells/autofilter/addfontcolorfilter/)(int, CellsColor) | Aggiunge un filtro di colore del carattere. |
| [AddIconFilter](../../aspose.cells/autofilter/addiconfilter/)(int, IconSetType, int) | Aggiunge un filtro icona. |
| [Custom](../../aspose.cells/autofilter/custom/#custom)(int, FilterOperatorType, object) | Filtra un elenco con un criterio personalizzato. |
| [Custom](../../aspose.cells/autofilter/custom/#custom_1)(int, FilterOperatorType, object, bool, FilterOperatorType, object) | Filtra un elenco con criteri personalizzati. |
| [DynamicFilter](../../aspose.cells/autofilter/dynamicfilter/)(int, DynamicFilterType) | Aggiunge un filtro dinamico. |
| [Filter](../../aspose.cells/autofilter/filter/)(int, string) | Filtra un elenco con criteri specificati. |
| [FilterTop10](../../aspose.cells/autofilter/filtertop10/)(int, bool, bool, int) | Filtra i primi 10 elementi dell'elenco |
| [GetCellArea](../../aspose.cells/autofilter/getcellarea/#getcellarea)() | Ottiene il [`CellArea`](../cellarea/) dove questo AutoFilter si applica. |
| [GetCellArea](../../aspose.cells/autofilter/getcellarea/#getcellarea_1)(bool) | Ottiene il [`CellArea`](../cellarea/) dove si applica l'AutoFilter specificato. |
| [MatchBlanks](../../aspose.cells/autofilter/matchblanks/)(int) | Corrisponde a tutte le celle vuote nell'elenco. |
| [MatchNonBlanks](../../aspose.cells/autofilter/matchnonblanks/)(int) | Corrisponde a tutte le celle non vuote nell'elenco. |
| [Refresh](../../aspose.cells/autofilter/refresh/#refresh)() | Aggiorna i filtri automatici per nascondere o mostrare le righe. |
| [Refresh](../../aspose.cells/autofilter/refresh/#refresh_1)(bool) | Ottiene gli indici di tutte le righe nascoste. |
| [RemoveDateFilter](../../aspose.cells/autofilter/removedatefilter/)(int, DateTimeGroupingType, int, int, int, int, int, int) | Rimuove un filtro data. |
| [RemoveFilter](../../aspose.cells/autofilter/removefilter/#removefilter)(int) | Rimuove il filtro specifico. |
| [RemoveFilter](../../aspose.cells/autofilter/removefilter/#removefilter_1)(int, string) | Rimuove un filtro per una colonna filtro. |
| [SetRange](../../aspose.cells/autofilter/setrange/)(int, int, int) | Imposta l'intervallo a cui si applica l'AutoFiltro specificato. |
| [ShowAll](../../aspose.cells/autofilter/showall/)() | Mostra tutte le righe. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class AutoFilterDemo
    {
        public static void AutoFilterExample()
        {
            // Creazione di un flusso file contenente il file Excel da aprire
            // Istanziare un oggetto Workbook
            Workbook workbook = new Workbook("AutoFilterExampleTemplate.xlsx");
            // Accesso al primo foglio di lavoro nel file Excel
            Worksheet worksheet = workbook.Worksheets[0];
            // Creazione dell'AutoFiltro fornendo l'intervallo di celle della riga di intestazione
            worksheet.AutoFilter.Range = "A1:B8";
            // Filtraggio delle colonne con i valori specificati
            worksheet.AutoFilter.Filter(0, "Bananas");
            worksheet.AutoFilter.Refresh();

            // Salvataggio del file Excel modificato.
            workbook.Save("AutoFilterExample.xlsx");
            workbook.Save("AutoFilterExample.pdf");

            // Istanziare un oggetto Workbook
            workbook = new Workbook("AutoFilterExampleTemplate.xlsx");
            // Accesso al primo foglio di lavoro nel file Excel
            worksheet = workbook.Worksheets[0];

            // Codice aggiuntivo per dimostrare altre funzionalità dell'AutoFiltro
            // Impostazione dell'intervallo per l'AutoFiltro
            worksheet.AutoFilter.Range = "A1:B8";
            // Aggiunta di un filtro
            worksheet.AutoFilter.AddFilter(0, "Apples");
            // Aggiunta di un filtro data
            worksheet.AutoFilter.AddDateFilter(1, DateTimeGroupingType.Year, 2022, 0, 0, 0, 0, 0);

            worksheet.AutoFilter.Refresh();
            // Salvataggio del file Excel modificato.
            workbook.Save("AutoFilterExample2.xlsx");
            workbook.Save("AutoFilterExample2.pdf");

            // Istanziare un oggetto Workbook
            workbook = new Workbook("AutoFilterExampleTemplate.xlsx");
            // Accesso al primo foglio di lavoro nel file Excel
            worksheet = workbook.Worksheets[0];
                        
            // Aggiunta di un filtro colore carattere
            CellsColor color = workbook.CreateCellsColor();
            color.Color = System.Drawing.Color.Red;

            worksheet.AutoFilter.AddFontColorFilter(0, color);

            worksheet.AutoFilter.Refresh();
            // Salvataggio del file Excel modificato.
            workbook.Save("AutoFilterExample3.xlsx");
            workbook.Save("AutoFilterExample3.pdf");

            // Istanziare un oggetto Workbook
            workbook = new Workbook("AutoFilterExampleTemplate.xlsx");
            // Accesso al primo foglio di lavoro nel file Excel
            worksheet = workbook.Worksheets[0];

            // Aggiunta di un filtro colore riempimento
            CellsColor foregroundColor = workbook.CreateCellsColor();
            foregroundColor.Color = System.Drawing.Color.Red;
            CellsColor backgroundColor = workbook.CreateCellsColor();
            backgroundColor.Color = System.Drawing.Color.White;

            worksheet.AutoFilter.AddFillColorFilter(0, BackgroundType.Solid, foregroundColor, backgroundColor);

            worksheet.AutoFilter.Refresh();
            // Salvataggio del file Excel modificato.
            workbook.Save("AutoFilterExample4.xlsx");
            workbook.Save("AutoFilterExample4.pdf");

            // Istanziare un oggetto Workbook
            workbook = new Workbook("AutoFilterExampleTemplate.xlsx");
            // Accesso al primo foglio di lavoro nel file Excel
            worksheet = workbook.Worksheets[0];

            // Corrispondenza di celle vuote
            worksheet.AutoFilter.MatchBlanks(0);

            worksheet.AutoFilter.Refresh();
            // Salvataggio del file Excel modificato.
            workbook.Save("AutoFilterExample5.xlsx");
            workbook.Save("AutoFilterExample5.pdf");

            // Istanziare un oggetto Workbook
            workbook = new Workbook("AutoFilterExampleTemplate.xlsx");
            // Accesso al primo foglio di lavoro nel file Excel
            worksheet = workbook.Worksheets[0];

            // Corrispondenza di celle non vuote
            worksheet.AutoFilter.MatchNonBlanks(0);

            worksheet.AutoFilter.Refresh();
            // Salvataggio del file Excel modificato.
            workbook.Save("AutoFilterExample6.xlsx");
            workbook.Save("AutoFilterExample6.pdf");

            // Istanziare un oggetto Workbook
            workbook = new Workbook("AutoFilterExampleTemplate.xlsx");
            // Accesso al primo foglio di lavoro nel file Excel
            worksheet = workbook.Worksheets[0];

            // Filtro personalizzato
            worksheet.AutoFilter.Custom(0, FilterOperatorType.Contains, "Test");

            worksheet.AutoFilter.Refresh();
            // Salvataggio del file Excel modificato.
            workbook.Save("AutoFilterExample7.xlsx");
            workbook.Save("AutoFilterExample7.pdf");
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


