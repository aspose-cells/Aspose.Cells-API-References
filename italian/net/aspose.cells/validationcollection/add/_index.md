---
title: "ValidationCollection.Add"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo ValidationCollection. Aggiunge una convalida dei dati alla collezione"
type: docs
url: /it/net/aspose.cells/validationcollection/add/
---
## Add() {#add}

Aggiunge una convalida dei dati alla raccolta.

```csharp
[Obsolete("Use ValidationCollection.Add(CellArea) method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int Add()
```

### Valore di ritorno

[`Validation`](../../validation/) object index.

### Osservazioni

NOTA: Questo metodo è ora obsoleto. Invece, si prega di utilizzare il metodo ValidationCollection.Add(CellArea). Questo metodo sarà rimosso tra 12 mesi a partire da GENNAIO 2015. Aspose si scusa per qualsiasi inconveniente tu possa aver riscontrato.

### Vedi anche

* class [ValidationCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Add(CellArea) {#add_1}

Aggiunge una convalida dei dati alla raccolta.

```csharp
public int Add(CellArea ca)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| ca | CellArea | L'area contiene questa convalida. |

### Valore di ritorno

[`Validation`](../../validation/) object index.

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ValidationCollectionMethodAddWithCellAreaDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Creare un'area di celle per la convalida
            CellArea cellarea = new CellArea();
            cellarea.StartRow = 0;
            cellarea.StartColumn = 0;
            cellarea.EndRow = 1;
            cellarea.EndColumn = 1;
            
            // Aggiungere la convalida alla collezione
            int index = sheet.Validations.Add(cellarea);
            Validation validation = sheet.Validations[index];
            
            // Configura le impostazioni di convalida
            validation.Type = ValidationType.List;
            validation.Formula1 = "Yes,No";
            validation.AlertStyle = ValidationAlertType.Information;
            
            // Salva la cartella di lavoro
            workbook.Save("ValidationCollectionMethodAddWithCellAreaDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Vedi anche

* struct [CellArea](../../cellarea/)
* class [ValidationCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


