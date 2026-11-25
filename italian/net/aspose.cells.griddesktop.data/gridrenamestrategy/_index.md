---
title: "Enum GridRenameStrategy"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Aspose.Cells.GridDesktop.Data.GridRenameStrategy enum. Opzione di strategia per nomi duplicati di colonne"
type: docs
url: /it/net/aspose.cells.griddesktop.data/gridrenamestrategy/
---
## GridRenameStrategy enumeration

Opzione di strategia per nomi duplicati delle colonne.

```csharp
public enum GridRenameStrategy
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| Exception | `0` | Lancia un'eccezione. |
| Digit | `1` | Denominato con cifra. I nomi duplicati diventeranno ...1, ...2, ecc. |
| Letter | `2` | Denominato con lettera. I nomi duplicati diventeranno ...A, ...B, ecc. |

### Osservazioni

Durante l'elaborazione dei dati con intestazioni, alcuni scenari richiedono che le intestazioni non siano duplicate per tutte le colonne. Ad esempio, quando si esportano i dati in un DataTable e l'intestazione deve essere utilizzata come nome della colonna del DataTable, i valori duplicati dell'intestazione sono invalidi. Per questo tipo di situazioni, l'utente può determinare come gestirle specificando questa strategia.

### Vedi anche

* namespace [Aspose.Cells.GridDesktop.Data](../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../)


