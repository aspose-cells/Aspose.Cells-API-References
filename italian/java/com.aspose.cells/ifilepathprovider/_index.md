---
title: "IFilePathProvider"
second_title: "Riferimento API di Aspose.Cells per Java"
description: "Rappresenta il provider del percorso del file esportato."
type: docs
url: /it/java/com.aspose.cells/ifilepathprovider/
---
```
public interface IFilePathProvider
```

Rappresenta il provider del percorso del file esportato.
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [getFullName(String sheetName)](#getFullName-java.lang.String-) | Ottiene il percorso completo del file per nome del foglio di lavoro quando si esporta il foglio di lavoro in HTML separatamente. |
### getFullName(String sheetName) {#getFullName-java.lang.String-}
```
public abstract String getFullName(String sheetName)
```


Ottiene il percorso completo del file per nome del foglio di lavoro quando si esporta il foglio di lavoro in HTML separatamente. In modo che i riferimenti tra i fogli di lavoro possano essere esportati correttamente.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| sheetName | java.lang.String | Nome del foglio di lavoro |

**Returns:**
java.lang.String - il percorso completo del file
