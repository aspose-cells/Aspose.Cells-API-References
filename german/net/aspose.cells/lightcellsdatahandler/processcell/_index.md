---
title: ProcessCell
second_title: Aspose.Cells für .NET-API-Referenz
description: Beginnt mit der Verarbeitung einer Zelle.
type: docs
weight: 10
url: /de/net/aspose.cells/lightcellsdatahandler/processcell/
---
## LightCellsDataHandler.ProcessCell method

Beginnt mit der Verarbeitung einer Zelle.

```csharp
public bool ProcessCell(Cell cell)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| cell | Cell | Zellobjekt, das gerade bearbeitet wird |

### Rückgabewert

ob diese Zelle im Zellenmodell des aktuellen Blatts aufbewahrt werden muss. Normalerweise sollte sie falsch sein, damit nicht alle Zellen nach der Verarbeitung im Speicher bleiben und dann gespeichert werden. Für einige spezielle Zwecke, z. B. wenn der Benutzer darauf zugreifen muss Einige Zellen später, nachdem die gesamte Arbeitsmappe verarbeitet wurde, der Benutzer kann diese Methode als wahr zurückgeben, um diese speziellen Zellen im Zellenmodell beizubehalten und später über APIs wie Cells[Zeile, Spalte]. auf sie zuzugreifen, wobei die Zellendaten jedoch in Zellen gehalten werden Das Modell benötigt mehr Speicher und wenn alle Zellen beibehalten werden, wird das Lesen der Vorlage file im LightCells-Modus mit dem Lesen auf normale Weise identisch sein.

### Bemerkungen

Es wird aufgerufen, nachdem die Daten einer Zelle gelesen wurden.

### Siehe auch

* class [Cell](../../cell)
* interface [LightCellsDataHandler](../../lightcellsdatahandler)
* namensraum [Aspose.Cells](../../lightcellsdatahandler)
* Montage [Aspose.Cells](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->