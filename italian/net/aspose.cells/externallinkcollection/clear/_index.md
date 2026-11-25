---
title: "ExternalLinkCollection.Clear"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo ExternalLinkCollection. Rimuove tutti i collegamenti esterni"
type: docs
url: /it/net/aspose.cells/externallinkcollection/clear/
---
## Clear() {#clear}

Rimuove tutti i collegamenti esterni.

```csharp
public void Clear()
```

### Osservazioni

Durante la rimozione dei collegamenti esterni, tutte le formule che vi fanno riferimento verranno rimosse perché i riferimenti diventano non validi.

### Vedi anche

* class [ExternalLinkCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Clear(bool) {#clear_1}

Rimuove tutti i collegamenti esterni.

```csharp
public void Clear(bool updateReferencesAsLocal)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| updateReferencesAsLocal | Booleano | Indica se aggiornare tutti i riferimenti ai collegamenti esterni nelle formule ai riferimenti della cartella di lavoro corrente. |

### Osservazioni

Se è necessario aggiornare i riferimenti, i riferimenti ai collegamenti esterni nelle formule verranno modificati alla cartella di lavoro corrente quando possibile. Ad esempio, la formula originale di una cella è "='externalsource.xlam'!customfunction()", dopo la rimozione dei collegamenti esterni la formula diventerà "=customfunction()"; quando la formula originale è "='[externalsource.xlam]Sheet1'!$A$1", a seconda che esista un foglio con nome "Sheet1" nella cartella di lavoro corrente: se vero, la formula diventerà "=Sheet1!$A$1"; se falso, la formula diventerà "=#REF!$A$1". Se i riferimenti non devono essere aggiornati, tutte le formule con riferimenti a collegamenti esterni verranno rimosse perché tali riferimenti diventano non validi.

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ExternalLinkCollectionMethodClearWithBooleanDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro
            Workbook workbook = new Workbook();
            
            // Aggiungi alcuni collegamenti esterni
            ExternalLinkCollection externalLinks = workbook.Worksheets.ExternalLinks;
            externalLinks.Add("externalWorkbook.xlsx", new string[] { "Sheet1" });
            externalLinks.Add("anotherExternal.xlsx", new string[] { "Sheet1" });
            
            Console.WriteLine("External links count before clear: " + externalLinks.Count);
            
            // Cancella con updateReferences = true
            externalLinks.Clear(true);
            Console.WriteLine("External links count after clear (updateReferences=true): " + externalLinks.Count);
            
            // Aggiungi nuovamente i collegamenti
            externalLinks.Add("externalWorkbook.xlsx", new string[] { "Sheet1" });
            externalLinks.Add("anotherExternal.xlsx", new string[] { "Sheet1" });
            
            // Cancella con updateReferences = false
            externalLinks.Clear(false);
            Console.WriteLine("External links count after clear (updateReferences=false): " + externalLinks.Count);
        }
    }
}
```

### Vedi anche

* class [ExternalLinkCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


