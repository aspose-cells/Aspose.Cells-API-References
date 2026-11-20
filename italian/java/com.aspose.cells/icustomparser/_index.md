---
title: "ICustomParser"
second_title: "Riferimento API di Aspose.Cells per Java"
description: "Consente agli utenti di aggiungere il proprio parser di valori personalizzato per analizzare i valori stringa in altri oggetti di valore cella appropriati."
type: docs
url: /it/java/com.aspose.cells/icustomparser/
---
```
public interface ICustomParser
```

Consente agli utenti di aggiungere il proprio parser di valori personalizzato per analizzare i valori stringa in altri oggetti di valore cella appropriati.
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [getFormat()](#getFormat--) | Restituisce il modello di formattazione corrispondente al valore analizzato dall'ultima invocazione di [parseObject(String)](../../com.aspose.cells/icustomparser\#parseObject-String-). |
| [parseObject(String value)](#parseObject-java.lang.String-) | Analizza la stringa fornita in un oggetto valore corretto. |
### getFormat() {#getFormat--}
```
public abstract String getFormat()
```


Restituisce il modello di formattazione corrispondente al valore analizzato dall'ultima invocazione di [parseObject(String)](../../com.aspose.cells/icustomparser\#parseObject-String-).

**Remarks**

Il modello di formattazione restituito può essere utilizzato per formattare la cella corrispondente (impostare su Style.Custom per la cella).

**Returns:**
java.lang.String
### parseObject(String value) {#parseObject-java.lang.String-}
```
public abstract Object parseObject(String value)
```


Analizza la stringa fornita in un oggetto valore corretto.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String | Il valore stringa da analizzare |

**Returns:**
java.lang.Object - Oggetto valore analizzato dalla stringa fornita. Se la stringa fornita non può essere analizzata in un oggetto valore corretto, restituisce null.
