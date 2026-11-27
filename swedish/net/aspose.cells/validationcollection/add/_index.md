---
title: "ValidationCollection.Add"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ValidationCollection-metod. Lägger till en datavalidering i samlingen"
type: docs
url: /sv/net/aspose.cells/validationcollection/add/
---
## Add() {#add}

Lägger till en datavalidering i samlingen.

```csharp
[Obsolete("Use ValidationCollection.Add(CellArea) method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int Add()
```

### Returvärde

[`Validation`](../../validation/) object index.

### Anmärkningar

OBS: Den här metoden är nu föråldrad. Använd i stället ValidationCollection.Add(CellArea)-metoden. Denna metod kommer att tas bort 12 månader senare sedan JANUARY 2015. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

### Se även

* class [ValidationCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Add(CellArea) {#add_1}

Lägger till en datavalidering i samlingen.

```csharp
public int Add(CellArea ca)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| ca | CellArea | Området innehåller denna validering. |

### Returvärde

[`Validation`](../../validation/) object index.

### Exempel

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
            
            // Skapa cellområde för validering
            CellArea cellarea = new CellArea();
            cellarea.StartRow = 0;
            cellarea.StartColumn = 0;
            cellarea.EndRow = 1;
            cellarea.EndColumn = 1;
            
            // Lägg till validering i samlingen
            int index = sheet.Validations.Add(cellarea);
            Validation validation = sheet.Validations[index];
            
            // Konfigurera valideringsinställningar
            validation.Type = ValidationType.List;
            validation.Formula1 = "Yes,No";
            validation.AlertStyle = ValidationAlertType.Information;
            
            // Spara arbetsboken
            workbook.Save("ValidationCollectionMethodAddWithCellAreaDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Se även

* struct [CellArea](../../cellarea/)
* class [ValidationCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


