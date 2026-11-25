---
title: "Enum LoadDataFilterOptions"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Enum Aspose.Cells.LoadDataFilterOptions. Rappresenta le opzioni per filtrare i dati durante il caricamento della cartella di lavoro da un modello"
type: docs
url: /it/net/aspose.cells/loaddatafilteroptions/
---
## LoadDataFilterOptions enumeration

Rappresenta le opzioni per filtrare i dati durante il caricamento della cartella di lavoro da un modello.

```csharp
public enum LoadDataFilterOptions
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| None | `0` | Non caricare nulla per i dati del foglio |
| All | `2147483647` | Carica tutto |
| CellBlank | `1` | Carica le celle il cui valore è vuoto |
| CellString | `2` | Carica le celle il cui valore è una stringa |
| CellNumeric | `4` | Carica le celle il cui valore è numerico (inclusi data/ora) |
| CellError | `8` | Carica le celle il cui valore è errore |
| CellBool | `16` | Carica le celle il cui valore è booleano |
| CellValue | `31` | Carica solo i valori delle celle (tutti i tipi di valore) |
| Formula | `32` | Carica le formule delle celle. |
| CellData | `67108927` | Carica i dati delle celle includendo valori, formule e formattazione |
| Chart | `256` | Carica i grafici |
| Shape | `402653696` | Carica le forme |
| Drawing | `402653952` | Oggetti di disegno (inclusi Chart, Picture, OleObject e tutti gli altri oggetti di disegno) |
| MergedArea | `1024` | Carica le celle unite |
| ConditionalFormatting | `2048` | Carica la formattazione condizionale |
| DataValidation | `4096` | Carica le convalide dei dati |
| PivotTable | `8192` | Carica le tabelle pivot |
| Table | `16384` | Carica le tabelle |
| Hyperlinks | `32768` | Carica i collegamenti ipertestuali |
| SheetSettings | `65536` | Carica le impostazioni del foglio di lavoro |
| SheetData | `403701759` | Carica tutti i dati del foglio di lavoro, come dati delle celle, impostazioni, oggetti, ...ecc. |
| BookSettings | `1048576` | Carica le impostazioni della cartella di lavoro |
| Settings | `1114112` | Carica le impostazioni della cartella di lavoro e del foglio di lavoro |
| XmlMap | `2097152` | Carica XmlMap |
| Structure | `4194304` | Carica la struttura della cartella di lavoro |
| DocumentProperties | `8388608` | Carica le proprietà del documento |
| DefinedNames | `16777216` | Carica gli oggetti Name definiti |
| VBA | `33554432` | Carica i progetti VBA |
| Style | `67108864` | Carica gli stili per la formattazione delle celle |
| Picture | `134217728` | Carica le immagini |
| OleObject | `268435456` | Carica OleObjects |
| Revision | `536870912` | Carica i log di revisione |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class LoadDataFilterOptionsDemo
    {
        public static void LoadDataFilterOptionsExample()
        {
            // Crea una nuova istanza di LoadOptions
            LoadOptions loadOptions = new LoadOptions();

            // Crea un'implementazione personalizzata di LoadFilter
            loadOptions.LoadFilter = new CustomLoadFilter();

            // Carica la cartella di lavoro con le opzioni di caricamento specificate
            Workbook workbook = new Workbook("LoadDataFilterOptionsExample_original.xlsx", loadOptions);

            // Salva la cartella di lavoro per verificare i dati caricati
            workbook.Save("LoadDataFilterOptionsExample.xlsx");
        }

        // Implementazione personalizzata di LoadFilter
        private class CustomLoadFilter : LoadFilter
        {
            public override void StartSheet(Worksheet sheet)
            {
                // Applica diverse opzioni di filtro in base al nome del foglio
                if (sheet.Name == "Sheet1")
                {
                    LoadDataFilterOptions = LoadDataFilterOptions.All;
                }
                else
                {
                    LoadDataFilterOptions = LoadDataFilterOptions.Structure;
                }
            }
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


