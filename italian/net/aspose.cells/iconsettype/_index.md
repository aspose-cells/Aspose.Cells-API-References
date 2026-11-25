---
title: "Enumerazione IconSetType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Enum Aspose.Cells.IconSetType. Tipo di set di icone per la formattazione condizionale. I valori soglia per attivare le diverse icone all'interno di un set sono configurabili e l'ordine delle icone è reversibile"
type: docs
url: /it/net/aspose.cells/iconsettype/
---
## IconSetType enumeration

Tipo di set di icone per la formattazione condizionale. I valori soglia per attivare le diverse icone all'interno di un set sono configurabili e l'ordine delle icone è invertibile.

```csharp
public enum IconSetType
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| Arrows3 | `0` | Set di icone 3 frecce. |
| ArrowsGray3 | `1` | Set di icone 3 frecce grigie. |
| Flags3 | `2` | Set di icone 3 bandiere. |
| Signs3 | `3` | Set di icone 3 segni. |
| Symbols3 | `4` | Set di icone 3 simboli (cerchiati). |
| Symbols32 | `5` | Set di icone 3 simboli (non cerchiati). |
| TrafficLights31 | `6` | Set di icone 3 semafori (senza bordo). |
| TrafficLights32 | `7` | Set di icone 3 semafori con bordo spesso nero. |
| Arrows4 | `8` | Set di icone 4 frecce. |
| ArrowsGray4 | `9` | Set di icone 4 frecce grigie. |
| Rating4 | `10` | Set di icone 4 valutazioni. |
| RedToBlack4 | `11` | Set di icone 4 'rosso a nero'. |
| TrafficLights4 | `12` | Set di icone 4 semafori. |
| Arrows5 | `13` | Set di icone con 5 frecce. |
| ArrowsGray5 | `14` | Set di icone con 5 frecce grigie. |
| Quarters5 | `15` | Set di icone con 5 quarti. |
| Rating5 | `16` | Set di icone di valutazione a 5. |
| Stars3 | `17` | Set di 3 stelle |
| Boxes5 | `18` | Set di 5 scatole |
| Triangles3 | `19` | Set di 3 triangoli |
| None | `20` | Nessuno |
| CustomSet | `21` | CustomSet. Questo elemento è di sola lettura. |
| Smilies3 | `22` | 3 emoticon. Solo per .ods. |
| ColorSmilies3 | `23` | 3 emoticon colorate. Solo per .ods. |

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassIconSetTypeDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            Cells cells = sheet.Cells;

            // Imposta valori di esempio
            cells["A1"].PutValue(1);
            cells["A2"].PutValue("#DIV/0!");
            cells["A3"].PutValue(3);

            // Aggiungi formattazione condizionale con set di icone
            ConditionalFormattingCollection cfs = sheet.ConditionalFormattings;
            FormatConditionCollection fcs = cfs[cfs.Add()];
            fcs.AddArea(CellArea.CreateCellArea(0, 0, 3, 0));
            
            FormatCondition fc = fcs[fcs.AddCondition(FormatConditionType.IconSet)];
            fc.IconSet.Type = IconSetType.TrafficLights31;

            // Ottieni e visualizza i risultati
            ConditionalFormattingResult res1 = cells["A1"].GetConditionalFormattingResult();
            Console.WriteLine($"A1 Icon Type: {res1.ConditionalFormattingIcon.Type}, Index: {res1.ConditionalFormattingIcon.Index}");

            ConditionalFormattingResult res3 = cells["A3"].GetConditionalFormattingResult();
            Console.WriteLine($"A3 Icon Type: {res3.ConditionalFormattingIcon.Type}, Index: {res3.ConditionalFormattingIcon.Index}");

            ConditionalFormattingResult res2 = cells["A2"].GetConditionalFormattingResult();
            Console.WriteLine($"A2 has formatting: {res2 != null && res2.ConditionalFormattingIcon != null}");
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


