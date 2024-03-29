---
title: CalcStackSize
second_title: Aspose.Cells für .NET-API-Referenz
description: Gibt die Stapelgröße für die rekursive Berechnung von Zellen an.
type: docs
weight: 20
url: /de/net/aspose.cells/calculationoptions/calcstacksize/
---
## CalculationOptions.CalcStackSize property

Gibt die Stapelgröße für die rekursive Berechnung von Zellen an.

```csharp
public int CalcStackSize { get; set; }
```

### Bemerkungen

Wenn eine große Anzahl von Zellen rekursiv in der Abhängigkeitsstruktur berechnet werden muss, kann eine StackOverflowException im Berechnungsprozess verursacht werden. Wenn ja, sollte der Benutzer einen kleineren Wert für diese Eigenschaft angeben. Für eine solche Situation sollte der Benutzer den bestimmen richtiger Wert für diese Eigenschaft gemäß den tatsächlichen Formeln und Daten. Ein zu kleiner Wert kann zu Leistungseinbußen bei der Formelberechnung führen.

### Siehe auch

* class [CalculationOptions](../../calculationoptions)
* namensraum [Aspose.Cells](../../calculationoptions)
* Montage [Aspose.Cells](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
