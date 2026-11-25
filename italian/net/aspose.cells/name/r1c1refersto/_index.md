---
title: "Name.R1C1RefersTo"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Name. Ottiene o imposta un riferimento R1C1 del Name"
type: docs
url: /it/net/aspose.cells/name/r1c1refersto/
---
## Name.R1C1RefersTo property

Ottiene o imposta un riferimento R1C1 del [`Name`](../).

```csharp
public string R1C1RefersTo { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class NamePropertyR1C1RefersToDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Aggiungi un nuovo nome alla collezione di nomi
            int nameIndex = workbook.Worksheets.Names.Add("TestRange");
            Name name = workbook.Worksheets.Names[nameIndex];
            
            // Imposta il riferimento R1C1 per il nome
            name.R1C1RefersTo = "'Sheet1'!R3C1:R9C4";
            
            // Verifica che il riferimento sia stato impostato correttamente
            Console.WriteLine("Name refers to: " + name.RefersTo);
            
            // Salva la cartella di lavoro
            workbook.Save("NamePropertyR1C1RefersToDemo_Output.xlsx");
        }
    }
}
```

### Vedi anche

* class [Name](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


