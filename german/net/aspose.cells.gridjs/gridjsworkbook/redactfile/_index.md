---
title: "GridJsWorkbook.RedactFile"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "GridJsWorkbook-Methode. Führt eine Redaktion einer Excel-Datei basierend auf einem Array von JSON-Operationen durch."
type: docs
url: /de/net/aspose.cells.gridjs/gridjsworkbook/redactfile/
---
## GridJsWorkbook.RedactFile method

Führt eine Redaktion einer Excel-Datei basierend auf einem Array von JSON-Operationen durch.

```csharp
public void RedactFile(string excelFilePath, string uid, string[] arrayOfRedactionOpr)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| excelDateipfad | String | Der Dateipfad der zu redigierenden Excel-Datei. |
| uid | String | Der eindeutige Bezeichner für das Arbeitsbuch. Wenn null oder leer, wird eine neue UID basierend auf dem Dateipfad generiert. |
| arrayOfRedactionOpr | String[] | Ein Array von JSON-Zeichenketten, das die anzuwendenden Redaktionsoperationen darstellt. |

### Ausnahmen

| Ausnahme | Bedingung |
| --- | --- |
| [GridCellException](../../gridcellexception/) | Wird ausgelöst, wenn während der Redaktionsoperation eine CellsException auftritt. |
| Ausnahme | Wird ausgelöst, wenn während der Redaktionsoperation eine allgemeine Ausnahme auftritt. |

### Siehe auch

* class [GridJsWorkbook](../)
* namespace [Aspose.Cells.GridJs](../../../aspose.cells.gridjs/)
* assembly [Aspose.Cells.GridJs](../../../)


