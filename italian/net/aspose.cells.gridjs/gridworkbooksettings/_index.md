---
title: "Classe GridWorkbookSettings"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Aspose.Cells.GridJs.GridWorkbookSettings class. Rappresenta le impostazioni della cartella di lavoro"
type: docs
url: /it/net/aspose.cells.gridjs/gridworkbooksettings/
---
## GridWorkbookSettings class

Rappresenta le impostazioni della cartella di lavoro.

```csharp
public class GridWorkbookSettings
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [GridWorkbookSettings](gridworkbooksettings/)() | Il costruttore predefinito. |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [Author](../../aspose.cells.gridjs/gridworkbooksettings/author/) { get; set; } | Ottiene/imposta l'autore del file. |
| [CheckCustomNumberFormat](../../aspose.cells.gridjs/gridworkbooksettings/checkcustomnumberformat/) { get; set; } | Indica se verificare il formato numerico personalizzato quando si imposta Style.Custom, il valore predefinito è false. |
| [CheckExcelRestriction](../../aspose.cells.gridjs/gridworkbooksettings/checkexcelrestriction/) { get; set; } | Indica se verificare le restrizioni del file Excel quando l'utente modifica oggetti correlati alle celle. Ad esempio, Excel non consente l'inserimento di una stringa più lunga di 32K. Quando si inserisce un valore più lungo di 32K, ad esempio con Cell.PutValue(string), se questa proprietà è true, verrà generata un'eccezione. Se la proprietà è false, accetteremo la stringa inserita come valore della cella, così in seguito potrai esportare la stringa completa per altri formati di file come CSV. Tuttavia, se hai impostato un valore di questo tipo non valido per il formato file Excel, non dovresti salvare la cartella di lavoro in formato Excel in seguito. Altrimenti potrebbero verificarsi errori inattesi nel file Excel generato. Il valore predefinito è false. |
| [CreateCalcChain](../../aspose.cells.gridjs/gridworkbooksettings/createcalcchain/) { get; set; } | Indica se creare la catena di formule calcolate. Il valore predefinito è false. |
| [Date1904](../../aspose.cells.gridjs/gridworkbooksettings/date1904/) { get; set; } | Ottiene o imposta un valore che indica se la workbook utilizza il sistema di data 1904. |
| [EnableMacros](../../aspose.cells.gridjs/gridworkbooksettings/enablemacros/) { get; set; } | Abilita le macro; ora funziona solo quando si copia un foglio di lavoro in un altro foglio all'interno di una cartella di lavoro. |
| [ForceFullCalculate](../../aspose.cells.gridjs/gridworkbooksettings/forcefullcalculate/) { get; set; } | Indica se eseguire il calcolo completo ogni volta che viene avviato un calcolo. |
| [Iteration](../../aspose.cells.gridjs/gridworkbooksettings/iteration/) { get; set; } | Indica se utilizzare l'iterazione per risolvere riferimenti circolari. |
| [MaxIteration](../../aspose.cells.gridjs/gridworkbooksettings/maxiteration/) { get; set; } | Restituisce o imposta il numero massimo di iterazioni per risolvere un riferimento circolare, il valore predefinito è 100. |
| [PrecisionAsDisplayed](../../aspose.cells.gridjs/gridworkbooksettings/precisionasdisplayed/) { get; set; } | True se i calcoli in questa cartella di lavoro verranno eseguiti utilizzando solo la precisione dei numeri così come sono visualizzati |
| [ReCalculateOnOpen](../../aspose.cells.gridjs/gridworkbooksettings/recalculateonopen/) { get; set; } | Indica se ricalcolare tutte le formule all'apertura del file. Il valore predefinito è true. |

### Esempi

```csharp
[C#]

GridJsWorkbook g = new GridJsWorkbook();

GridWorkbookSettings gsettings = new GridWorkbookSettings();
g.Settings=gsettings;

//esegui la tua attività

[Visual Basic]
Dim g as GridJsWorkbook = new GridJsWorkbook()

Dim gsettings as GridWorkbookSettings = new GridWorkbookSettings()
 g.Settings=gsettings;
 
'do your business
```

### Vedi anche

* namespace [Aspose.Cells.GridJs](../../aspose.cells.gridjs/)
* assembly [Aspose.Cells.GridJs](../../)


