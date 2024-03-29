---
title: IsParamLiteralRequired
second_title: Aspose.Cells für .NET-API-Referenz
description: Gibt an ob diese Engine während der Berechnung den wörtlichen Text des Parameters benötigt. Der Standardwert ist false.
type: docs
weight: 10
url: /de/net/aspose.cells/abstractcalculationengine/isparamliteralrequired/
---
## AbstractCalculationEngine.IsParamLiteralRequired property

Gibt an, ob diese Engine während der Berechnung den wörtlichen Text des Parameters benötigt. Der Standardwert ist false.

```csharp
public virtual bool IsParamLiteralRequired { get; }
```

### Bemerkungen

Wenn diese benutzerdefinierte Berechnungsmaschine den wörtlichen Text des Parameters benötigt, werden mehr Stacks benötigt, um den wörtlichen Text für Parameter zwischenzuspeichern, und die Methode Calculate() kann rekursiv aufgerufen werden, um den Wert des Parameters zu berechnen. Normalerweise wird der wörtliche Text nicht zum Berechnen von Formeln benötigt und Diese Methode sollte für die meisten Implementierungen false zurückgeben, um eine bessere Leistung zu erzielen.

### Siehe auch

* class [AbstractCalculationEngine](../../abstractcalculationengine)
* namensraum [Aspose.Cells](../../abstractcalculationengine)
* Montage [Aspose.Cells](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
