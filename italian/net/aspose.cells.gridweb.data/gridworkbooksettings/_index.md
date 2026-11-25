---
title: "Classe GridWorkbookSettings"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.GridWeb.Data.GridWorkbookSettings. Rappresenta le impostazioni della cartella di lavoro"
type: docs
url: /it/net/aspose.cells.gridweb.data/gridworkbooksettings/
---
## GridWorkbookSettings class

Rappresenta le impostazioni della cartella di lavoro.

```csharp
public class GridWorkbookSettings : ISerializable
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [GridWorkbookSettings](gridworkbooksettings/)() | costruttore predefinito |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [Author](../../aspose.cells.gridweb.data/gridworkbooksettings/author/) { get; set; } | Ottiene e imposta l'autore del file. |
| [CheckCustomNumberFormat](../../aspose.cells.gridweb.data/gridworkbooksettings/checkcustomnumberformat/) { get; set; } | Ottiene o imposta se verificare il formato numerico personalizzato quando si imposta Style.Custom. |
| [CreateCalcChain](../../aspose.cells.gridweb.data/gridworkbooksettings/createcalcchain/) { get; set; } | Ottiene o imposta se creare una catena di formule calcolate. Il valore predefinito è false. |
| [Date1904](../../aspose.cells.gridweb.data/gridworkbooksettings/date1904/) { get; set; } | Ottiene o imposta il valore che indica se la cartella di lavoro utilizza il sistema di data 1904. |
| [EnableMacros](../../aspose.cells.gridweb.data/gridworkbooksettings/enablemacros/) { get; set; } | Ottiene o imposta se abilitare le macro; ora funziona solo quando si copia un foglio di lavoro in un altro foglio all'interno di una cartella di lavoro. |
| [ForceFullCalculate](../../aspose.cells.gridweb.data/gridworkbooksettings/forcefullcalculate/) { get; set; } | Ottiene o imposta se calcolare completamente ogni volta che viene avviato un calcolo. |
| [Iteration](../../aspose.cells.gridweb.data/gridworkbooksettings/iteration/) { get; set; } | Ottiene o imposta se utilizzare l'iterazione per risolvere riferimenti circolari. |
| [MaxIteration](../../aspose.cells.gridweb.data/gridworkbooksettings/maxiteration/) { get; set; } | Ottiene o imposta il numero massimo di iterazioni per risolvere un riferimento circolare; il valore predefinito è 100. |
| [PrecisionAsDisplayed](../../aspose.cells.gridweb.data/gridworkbooksettings/precisionasdisplayed/) { get; set; } | True se i calcoli in questa cartella di lavoro verranno eseguiti utilizzando solo la precisione dei numeri così come sono visualizzati |
| [PreservePaddingSpaces](../../aspose.cells.gridweb.data/gridworkbooksettings/preservepaddingspaces/) { get; set; } | Indica se preservare quegli spazi e interruzioni di riga inseriti tra i token della formula durante l'ottenimento e l'impostazione delle formule. Il valore predefinito è false. |
| [ReCalculateOnOpen](../../aspose.cells.gridweb.data/gridworkbooksettings/recalculateonopen/) { get; set; } | Ottiene o imposta se ricalcolare tutte le formule all'apertura del file. |

### Esempi

```csharp
[C#]

 
GridWeb gridweb = new GridWeb();
GridWorkbookSettings gsettings = new GridWorkbookSettings();
gridweb.Settings=gsettings;

//esegui la tua attività

[Visual Basic]


Dim gsettings as GridWorkbookSettings = new GridWorkbookSettings()
 gridweb.Settings=gsettings;
 
'do your business
```

### Vedi anche

* namespace [Aspose.Cells.GridWeb.Data](../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../)


