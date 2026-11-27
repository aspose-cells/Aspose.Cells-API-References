---
title: "Enum AccessCacheOptions"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.AccessCacheOptions enum. Cachningsalternativ för dataåtkomst. Flera alternativ kan kombineras med operatorn."
type: docs
url: /sv/net/aspose.cells/accesscacheoptions/
---
## AccessCacheOptions enumeration

Cachealternativ för dataåtkomst. Flera alternativ kan kombineras med operatorn "&#x7C;".

```csharp
[Flags]
public enum AccessCacheOptions
```

### Värden

| Namn | Värde | Beskrivning |
| --- | --- | --- |
| None | `0` | Ingen cache för någon dataåtkomst. |
| All | `FFFFFFFFFFFFFFFF` | Tillämpa alla möjliga optimeringar för alla typer av dataåtkomst i arbetsboken. Alla inställningar och data får inte ändras under den optimerade åtkomsten. |
| PositionAndSize | `3` | Tillämpa möjlig optimering för att hämta ett objekts (t.ex. Shape) position och storlek. Inställningar för radhöjd och kolumnbredd får inte ändras under den optimerade åtkomsten. |
| CellsData | `9` | Tillämpa möjlig optimering för att hämta cellers värden. Celldata (data och inställningar för Cell, Row) får inte ändras under den optimerade åtkomsten, inga nya Cell/Row‑objekt ska skapas heller (t.ex. via [`Item`](../cells/item/)). |
| CellDisplay | `100086` | Tillämpa möjlig optimering för att hämta displayrelaterade resultat för celler([`DisplayStringValue`](../cell/displaystringvalue/), [`GetStyle`](../cell/getstyle/), [`GetDisplayStyle`](../cell/getdisplaystyle/), etc.). Celldata och stilrelaterade objekt (Cell/Row/Column‑stilar, kolumnbredd, etc.) får inte ändras under den optimerade åtkomsten. |
| GetFormula | `200000` | Tillämpa möjlig optimering för att hämta formler. All data och inställningar som kan påverka formeluttrycket (arbetsbladets namn, namnens text, tabellens kolumn, etc.) får inte ändras under den optimerade åtkomsten. |
| SetFormula | `400000` | Tillämpa möjlig optimering för att sätta formler. All data och inställningar som kan påverka formeluttrycket (arbetsbladets namn, namnens text, tabellens kolumn, etc.) får inte ändras under den optimerade åtkomsten. |
| CalculateFormula | `800009` | Tillämpa möjlig optimering för att beräkna formler. Celldata får inte ändras under den optimerade åtkomsten, inga nya objekt (Cell, Row, etc.) ska skapas heller (t.ex. via [`Item`](../cells/item/)). |
| ConditionalFormatting | `1000009` | Tillämpa möjlig optimering för att hämta formateringsresultat för villkorliga formateringar. All data och inställningar som kan påverka resultatet av villkorliga formateringar (inställningar för villkorliga formateringar, beroende cellvärden, etc.) får inte ändras under den optimerade åtkomsten. |
| Validation | `2000009` | Tillämpa möjlig optimering för att hämta valideringsresultat. All data och inställningar som kan påverka resultatet av validering (inställningar för valideringen, beroende cellvärden, etc.) får inte ändras under den optimerade åtkomsten. |

### Anmärkningar

För vissa funktioner kräver åtkomst till stora dataset många upprepade och komplicerade operationer såsom sökning, beräkning, ...etc och dessa operationer tar mycket extra tid. För vanliga situationer förblir all beroende data oförändrad under åtkomsten, så vissa cacheminnen kan byggas och användas för att förbättra åtkomstprestanda. För detta ändamål tillhandahåller vi detta API så att användaren kan ange vilken typ av dataåtkomst som bör optimeras med en möjlig cachemekanism. Observera att för olika alternativ kan olika dataset behöva vara "read-only". Och prestandan för dataåtkomst beror på många faktorer, användning av cachemekanism garanterar inte att prestandan förbättras. För vissa situationer, såsom när datasetet som ska nås är litet, kan användning av cache leda till ännu mer tid eftersom cachelagring själv också kräver viss extra tid.

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class AccessCacheOptionsDemo
    {
        public static void AccessCacheOptionsExample()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Starta åtkomstcache med specifika alternativ
            workbook.StartAccessCache(AccessCacheOptions.PositionAndSize | AccessCacheOptions.CellsData);

            // Utför några operationer som drar nytta av cachning
            for (int i = 0; i < 10; i++)
            {
                for (int j = 0; j < 10; j++)
                {
                    worksheet.Cells[i, j].PutValue(i + j);
                }
            }

            // Stäng åtkomstcache
            workbook.CloseAccessCache(AccessCacheOptions.PositionAndSize | AccessCacheOptions.CellsData);

            // Spara arbetsboken
            workbook.Save("AccessCacheOptionsExample.xlsx");
        }
    }
}
```

### Se även

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


