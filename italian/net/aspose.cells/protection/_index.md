---
title: "Classe Protection"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.Protection. Rappresenta i vari tipi di opzioni di protezione disponibili per un foglio di lavoro"
type: docs
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
| [AllowDeletingColumn](../../aspose.cells/protection/allowdeletingcolumn/) { get; set; } | Rappresenta se l'eliminazione delle colonne è consentita su un foglio di lavoro protetto. |
| [AllowDeletingRow](../../aspose.cells/protection/allowdeletingrow/) { get; set; } | Rappresenta se l'eliminazione delle righe è consentita su un foglio di lavoro protetto. |
| [AllowEditingContent](../../aspose.cells/protection/alloweditingcontent/) { get; set; } | Rappresenta se all'utente è consentito modificare il contenuto delle celle bloccate su un foglio di lavoro protetto. |
| [AllowEditingObject](../../aspose.cells/protection/alloweditingobject/) { get; set; } | Rappresenta se all'utente è consentito manipolare gli oggetti di disegno su un foglio di lavoro protetto. |
| [AllowEditingScenario](../../aspose.cells/protection/alloweditingscenario/) { get; set; } | Rappresenta se all'utente è consentito modificare gli scenari su un foglio di lavoro protetto. |
| [AllowFiltering](../../aspose.cells/protection/allowfiltering/) { get; set; } | Rappresenta se all'utente è consentito utilizzare un AutoFiltro creato prima che il foglio fosse protetto. |
| [AllowFormattingCell](../../aspose.cells/protection/allowformattingcell/) { get; set; } | Rappresenta se la formattazione delle celle è consentita su un foglio di lavoro protetto. |
| [AllowFormattingColumn](../../aspose.cells/protection/allowformattingcolumn/) { get; set; } | Rappresenta se la formattazione delle colonne è consentita su un foglio di lavoro protetto |
| [AllowFormattingRow](../../aspose.cells/protection/allowformattingrow/) { get; set; } | Rappresenta se la formattazione delle righe è consentita su un foglio di lavoro protetto |
| [AllowInsertingColumn](../../aspose.cells/protection/allowinsertingcolumn/) { get; set; } | Rappresenta se l'inserimento delle colonne è consentito su un foglio di lavoro protetto |
| [AllowInsertingHyperlink](../../aspose.cells/protection/allowinsertinghyperlink/) { get; set; } | Rappresenta se l'inserimento dei collegamenti ipertestuali è consentito su un foglio di lavoro protetto |
| [AllowInsertingRow](../../aspose.cells/protection/allowinsertingrow/) { get; set; } | Rappresenta se l'inserimento delle righe è consentito su un foglio di lavoro protetto |
| [AllowSelectingLockedCell](../../aspose.cells/protection/allowselectinglockedcell/) { get; set; } | Rappresenta se all'utente è consentito selezionare le celle bloccate su un foglio di lavoro protetto. |
| [AllowSelectingUnlockedCell](../../aspose.cells/protection/allowselectingunlockedcell/) { get; set; } | Rappresenta se all'utente è consentito selezionare le celle sbloccate su un foglio di lavoro protetto. |
| [AllowSorting](../../aspose.cells/protection/allowsorting/) { get; set; } | Rappresenta se l'opzione di ordinamento è consentita su un foglio di lavoro protetto. |
| [AllowUsingPivotTable](../../aspose.cells/protection/allowusingpivottable/) { get; set; } | Rappresenta se all'utente è consentito manipolare le tabelle pivot su un foglio di lavoro protetto. |
| [IsProtectedWithPassword](../../aspose.cells/protection/isprotectedwithpassword/) { get; } | Indica se i fogli di lavoro sono protetti da password. |
| [Password](../../aspose.cells/protection/password/) { get; set; } | Rappresenta la password per proteggere il foglio di lavoro. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [Copy](../../aspose.cells/protection/copy/)(Protection) | Copia le informazioni di protezione. |
| [GetPasswordHash](../../aspose.cells/protection/getpasswordhash/)() | Ottiene l'hash della password corrente. |
| [VerifyPassword](../../aspose.cells/protection/verifypassword/)(string) | Verifica la password. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ProtectionDemo
    {
        public static void ProtectionExample()
        {
            // Istanziare un oggetto Workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Accesso alle impostazioni di protezione del foglio di lavoro
            Protection protection = worksheet.Protection;

            // Impostazione di varie proprietà di protezione
            protection.AllowDeletingColumn = true;
            protection.AllowDeletingRow = true;
            protection.AllowFiltering = true;
            protection.AllowFormattingCell = true;
            protection.AllowFormattingColumn = true;
            protection.AllowFormattingRow = true;
            protection.AllowInsertingColumn = true;
            protection.AllowInsertingHyperlink = true;
            protection.AllowInsertingRow = true;
            protection.AllowSorting = true;
            protection.AllowUsingPivotTable = true;
            protection.AllowEditingContent = true;
            protection.AllowEditingObject = true;
            protection.AllowEditingScenario = true;
            protection.Password = "password123";
            protection.AllowSelectingLockedCell = true;
            protection.AllowSelectingUnlockedCell = true;

            // Verifica se il foglio di lavoro è protetto da una password
            bool isProtectedWithPassword = protection.IsProtectedWithPassword;

            // Salvataggio della cartella di lavoro
            workbook.Save("ProtectionExample.xlsx");

            return;
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


