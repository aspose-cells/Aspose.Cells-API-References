---
title: "Classe ConnectionParameter"
linktitle: "ConnectionParameter"
second_title: "Riferimento API C++ di Aspose.Cells per Go"
description: "Classe ConnectionParameter. Incapsula l'oggetto che rappresenta connectionparameter in Go."
type: docs
weight: 200
url: /it/go-cpp/connectionparameter/
---

## ConnectionParameter class

Specifica le proprietà di tutti i parametri utilizzati con le connessioni dati esterne. I parametri sono validi per ODBC e query web.

```go

type ConnectionParameter struct  {
	ptr unsafe.Pointer
}

```
## Costruttori

| Metodo | Descrizione |
| --- | --- |

## Metodi

| Metodo | Descrizione |
| --- | --- |
| [IsNull](./isnull/) | Verifica se l'oggetto di implementazione è nullptr. |
| [GetSqlType](./getsqltype/) | Tipo di dati SQL del parametro. Valido solo per le origini ODBC. |
| [SetSqlType](./setsqltype/) | Tipo di dati SQL del parametro. Valido solo per le origini ODBC. |
| [GetRefreshOnChange](./getrefreshonchange/) | Flag che indica se la query deve aggiornarsi automaticamente quando il contenuto di una cella che fornisce il valore del parametro cambia. Se true, i dati esterni vengono aggiornati utilizzando il nuovo valore del parametro ogni volta che si verifica una modifica. Se false, i dati esterni vengono aggiornati solo quando richiesto dall'utente, o quando qualche altro evento attiva l'aggiornamento (ad esempio, apertura della cartella di lavoro). |
| [SetRefreshOnChange](./setrefreshonchange/) | Flag che indica se la query deve aggiornarsi automaticamente quando il contenuto di una cella che fornisce il valore del parametro cambia. Se true, i dati esterni vengono aggiornati utilizzando il nuovo valore del parametro ogni volta che si verifica una modifica. Se false, i dati esterni vengono aggiornati solo quando richiesto dall'utente, o quando qualche altro evento attiva l'aggiornamento (ad esempio, apertura della cartella di lavoro). |
| [GetPrompt](./getprompt/) | Stringa di prompt per il parametro. Presentata all'utente del foglio di calcolo insieme all'interfaccia UI di input per raccogliere il valore del parametro prima di aggiornare i dati esterni. Utilizzata solo quando parameterType = prompt. |
| [SetPrompt](./setprompt/) | Stringa di prompt per il parametro. Presentata all'utente del foglio di calcolo insieme all'interfaccia UI di input per raccogliere il valore del parametro prima di aggiornare i dati esterni. Utilizzata solo quando parameterType = prompt. |
| [GetType](./gettype/) | Tipo di parametro utilizzato. Se parameterType=valore, allora verrà usato il valore da boolean, double, integer o string. In questo caso, ci si aspetta che venga specificato solo uno di {boolean, double, integer, or string}. |
| [SetType](./settype/) | Tipo di parametro utilizzato. Se parameterType=valore, allora verrà usato il valore da boolean, double, integer o string. In questo caso, ci si aspetta che venga specificato solo uno di {boolean, double, integer, or string}. |
| [GetName](./getname/) | Il nome del parametro. |
| [SetName](./setname/) | Il nome del parametro. |
| [GetCellReference](./getcellreference/) | Riferimento di cella che indica quale valore di cella utilizzare per il parametro della query. Utilizzato solo quando parameterType è cell. |
| [SetCellReference](./setcellreference/) | Riferimento di cella che indica quale valore di cella utilizzare per il parametro della query. Utilizzato solo quando parameterType è cell. |
| [GetValue](./getvalue/) | Valore numerico non intero, valore intero, valore stringa o valore booleano da utilizzare come parametro della query. Utilizzato solo quando parameterType è value. |
| [SetValue](./setvalue/) | Valore numerico non intero, valore intero, valore stringa o valore booleano da utilizzare come parametro della query. Utilizzato solo quando parameterType è value. |
