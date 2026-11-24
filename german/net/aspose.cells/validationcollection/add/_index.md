---
title: "ValidationCollection.Add"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ValidationCollection-Methode. Fügt der Sammlung eine Datenvalidierung hinzu"
type: docs
url: /de/net/aspose.cells/validationcollection/add/
---
## Add() {#add}

Fügt der Sammlung eine Datenvalidierung hinzu.

```csharp
[Obsolete("Use ValidationCollection.Add(CellArea) method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int Add()
```

### Rückgabewert

[`Validation`](../../validation/) object index.

### Hinweise

HINWEIS: Diese Methode ist jetzt veraltet. Verwenden Sie stattdessen die Methode ValidationCollection.Add(CellArea). Diese Methode wird 12 Monate später, seit JANUAR 2015, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie möglicherweise erlebt haben.

### Siehe auch

* class [ValidationCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Add(CellArea) {#add_1}

Fügt der Sammlung eine Datenvalidierung hinzu.

```csharp
public int Add(CellArea ca)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| ca | CellArea | Der Bereich enthält diese Validierung. |

### Rückgabewert

[`Validation`](../../validation/) object index.

### Beispiele

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
            
            // Erstellen Sie einen Zellbereich für die Validierung
            CellArea cellarea = new CellArea();
            cellarea.StartRow = 0;
            cellarea.StartColumn = 0;
            cellarea.EndRow = 1;
            cellarea.EndColumn = 1;
            
            // Fügen Sie der Sammlung eine Validierung hinzu
            int index = sheet.Validations.Add(cellarea);
            Validation validation = sheet.Validations[index];
            
            // Validierungseinstellungen konfigurieren
            validation.Type = ValidationType.List;
            validation.Formula1 = "Yes,No";
            validation.AlertStyle = ValidationAlertType.Information;
            
            // Speichere die Arbeitsmappe
            workbook.Save("ValidationCollectionMethodAddWithCellAreaDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Siehe auch

* struct [CellArea](../../cellarea/)
* class [ValidationCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


