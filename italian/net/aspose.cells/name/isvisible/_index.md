---
title: "Name.IsVisible"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Name. Indica se il nome è visibile"
type: docs
url: /it/net/aspose.cells/name/isvisible/
---
## Name.IsVisible property

Indica se il nome è visibile.

```csharp
public bool IsVisible { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class NamePropertyIsVisibleDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Crea un intervallo denominato visibile
            int visibleIndex = workbook.Worksheets.Names.Add("VisibleRange");
            Name visibleName = workbook.Worksheets.Names[visibleIndex];
            visibleName.RefersTo = "=Sheet1!$A$1:$B$2";
            visibleName.IsVisible = true;
            
            // Crea un intervallo denominato nascosto
            int hiddenIndex = workbook.Worksheets.Names.Add("HiddenRange");
            Name hiddenName = workbook.Worksheets.Names[hiddenIndex];
            hiddenName.RefersTo = "=Sheet1!$C$1:$D$2";
            hiddenName.IsVisible = false;
            
            // Dimostra la proprietà IsVisible
            Console.WriteLine("VisibleRange IsVisible: " + visibleName.IsVisible);
            Console.WriteLine("HiddenRange IsVisible: " + hiddenName.IsVisible);
            
            // Salva la cartella di lavoro
            workbook.Save("NameVisibilityDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Name](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


