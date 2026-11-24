---
title: "Enum AccessCacheOptions"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.AccessCacheOptions enum. Caching-Optionen für den Datenzugriff. Mehrere Optionen können mithilfe des Operators kombiniert werden."
type: docs
url: /de/net/aspose.cells/accesscacheoptions/
---
## AccessCacheOptions enumeration

Cache‑Optionen für den Datenzugriff. Mehrere Optionen können mit dem Operator "&#x7C;" kombiniert werden.

```csharp
[Flags]
public enum AccessCacheOptions
```

### Werte

| Name | Wert | Beschreibung |
| --- | --- | --- |
| None | `0` | Kein Cache für irgendeinen Datenzugriff. |
| All | `FFFFFFFFFFFFFFFF` | Wende alle möglichen Optimierungen für alle Arten des Datenzugriffs in der Arbeitsmappe an. Alle Einstellungen und Daten dürfen während des optimierten Zugriffs nicht geändert werden. |
| PositionAndSize | `3` | Wende mögliche Optimierung für das Abrufen der Position und Größe von Objekten (wie Shape) an. Zeilenhöhen- und Spaltenbreiteneinstellungen dürfen während des optimierten Zugriffs nicht geändert werden. |
| CellsData | `9` | Wende mögliche Optimierung für das Abrufen von Zellwerten an. Zellen­daten (Daten und Einstellungen von Cell, Row) dürfen während des optimierten Zugriffs nicht geändert werden, es dürfen auch keine neuen Cell/Row‑Objekte erstellt werden (z. B. durch [`Item`](../cells/item/)). |
| CellDisplay | `100086` | Wende mögliche Optimierung für das Abrufen von anzeigerelevanten Ergebnissen von Zellen ([`DisplayStringValue`](../cell/displaystringvalue/), [`GetStyle`](../cell/getstyle/), [`GetDisplayStyle`](../cell/getdisplaystyle/), usw.) an. Zellen­daten und stilbezogene Objekte (Cell/Row/Column‑Stile, Spaltenbreite usw.) dürfen während des optimierten Zugriffs nicht geändert werden. |
| GetFormula | `200000` | Wende mögliche Optimierung für das Abrufen von Formeln an. Alle Daten und Einstellungen, die den Formelausdruck beeinflussen können (Arbeitsblattname, Name‑Text, Tabellenspalte usw.), dürfen während des optimierten Zugriffs nicht geändert werden. |
| SetFormula | `400000` | Wende mögliche Optimierung für das Festlegen von Formeln an. Alle Daten und Einstellungen, die den Formelausdruck beeinflussen können (Arbeitsblattname, Name‑Text, Tabellenspalte usw.), dürfen während des optimierten Zugriffs nicht geändert werden. |
| CalculateFormula | `800009` | Wende mögliche Optimierung für das Berechnen von Formeln an. Zellen­daten dürfen während des optimierten Zugriffs nicht geändert werden, es dürfen auch keine neuen Objekte (Cell, Row usw.) erstellt werden (z. B. durch [`Item`](../cells/item/)). |
| ConditionalFormatting | `1000009` | Wende mögliche Optimierung für das Abrufen von Formatierungsergebnissen bedingter Formatierungen an. Alle Daten und Einstellungen, die das Ergebnis bedingter Formatierungen beeinflussen können (Einstellungen der bedingten Formatierungen, abhängige Zellwerte usw.), dürfen während des optimierten Zugriffs nicht geändert werden. |
| Validation | `2000009` | Wende mögliche Optimierung für das Abrufen von Validierungsergebnissen an. Alle Daten und Einstellungen, die das Ergebnis der Validierung beeinflussen können (Einstellungen der Validierung, abhängige Zellwerte usw.), dürfen während des optimierten Zugriffs nicht geändert werden. |

### Hinweise

Für einige Funktionen erfordert der Zugriff auf große Datensätze viele wiederholte und komplizierte Vorgänge wie Suche, Berechnung, ...etc, und diese Vorgänge benötigen zusätzliche Zeit. In üblichen Situationen bleiben alle abhängigen Daten während des Zugriffs unverändert, sodass einige Caches erstellt und verwendet werden können, um die Zugriffsleistung zu verbessern. Zu diesem Zweck stellen wir diese API bereit, damit der Benutzer angeben kann, welche Art von Datenzugriff durch einen möglichen Caching‑Mechanismus optimiert werden soll. Bitte beachten Sie, dass für unterschiedliche Optionen unterschiedliche Datensätze möglicherweise "read-only" sein müssen. Und die Leistung des Datenzugriffs hängt von vielen Aspekten ab; die Verwendung eines Caching‑Mechanismus garantiert nicht, dass die Leistung verbessert wird. In manchen Situationen, z. B. wenn der zuzugreifende Datensatz klein ist, kann die Nutzung eines Caches sogar mehr Zeit beanspruchen, da das Caching selbst ebenfalls zusätzlichen Aufwand erfordert.

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class AccessCacheOptionsDemo
    {
        public static void AccessCacheOptionsExample()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Starten Sie den Zugriffs‑Cache mit spezifischen Optionen
            workbook.StartAccessCache(AccessCacheOptions.PositionAndSize | AccessCacheOptions.CellsData);

            // Führen Sie einige Vorgänge aus, die vom Caching profitieren
            for (int i = 0; i < 10; i++)
            {
                for (int j = 0; j < 10; j++)
                {
                    worksheet.Cells[i, j].PutValue(i + j);
                }
            }

            // Zugriffs‑Cache schließen
            workbook.CloseAccessCache(AccessCacheOptions.PositionAndSize | AccessCacheOptions.CellsData);

            // Speichere die Arbeitsmappe
            workbook.Save("AccessCacheOptionsExample.xlsx");
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


