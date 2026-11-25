---
title: "Classe ComboBox"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.GridDesktop.ComboBox. Rappresenta un controllo combobox della cella"
type: docs
url: /it/net/aspose.cells.griddesktop/combobox/
---
## ComboBox class

Rappresenta un controllo combobox della cella.

```csharp
public class ComboBox : CellControl
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [Height](../../aspose.cells.griddesktop/combobox/height/) { get; set; } | Ottiene o imposta l'altezza del controllo elenco. |
| [IsInputable](../../aspose.cells.griddesktop/combobox/isinputable/) { get; set; } | Indica se l'utente può inserire testo nel combobox. Il testo inserito verrà salvato come valore della cella. Il valore predefinito è "false". |
| [Items](../../aspose.cells.griddesktop/combobox/items/) { get; } | Ottiene un oggetto che rappresenta la collezione degli elementi contenuti in questo ComboBox. |
| [SelectedIndex](../../aspose.cells.griddesktop/combobox/selectedindex/) { get; set; } | Ottiene o imposta l'indice che specifica l'elemento attualmente selezionato. Impostare l'indice chiamerà automaticamente il metodo GridDesktop.RunAllFormulas se la proprietà GridDesktop.RecalculateFormulas è true. |
| [Text](../../aspose.cells.griddesktop/cellcontrol/text/) { get; set; } | Ottiene o imposta il testo associato a questo controllo. (Ereditato da [`CellControl`](../cellcontrol/).) |
| [Values](../../aspose.cells.griddesktop/combobox/values/) { get; } | Ottiene un oggetto che rappresenta la collezione dei valori contenuti in questo ComboBox. |
| [Width](../../aspose.cells.griddesktop/combobox/width/) { get; set; } | Ottiene o imposta la larghezza del controllo elenco. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [SetSelectedIndex](../../aspose.cells.griddesktop/combobox/setselectedindex/)(int) | Imposta l'indice selezionato del ComboBox. Questo non calcolerà la formula. Per calcolare la formula, è necessario chiamare manualmente GridDesktop.RunAllFormulas. Non calcolerà automaticamente le formule in nessun caso, anche se GridDesktop.RecalculateFormulas è true. |

### Vedi anche

* class [CellControl](../cellcontrol/)
* namespace [Aspose.Cells.GridDesktop](../../aspose.cells.griddesktop/)
* assembly [Aspose.Cells.GridDesktop](../../)


