---
title: "GridCustomServerValidation"
second_title: "Riferimento API di Aspose.Cells per Java"
description: "l'interfaccia che devi implementare quando usi la convalida lato server."
type: docs
url: /it/java/com.aspose.gridweb/gridcustomservervalidation/
---
```
public interface GridCustomServerValidation
```

l'interfaccia che devi implementare quando usi la convalida lato server. CustomServerFunction.
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [validate(GridWorksheet sheet, int row, int col, String value)](#validate-com.aspose.gridweb.GridWorksheet-int-int-java.lang.String-) | **Osservazioni** |
### validate(GridWorksheet sheet, int row, int col, String value) {#validate-com.aspose.gridweb.GridWorksheet-int-int-java.lang.String-}
```
public abstract String validate(GridWorksheet sheet, int row, int col, String value)
```


**Remarks**

se restituisci string.empty la convalida è superata, altrimenti puoi restituire qualsiasi messaggio correlato che può essere gestito nella funzione ClientCallback

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| sheet | [GridWorksheet](../../com.aspose.gridweb/gridworksheet) | il GridWorksheet |
| riga | int | l'indice di riga della cella |
| col | int | l'indice di colonna della cella |
| valore | java.lang.String | il valore per eseguire la convalida |

**Returns:**
java.lang.String - valore risultato basato su stringa
