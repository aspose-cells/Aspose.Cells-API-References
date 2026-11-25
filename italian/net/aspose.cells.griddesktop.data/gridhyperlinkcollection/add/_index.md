---
title: "GridHyperlinkCollection.Add"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "GridHyperlinkCollection metodo. Aggiunge un collegamento ipertestuale a una cella specificata o a un intervallo di celle"
type: docs
url: /it/net/aspose.cells.griddesktop.data/gridhyperlinkcollection/add/
---
## Add(int, int, int, int, string) {#add}

Aggiunge un hyperlink a una cella specificata o a un intervallo di celle.

```csharp
public int Add(int firstRow, int firstColumn, int totalRows, int totalColumns, string address)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| firstRow | Int32 | Prima riga dell'intervallo di collegamenti ipertestuali. |
| firstColumn | Int32 | Prima colonna dell'intervallo di collegamenti ipertestuali. |
| totalRows | Int32 | Numero di righe in questo intervallo di collegamenti ipertestuali. |
| totalColumns | Int32 | Numero di colonne di questo intervallo di collegamenti ipertestuali. |
| address | String | Indirizzo del collegamento ipertestuale. |

### Valore di ritorno

Indice dell'oggetto hyperlink.

### Esempi

```csharp
[C#]

Worksheet worksheet = excel.Worksheets[0];
worksheet.Hyperlinks.Add("A4", 1, 1, "http://www.aspose.com");
worksheet.Hyperlinks.Add("A5", 1, 1, "c:\\book1.xls");

[Visual Basic]

Dim worksheet as Worksheet = excel.Worksheets(0)
worksheet.Hyperlinks.Add("A4", 1, 1, "http://www.aspose.com")
worksheet.Hyperlinks.Add("A5", 1, 1, "c:\\book1.xls")

```

### Vedi anche

* class [GridHyperlinkCollection](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)

---

## Add(string, int, int, string) {#add_1}

Aggiunge un hyperlink a una cella specificata o a un intervallo di celle.

```csharp
public int Add(string cellName, int totalRows, int totalColumns, string address)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| cellName | String | Nome della cella. |
| totalRows | Int32 | Numero di righe in questo intervallo di collegamenti ipertestuali. |
| totalColumns | Int32 | Numero di colonne di questo intervallo di collegamenti ipertestuali. |
| address | String | Indirizzo del collegamento ipertestuale. |

### Valore di ritorno

Indice dell'oggetto hyperlink.

### Vedi anche

* class [GridHyperlinkCollection](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)

---

## Add(string, string) {#add_2}

Aggiunge un hyperlink a una cella specificata.

```csharp
public int Add(string cellName, string address)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| cellName | String | Nome della cella. |
| address | String | Indirizzo del collegamento ipertestuale. |

### Valore di ritorno

Indice dell'oggetto hyperlink.

### Vedi anche

* class [GridHyperlinkCollection](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)

---

## Add(string, string, string, string, string) {#add_3}

Aggiunge un hyperlink a una cella specificata o a un intervallo di celle.

```csharp
public int Add(string startCellName, string endCellName, string address, string textToDisplay, 
    string screenTip)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| startCellName | String | La cella in alto a sinistra dell'intervallo. |
| endCellName | String | La cella in basso a destra dell'intervallo. |
| address | String | Indirizzo del collegamento ipertestuale. |
| textToDisplay | String | Il testo da visualizzare per il collegamento ipertestuale specificato. |
| screenTip | String | Il testo screenTip per il collegamento ipertestuale specificato. |

### Valore di ritorno

Indice dell'oggetto hyperlink.

### Vedi anche

* class [GridHyperlinkCollection](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)

---

## Add(int, int, string) {#add_4}

Aggiunge un hyperlink a una cella specificata all'indice di riga e colonna.

```csharp
public void Add(int row, int col, string url)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| riga | Int32 | Indice di riga della cella. |
| col | Int32 | Indice di colonna della cella. |
| url | String | Url dell'hyperlink. |

### Vedi anche

* class [GridHyperlinkCollection](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)


