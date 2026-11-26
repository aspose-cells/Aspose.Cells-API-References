---
title: "Style.NumberType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Style. Obtiene o establece el formato de visualización de números y fechas. Los patrones de formato son diferentes para distintas regiones"
type: docs
url: /es/net/aspose.cells.griddesktop/style/numbertype/
---
## Style.NumberType property

Obtiene o establece el formato de visualización de números y fechas. Los patrones de formato son diferentes según la región.

```csharp
public int NumberType { get; set; }
```

### Observaciones

Por ejemplo, los patrones de formato representados por números para la región en_US:

| **Value** | **Type** | **Format String** |
| --- | --- | --- |
| 0 | General | `General` |
| 1 | Decimal | `0` |
| 2 | Decimal | `0.00` |
| 3 | Decimal | `#,##0` |
| 4 | Decimal | `#,##0.00` |
| 5 | Currency | `$#,##0_);($#,##0)` |
| 6 | Currency | `$#,##0_);[Red]($#,##0)` |
| 7 | Currency | `$#,##0.00_);($#,##0.00)` |
| 8 | Currency | `$#,##0.00_);[Red]($#,##0.00)` |
| 9 | Percentage | `0%` |
| 10 | Percentage | `0.00%` |
| 11 | Scientific | `0.00E+00` |
| 12 | Fraction | `# ?/?` |
| 13 | Fraction | `# ??/??` |
| 14 | Date | `m/d/yyyy` |
| 15 | Date | `d-mmm-yy` |
| 16 | Date | `d-mmm` |
| 17 | Date | `mmm-yy` |
| 18 | Time | `h:mm AM/PM` |
| 19 | Time | `h:mm:ss AM/PM` |
| 20 | Time | `h:mm` |
| 21 | Time | `h:mm:ss` |
| 22 | Time | `m/d/yyyy h:mm` |
| 37 | Accounting | `#,##0_);(#,##0)` |
| 38 | Accounting | `#,##0_);[Red](#,##0)` |
| 39 | Accounting | `#,##0.00_);(#,##0.00)` |
| 40 | Accounting | `#,##0.00_);[Red](#,##0.00)` |
| 41 | Accounting | `_(* #,##0_);_(* (#,##0);_(* \"-\"_);_(@_)` |
| 42 | Currency | `_($* #,##0_);_($* (#,##0);_($* \"-\"_);_(@_)` |
| 43 | Accounting | `_(* #,##0.00_);_(* (#,##0.00);_(* \"-\"??_);_(@_)` |
| 44 | Currency | `_($* #,##0.00_);_($* (#,##0.00);_($* \"-\"??_);_(@_)` |
| 45 | Time | `mm:ss` |
| 46 | Time | `[h]:mm:ss` |
| 47 | Time | `mm:ss.0` |
| 48 | Scientific | `##0.0E+0` |
| 49 | Text | `@` |

### Ver también

* class [Style](../)
* namespace [Aspose.Cells.GridDesktop](../../../aspose.cells.griddesktop/)
* assembly [Aspose.Cells.GridDesktop](../../../)


