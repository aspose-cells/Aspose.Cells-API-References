---
title: "Name.RefersTo"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Name. Restituisce o imposta la formula a cui il nome è definito per fare riferimento, iniziando con un segno di uguale"
type: docs
url: /it/net/aspose.cells/name/refersto/
---
## Name.RefersTo property

Restituisce o imposta la formula a cui il nome è definito per riferirsi, iniziando con il segno di uguale.

```csharp
public string RefersTo { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class NamePropertyRefersToDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Name = "Sheet1";

            // Aggiungi intervalli denominati con RefersTo
            int index1 = workbook.Worksheets.Names.Add("NamedRange1");
            workbook.Worksheets.Names[index1].RefersTo = "=Sheet1!$6:$8";
            
            int index2 = workbook.Worksheets.Names.Add("NamedRange2");
            workbook.Worksheets.Names[index2].RefersTo = "=Sheet1!$C:$D";

            // Visualizza la proprietà RefersTo degli intervalli denominati
            Console.WriteLine("NamedRange1 RefersTo: " + workbook.Worksheets.Names[0].RefersTo);
            Console.WriteLine("NamedRange2 RefersTo: " + workbook.Worksheets.Names[1].RefersTo);
        }
    }
}
```

### Vedi anche

* class [Name](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


