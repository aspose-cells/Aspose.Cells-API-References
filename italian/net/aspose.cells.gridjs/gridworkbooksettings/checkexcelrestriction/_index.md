---
title: "GridWorkbookSettings.CheckExcelRestriction"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà GridWorkbookSettings. Indica se verificare le restrizioni del file Excel quando l'utente modifica oggetti correlati alle celle. Ad esempio, Excel non consente l'inserimento di una stringa più lunga di 32K. Quando si inserisce un valore più lungo di 32K, ad esempio tramite Cell.PutValuestring, se questa proprietà è true si otterrà un'eccezione. Se la proprietà è false accetteremo la stringa inserita come valore della cella, così in seguito potrai esportare la stringa completa per altri formati di file come CSV. Tuttavia, se hai impostato un valore di questo tipo non valido per il formato Excel, non dovresti salvare la cartella di lavoro come file Excel in seguito. Altrimenti potrebbero verificarsi errori imprevisti nel file Excel generato. Il valore predefinito è false"
type: docs
url: /it/net/aspose.cells.gridjs/gridworkbooksettings/checkexcelrestriction/
---
## GridWorkbookSettings.CheckExcelRestriction property

Indica se verificare le restrizioni del file Excel quando l'utente modifica oggetti correlati alle celle. Ad esempio, Excel non consente l'inserimento di una stringa più lunga di 32K. Quando si inserisce un valore più lungo di 32K, ad esempio con Cell.PutValue(string), se questa proprietà è true, verrà generata un'eccezione. Se la proprietà è false, accetteremo la stringa inserita come valore della cella, così in seguito potrai esportare la stringa completa per altri formati di file come CSV. Tuttavia, se hai impostato un valore di questo tipo non valido per il formato file Excel, non dovresti salvare la cartella di lavoro in formato Excel in seguito. Altrimenti potrebbero verificarsi errori inattesi nel file Excel generato. Il valore predefinito è false.

```csharp
public bool CheckExcelRestriction { get; set; }
```

### Vedi anche

* class [GridWorkbookSettings](../)
* namespace [Aspose.Cells.GridJs](../../../aspose.cells.gridjs/)
* assembly [Aspose.Cells.GridJs](../../../)


