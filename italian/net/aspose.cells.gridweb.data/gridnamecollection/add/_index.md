---
title: "GridNameCollection.Add"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "GridNameCollection metodo. Definisce un nuovo nome globale"
type: docs
url: /it/net/aspose.cells.gridweb.data/gridnamecollection/add/
---
## Add(string, string) {#add_1}

Definisce un nuovo nome globale.

```csharp
public int Add(string text, string refersTo)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| testo | String | Testo del nome. Può contenere il nome del foglio. |
| refersTo | String | La formula a cui il nome è definito per fare riferimento. Deve contenere il nome del foglio, ad es. 'sheet hello!'A1:B2. |

### Valore di ritorno

Indice dell'oggetto Name.

### Vedi anche

* class [GridNameCollection](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)

---

## Add(int, string, string) {#add}

Definisce un nuovo nome nel foglio specificato.

```csharp
public int Add(int sheetIndex, string text, string refersTo)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| sheetIndex | Int32 | L'indice del foglio in cui il nome è applicato. |
| testo | String | Testo del nome. Non può contenere il nome del foglio. |
| refersTo | String | La formula a cui il nome è definito per fare riferimento. Deve contenere il nome del foglio, ad es. 'sheet hello!'A1:B2. |

### Valore di ritorno

Indice dell'oggetto Name.

### Vedi anche

* class [GridNameCollection](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)


