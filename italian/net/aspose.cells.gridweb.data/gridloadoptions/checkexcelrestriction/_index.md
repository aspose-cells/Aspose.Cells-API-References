---
title: "GridLoadOptions.CheckExcelRestriction"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà GridLoadOptions. Indica se verificare le restrizioni del file Excel quando l'utente modifica oggetti correlati alle celle. Per esempio Excel non consente l'inserimento di una stringa più lunga di 32K. Quando inserisci un valore più lungo di 32K, ad esempio tramite Cell.PutValuestring, se questa proprietà è true otterrai un'Exception. Se la proprietà è false accetteremo il valore stringa inserito come valore della cella, così in seguito potrai esportare la stringa completa per altri formati di file come CSV. Tuttavia, se hai impostato un valore di questo tipo non valido per il formato Excel, non dovresti salvare la cartella di lavoro come file Excel in seguito. Altrimenti potrebbero verificarsi errori imprevisti nel file Excel generato."
type: docs
url: /it/net/aspose.cells.gridweb.data/gridloadoptions/checkexcelrestriction/
---
## GridLoadOptions.CheckExcelRestriction property

Indica se verificare le restrizioni del file excel quando l'utente modifica oggetti correlati alle celle. Per esempio, excel non consente l'inserimento di una stringa più lunga di 32K. Quando inserisci un valore più lungo di 32K, ad esempio tramite Cell.PutValue(string), se questa proprietà è true otterrai un'Exception. Se la proprietà è false, accetteremo la stringa inserita come valore della cella, così in seguito potrai esportare la stringa completa per altri formati di file come CSV. Tuttavia, se hai impostato un valore di questo tipo non valido per il formato file excel, non dovresti salvare la workbook in formato excel in seguito. Altrimenti potrebbero verificarsi errori imprevisti nel file excel generato.

```csharp
public bool CheckExcelRestriction { get; set; }
```

### Vedi anche

* class [GridLoadOptions](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)


