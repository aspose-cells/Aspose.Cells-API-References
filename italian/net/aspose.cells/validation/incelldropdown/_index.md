---
title: "Validation.InCellDropDown"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà di convalida. Indica se la convalida dei dati visualizza un elenco a discesa che contiene valori accettabili"
type: docs
url: /it/net/aspose.cells/validation/incelldropdown/
---
## Validation.InCellDropDown property

Indica se la convalida dei dati visualizza un elenco a discesa che contiene valori accettabili.

```csharp
public bool InCellDropDown { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ValidationPropertyInCellDropDownDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crea una convalida per la cella A1
            Validation validation = worksheet.Cells["A1"].GetValidation();
            
            // Imposta il tipo di convalida su elenco con valori
            validation.Type = ValidationType.List;
            validation.Formula1 = "Option1,Option2,Option3";
            
            // Abilita l'elenco a discesa nella cella
            validation.InCellDropDown = true;

            // Crea un'altra convalida per la cella B1 senza elenco a discesa
            Validation validation2 = worksheet.Cells["B1"].GetValidation();
            validation2.Type = ValidationType.List;
            validation2.Formula1 = "Choice1,Choice2,Choice3";
            validation2.InCellDropDown = false;

            // Salva la cartella di lavoro
            workbook.Save("InCellDropDownDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Validation](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


