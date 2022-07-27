---
title: Protection
second_title: Riferimento alle API di Aspose.Cells per .NET
description: Rappresenta i vari tipi di opzioni di protezione disponibili per un foglio di lavoro.
type: docs
weight: 4910
url: /it/net/aspose.cells/protection/
---
## Protection class

Rappresenta i vari tipi di opzioni di protezione disponibili per un foglio di lavoro.

```csharp
public class Protection
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [AllowDeletingColumn](../../aspose.cells/protection/allowdeletingcolumn) { get; set; } | Rappresenta se l'eliminazione di colonne è consentita su un foglio di lavoro protetto. |
| [AllowDeletingRow](../../aspose.cells/protection/allowdeletingrow) { get; set; } | Rappresenta se l'eliminazione di righe è consentita su un foglio di lavoro protetto. |
| [AllowEditingContent](../../aspose.cells/protection/alloweditingcontent) { get; set; } | Indica se l'utente è autorizzato a modificare il contenuto delle celle bloccate su un foglio di lavoro protetto. |
| [AllowEditingObject](../../aspose.cells/protection/alloweditingobject) { get; set; } | Indica se l'utente è autorizzato a manipolare oggetti di disegno su un foglio di lavoro protetto. |
| [AllowEditingScenario](../../aspose.cells/protection/alloweditingscenario) { get; set; } | Indica se l'utente è autorizzato a modificare gli scenari su un foglio di lavoro protetto. |
| [AllowFiltering](../../aspose.cells/protection/allowfiltering) { get; set; } | Indica se l'utente può utilizzare un filtro automatico creato prima che il foglio fosse protetto. |
| [AllowFormattingCell](../../aspose.cells/protection/allowformattingcell) { get; set; } | Indica se la formattazione delle celle è consentita su un foglio di lavoro protetto. |
| [AllowFormattingColumn](../../aspose.cells/protection/allowformattingcolumn) { get; set; } | Rappresenta se la formattazione delle colonne è consentita su un foglio di lavoro protetto |
| [AllowFormattingRow](../../aspose.cells/protection/allowformattingrow) { get; set; } | Rappresenta se la formattazione delle righe è consentita su un foglio di lavoro protetto |
| [AllowInsertingColumn](../../aspose.cells/protection/allowinsertingcolumn) { get; set; } | Rappresenta se l'inserimento di colonne è consentito su un foglio di lavoro protetto |
| [AllowInsertingHyperlink](../../aspose.cells/protection/allowinsertinghyperlink) { get; set; } | Rappresenta se l'inserimento di collegamenti ipertestuali è consentito su un foglio di lavoro protetto |
| [AllowInsertingRow](../../aspose.cells/protection/allowinsertingrow) { get; set; } | Rappresenta se l'inserimento di righe è consentito su un foglio di lavoro protetto |
| [AllowSelectingLockedCell](../../aspose.cells/protection/allowselectinglockedcell) { get; set; } | Indica se l'utente può selezionare le celle bloccate su un foglio di lavoro protetto. |
| [AllowSelectingUnlockedCell](../../aspose.cells/protection/allowselectingunlockedcell) { get; set; } | Indica se l'utente è autorizzato a selezionare celle sbloccate su un foglio di lavoro protetto. |
| [AllowSorting](../../aspose.cells/protection/allowsorting) { get; set; } | Indica se l'opzione di ordinamento è consentita su un foglio di lavoro protetto. |
| [AllowUsingPivotTable](../../aspose.cells/protection/allowusingpivottable) { get; set; } | Indica se l'utente può manipolare tabelle pivot su un foglio di lavoro protetto. |
| [IsProtectedWithPassword](../../aspose.cells/protection/isprotectedwithpassword) { get; } | Indica se i fogli di lavoro sono protetti con password. |
| [Password](../../aspose.cells/protection/password) { get; set; } | Rappresenta la password per proteggere il foglio di lavoro. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [Copy](../../aspose.cells/protection/copy)(Protection) | Informazioni sulla protezione dalla copia. |
| [GetPasswordHash](../../aspose.cells/protection/getpasswordhash)() | Ottiene l'hash della password corrente. |
| [VerifyPassword](../../aspose.cells/protection/verifypassword)(string) | Verifica la password. |

### Esempi

```csharp

[C#]
//Creazione di un'istanza di un oggetto cartella di lavoro
Workbook workbook = new Workbook();

Worksheet worksheet = workbook.Worksheets[0];
//Consenti agli utenti di selezionare le celle bloccate del foglio di lavoro
worksheet.Protection.AllowSelectingLockedCell = true;
//Consenti agli utenti di selezionare le celle sbloccate del foglio di lavoro
worksheet.Protection.AllowSelectingUnlockedCell = true;  

[Visual Basic]

'Creazione di un'istanza di un oggetto Workbook
Dim workbook As Workbook = New Workbook()
Dim worksheet As Worksheet = workbook.Worksheets(0)
'Consentire agli utenti di selezionare le celle bloccate del foglio di lavoro
worksheet.Protection.AllowSelectingLockedCell = True
'Consentire agli utenti di selezionare le celle sbloccate del foglio di lavoro
worksheet.Protection.AllowSelectingUnlockedCell = True
```

### Guarda anche

* spazio dei nomi [Aspose.Cells](../../aspose.cells)
* assemblea [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
