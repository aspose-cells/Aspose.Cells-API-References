---
title: "NameCollection.Item"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà NameCollection. Ottiene l'elemento Name all'indice specificato"
type: docs
url: /it/net/aspose.cells/namecollection/item/
---
## NameCollection indexer (1 of 2)

Ottiene l'elemento [`Name`](../../name/) all'indice specificato.

```csharp
public Name this[int index] { get; }
```

| Parametro | Descrizione |
| --- | --- |
| indice | L'indice a base zero dell'elemento. |

### Valore di ritorno

L'elemento all'indice specificato.

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class NameCollectionPropertyItemDemo1
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Aggiungi alcuni fogli di lavoro
            workbook.Worksheets.Add("Sheet1");
            workbook.Worksheets.Add("Sheet2");
            workbook.Worksheets.Add("Sheet3");

            // Accedi alla collezione di nomi
            NameCollection names = workbook.Worksheets.Names;
            
            // Aggiungi intervalli denominati usando la firma del metodo corretta
            int index1 = names.Add("Range1");
            names[index1].RefersTo = "=Sheet1!$A$1:$B$2";
            
            int index2 = names.Add("Range2");
            names[index2].RefersTo = "=Sheet2!$C$3:$D$4";
            
            int index3 = names.Add("Range3");
            names[index3].RefersTo = "=Sheet3!$E$5:$F$6";

            // Dimostra l'uso della proprietà Item
            Console.WriteLine("Named Ranges:");
            for (int i = 0; i < names.Count; i++)
            {
                Name name = names[i]; // Using Item property with index
                Console.WriteLine($"{name.Text}: {name.RefersTo}");
            }

            // Accedi per nome usando la proprietà Item
            Name specificName = names["Range2"];
            Console.WriteLine($"\nSpecific Range: {specificName.Text} refers to {specificName.RefersTo}");

            // Modifica un intervallo denominato
            names["Range3"].RefersTo = "=Sheet3!$A$1:$B$10";
            Console.WriteLine($"\nModified Range3 now refers to: {names["Range3"].RefersTo}");
        }
    }
}
```

### Vedi anche

* class [Name](../../name/)
* class [NameCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## NameCollection indexer (2 of 2)

Ottiene l'elemento [`Name`](../../name/) con il nome specificato.

```csharp
public Name this[string text] { get; }
```

| Parametro | Descrizione |
| --- | --- |
| testo | Testo del nome. |

### Valore di ritorno

L'elemento con il nome specificato.

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class NameCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi alla collezione dei nomi dei fogli di lavoro
            NameCollection names = workbook.Worksheets.Names;
            
            // Aggiungi alcuni intervalli denominati (corretto per usare la firma corretta del metodo Add)
            int index1 = names.Add("Range1");
            names[index1].RefersTo = "=Sheet1!$A$1:$A$10";
            
            int index2 = names.Add("Range2");
            names[index2].RefersTo = "=Sheet1!$B$1:$B$10";
            
            // Accedi agli intervalli denominati usando la proprietà Item
            Name range1 = names["Range1"];
            Name range2 = names["Range2"];
            
            // Verifica che i nomi esistano
            if (range1 != null && range2 != null)
            {
                Console.WriteLine("Named range 'Range1' refers to: " + range1.RefersTo);
                Console.WriteLine("Named range 'Range2' refers to: " + range2.RefersTo);
            }
            
            // Prova ad accedere a un nome inesistente
            Name range3 = names["NonExistentRange"];
            if (range3 == null)
            {
                Console.WriteLine("Named range 'NonExistentRange' not found");
            }
        }
    }
}
```

### Vedi anche

* class [Name](../../name/)
* class [NameCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


