---
title: "CellsHelper.CreateSafeSheetName"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo CellsHelper. Controlla il nome del foglio fornito e crea uno valido quando necessario. Se il nome del foglio fornito rispetta le regole dei nomi dei fogli Excel, lo restituisce. Altrimenti la stringa verrà troncata se la lunghezza supera il limite e i caratteri non validi saranno sostituiti con   quindi verrà restituito il valore della stringa ricostruita."
type: docs
url: /it/net/aspose.cells/cellshelper/createsafesheetname/
---
## CreateSafeSheetName(string) {#createsafesheetname}

Verifica il nome del foglio fornito e crea uno valido quando necessario. Se il nome del foglio fornito rispetta le regole dei nomi dei fogli Excel, lo restituisce. Altrimenti la stringa verrà troncata se la lunghezza supera il limite e i caratteri non validi saranno sostituiti con ' ', quindi verrà restituito il valore della stringa ricostruita.

```csharp
public static string CreateSafeSheetName(string nameProposal)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| nameProposal | String | nome del foglio da utilizzare |

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsHelperMethodCreateSafeSheetNameWithStringDemo
    {
        public static void Run()
        {
            string unsafeName = "sheet*/test*/?#";
            string safeName = CellsHelper.CreateSafeSheetName(unsafeName);
            Console.WriteLine("Original name: " + unsafeName);
            Console.WriteLine("Safe name: " + safeName);
        }
    }
}
```

### Vedi anche

* class [CellsHelper](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## CreateSafeSheetName(string, char) {#createsafesheetname_1}

Verifica il nome del foglio fornito e crea uno valido quando necessario. Se il nome del foglio fornito rispetta le regole dei nomi dei fogli Excel, lo restituisce. Altrimenti la stringa verrà troncata se la lunghezza supera il limite e i caratteri non validi saranno sostituiti con il carattere fornito, quindi verrà restituito il valore della stringa ricostruita.

```csharp
public static string CreateSafeSheetName(string nameProposal, char replaceChar)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| nameProposal | String | nome del foglio da utilizzare |
| replaceChar | Carattere | carattere che verrà usato per sostituire i caratteri non validi nel nome del foglio fornito |

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsHelperMethodCreateSafeSheetNameWithStringCharDemo
    {
        public static void Run()
        {
            // Esempio 1: Crea un nome di foglio sicuro con il carattere di sostituzione predefinito
            string name1 = CellsHelper.CreateSafeSheetName("sheet*/test*/?#");
            Console.WriteLine("Safe sheet name (default replacement): " + name1);

            // Esempio 2: Crea un nome di foglio sicuro con un carattere di sostituzione personalizzato 'A'
            string name2 = CellsHelper.CreateSafeSheetName("sheet*/test*/?#", 'A');
            Console.WriteLine("Safe sheet name (custom replacement): " + name2);
        }
    }
}
```

### Vedi anche

* class [CellsHelper](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


