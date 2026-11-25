---
title: "Classe ProtectedRange"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.ProtectedRange. Un intervallo specificato che può essere modificato quando la protezione del foglio è ATTIVA"
type: docs
url: /it/net/aspose.cells/protectedrange/
---
## ProtectedRange class

Un intervallo specificato che può essere modificato quando la protezione del foglio è ATTIVA.

```csharp
public class ProtectedRange
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [CellArea](../../aspose.cells/protectedrange/cellarea/) { get; } | Ottiene l'oggetto [`CellArea`](./cellarea/) che rappresenta l'area di celle da proteggere. |
| [IsProtectedWithPassword](../../aspose.cells/protectedrange/isprotectedwithpassword/) { get; } | Indica se i fogli di lavoro sono protetti da password. |
| [Name](../../aspose.cells/protectedrange/name/) { get; set; } | Ottiene il titolo dell'intervallo. Questo è usato come descrizione, non come definizione di intervallo nominato. |
| [Password](../../aspose.cells/protectedrange/password/) { get; set; } | Rappresenta la password per proteggere l'intervallo. |
| [SecurityDescriptor](../../aspose.cells/protectedrange/securitydescriptor/) { get; set; } | Il descrittore di sicurezza definisce gli account utente che possono modificare questo intervallo senza fornire una password per accedere all'intervallo. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [AddArea](../../aspose.cells/protectedrange/addarea/)(int, int, int, int) | Aggiunge un'area di riferimento a questo |
| [GetAreas](../../aspose.cells/protectedrange/getareas/)() | Ottiene tutte le aree di riferimento. |

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassProtectedRangeDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ottieni la collezione di intervalli protetti
            ProtectedRangeCollection protectedRanges = worksheet.AllowEditRanges;
            
            // Aggiungi un nuovo intervallo protetto (A1:J10)
            int index = protectedRanges.Add("MyProtectedRange", 0, 0, 10, 10);
            
            // Ottieni l'intervallo protetto
            ProtectedRange protectedRange = protectedRanges[index];
            
            // Imposta il descrittore di sicurezza
            string securityDescriptor = "O:WDG:WDD:(D;;CC;;;S-1-5-21-2854911246-2539335229-2923752399-1000)(A;;CC;;;S-1-5-21-2854911246-2539335229-2923752399-1013)";
            protectedRange.SecurityDescriptor = securityDescriptor;
            
            // Salva la cartella di lavoro
            workbook.Save("ProtectedRangeDemo.xlsx");
            
            Console.WriteLine("Protected range demo completed successfully.");
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


