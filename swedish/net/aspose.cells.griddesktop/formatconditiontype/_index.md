---
title: "Enum FormatConditionType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.GridDesktop.FormatConditionType enum. Typ av villkorsformatregel"
type: docs
url: /sv/net/aspose.cells.griddesktop/formatconditiontype/
---
## FormatConditionType enumeration

Villkorlig formatregeltyp.

```csharp
public enum FormatConditionType
```

### Värden

| Namn | Värde | Beskrivning |
| --- | --- | --- |
| CellValue | `0` | Denna villkorsformateringsregel jämför ett cellvärde med ett formelberäknat resultat med hjälp av en operator. |
| Expression | `1` | Denna villkorsformateringsregel innehåller en formel att utvärdera. När formelresultatet är sant markeras cellen. |
| ColorScale | `2` | Denna villkorsformateringsregel skapar en graderad färgskala på cellerna. |
| DataBar | `3` | Denna villkorsformateringsregel visar en graderad datastapel i cellintervallet. |
| IconSet | `4` | Denna villkorsformateringsregel tillämpar ikoner på celler enligt deras värden. |
| Top10 | `5` | Denna villkorsformateringsregel markerar celler vars värden faller inom de översta N eller nedersta N intervallen, enligt specifikationen. |
| UniqueValues | `6` | Denna villkorsformateringsregel markerar unika värden i intervallet. |
| DuplicateValues | `7` | Denna villkorsformateringsregel markerar duplicerade värden. |
| ContainsText | `8` | Denna villkorsformateringsregel markerar celler som innehåller given text. Motsvarande att använda bladfunktionen SEARCH() för att avgöra om cellen innehåller texten. |
| NotContainsText | `9` | Denna villkorsformateringsregel markerar celler som inte är tomma. Motsvarande att använda LEN(TRIM()). Detta betyder att om cellen endast innehåller tecken som TRIM() skulle ta bort, betraktas den som tom. En tom cell betraktas också som tom. |
| BeginsWith | `10` | Denna villkorsformateringsregel markerar celler i intervallet som börjar med given text. Motsvarande att använda bladfunktionen LEFT() och jämföra värden. |
| EndsWith | `11` | Denna villkorsformateringsregel markerar celler som slutar med given text. Motsvarande att använda bladfunktionen RIGHT() och jämföra värden. |
| ContainsBlanks | `12` | Denna villkorsformateringsregel markerar celler som är helt tomma. Motsvarande att använda LEN(TRIM()). Detta betyder att om cellen endast innehåller tecken som TRIM() skulle ta bort, betraktas den som tom. En tom cell betraktas också som tom. |
| NotContainsBlanks | `13` | Denna villkorsformateringsregel markerar celler som inte är tomma. Motsvarande att använda LEN(TRIM()). Detta betyder att om cellen endast innehåller tecken som TRIM() skulle ta bort, betraktas den som tom. En tom cell betraktas också som tom. |
| ContainsErrors | `14` | Denna villkorsformateringsregel markerar celler med formelfel. Motsvarande att använda bladfunktionen ISERROR() för att avgöra om det finns ett formelfel. |
| NotContainsErrors | `15` | Denna villkorsformateringsregel markerar celler utan formelfel. Motsvarande att använda bladfunktionen ISERROR() för att avgöra om det finns ett formelfel. |
| TimePeriod | `16` | Denna villkorsformateringsregel markerar celler som innehåller datum under den angivna tidsperioden. Cellens underliggande värde utvärderas, därför behöver cellen inte vara formaterad som ett datum för att utvärderas. Till exempel, med en cell som innehåller värdet 38913 ska den villkorsstyrda formateringen tillämpas om regeln kräver ett värde av 7/14/2006. |
| AboveAverage | `17` | Denna villkorsformateringsregel markerar celler som ligger över eller under genomsnittet för alla värden i intervallet. |

### Se även

* namespace [Aspose.Cells.GridDesktop](../../aspose.cells.griddesktop/)
* assembly [Aspose.Cells.GridDesktop](../../)


