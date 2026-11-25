---
title: "Enum ParameterType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Aspose.Cells.ParameterType enum. Rappresenta tutti i tipi di parametri o il tipo di valore di ritorno della funzione"
type: docs
url: /it/net/aspose.cells/parametertype/
---
## ParameterType enumeration

Rappresenta il tipo di tutti i parametri o il tipo di valore di ritorno di una funzione.

```csharp
public enum ParameterType
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| Reference | `0` |  |
| Value | `1` |  |
| Array | `2` |  |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ParameterTypeDemo
    {
        public static void ParameterTypeExample()
        {
            // Creazione di una cartella di lavoro e di un foglio per dimostrare l'uso
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Esempio di utilizzo dell'enum ParameterType in una funzione di formula
            // Supponiamo di definire una funzione personalizzata con tipi di parametro specifici

            // Definisci un array di tipi di parametro
            ParameterType[] parameterTypes = new ParameterType[]
            {
                ParameterType.Reference,
                ParameterType.Value,
                ParameterType.Array
            };

            // Funzione di esempio che utilizza questi tipi di parametro
            // Ad esempio, impostare una funzione personalizzata ipotetica con tipi di parametro definiti
            // (Nota: la gestione delle funzioni personalizzate dipenderebbe dalle capacità dell'API Aspose.Cells)

            // Salva la cartella di lavoro per dimostrare le modifiche
            workbook.Save("ParameterTypeExample.xlsx");
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


