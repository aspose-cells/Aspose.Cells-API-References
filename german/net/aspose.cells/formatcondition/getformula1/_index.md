---
title: GetFormula1
second_title: Aspose.Cells für .NET-API-Referenz
description: Ruft den Wert oder Ausdruck ab der dieser Formatbedingung zugeordnet ist.
type: docs
weight: 150
url: /de/net/aspose.cells/formatcondition/getformula1/
---
## GetFormula1(bool, bool) {#getformula1}

Ruft den Wert oder Ausdruck ab, der dieser Formatbedingung zugeordnet ist.

```csharp
public string GetFormula1(bool isR1C1, bool isLocal)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| isR1C1 | Boolean | Ob die Formel als R1C1 formatiert werden muss. |
| isLocal | Boolean | Ob die Formel nach Gebietsschema formatiert werden muss. |

### Rückgabewert

Der Wert oder Ausdruck, der dieser Formatbedingung zugeordnet ist.

### Siehe auch

* class [FormatCondition](../../formatcondition)
* namensraum [Aspose.Cells](../../formatcondition)
* Montage [Aspose.Cells](../../../)

---

## GetFormula1(bool, bool, int, int) {#getformula1_1}

Ruft den Wert oder Ausdruck der bedingten Formatierung der Zelle ab.

```csharp
public string GetFormula1(bool isR1C1, bool isLocal, int row, int column)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| isR1C1 | Boolean | Ob die Formel als R1C1 formatiert werden muss. |
| isLocal | Boolean | Ob die Formel nach Gebietsschema formatiert werden muss. |
| row | Int32 | Der Zeilenindex. |
| column | Int32 | Der Spaltenindex. |

### Rückgabewert

Der Wert oder Ausdruck, der der bedingten Formatierung der Zelle zugeordnet ist.

### Bemerkungen

Die angegebene Zelle muss in dieser bedingten Formatierung enthalten sein, andernfalls wird null zurückgegeben.

### Siehe auch

* class [FormatCondition](../../formatcondition)
* namensraum [Aspose.Cells](../../formatcondition)
* Montage [Aspose.Cells](../../../)

---

## GetFormula1(int, int) {#getformula1_2}

Ruft die Formel der bedingten Formatierung der Zelle ab.

```csharp
public string GetFormula1(int row, int column)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| row | Int32 | Der Zeilenindex. |
| column | Int32 | Der Spaltenindex. |

### Rückgabewert

Die Formel.

### Siehe auch

* class [FormatCondition](../../formatcondition)
* namensraum [Aspose.Cells](../../formatcondition)
* Montage [Aspose.Cells](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->