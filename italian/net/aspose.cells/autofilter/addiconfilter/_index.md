---
title: "AutoFilter.AddIconFilter"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo AutoFilter. Aggiunge un filtro icona"
type: docs
url: /it/net/aspose.cells/autofilter/addiconfilter/
---
## AutoFilter.AddIconFilter method

Aggiunge un filtro icona.

```csharp
public void AddIconFilter(int fieldIndex, IconSetType iconSetType, int iconId)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| fieldIndex | Int32 | L'offset intero del campo su cui si desidera basare il filtro (da sinistra dell'elenco; il campo più a sinistra è il campo 0). |
| iconSetType | IconSetType | Il tipo di set di icone. |
| iconId | Int32 | L'ID dell'icona. |

### Osservazioni

Supporta solo l'aggiunta del filtro icona. Non supporta il controllo di quale riga è visibile se il filtro è un filtro icona.

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class AutoFilterMethodAddIconFilterWithInt32IconSetTypeInt32Demo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Popola dati di esempio nella colonna A
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Values");
            worksheet.Cells["A2"].PutValue(10);
            worksheet.Cells["A3"].PutValue(20);
            worksheet.Cells["A4"].PutValue(30);
            worksheet.Cells["A5"].PutValue(40);
            worksheet.Cells["A6"].PutValue(50);
            cell = worksheet.Cells["B1"];
            cell.PutValue("Values2");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);
            worksheet.Cells["B5"].PutValue(40);
            worksheet.Cells["B6"].PutValue(50);

            ConditionalFormattingCollection cfs = worksheet.ConditionalFormattings;
            FormatConditionCollection fcs = cfs[cfs.Add()];
            fcs.AddArea(CellArea.CreateCellArea(1, 0, 5, 1));
            FormatCondition fc = fcs[fcs.AddCondition(FormatConditionType.IconSet)];

            // Ottieni l'istanza del filtro automatico
            AutoFilter autoFilter = worksheet.AutoFilter;
            
            // Imposta l'intervallo del filtro automatico (A1:A6) usando startRow, startColumn, endRow
            autoFilter.SetRange(0, 0, 1);

            try
            {
                // Aggiungi filtro icona alla prima colonna (fieldIndex: 0)
                // Utilizzando il set di icone 3 Traffic Lights (IconSetType.TrafficLights31)
                // Filtraggio per la prima icona nel set (iconId: 0)
                autoFilter.AddIconFilter(0, IconSetType.TrafficLights31, 0);
                
                // Aggiorna il filtro per applicare le modifiche
                autoFilter.Refresh();

                Console.WriteLine("Added icon filter to column A showing items with first traffic light icon");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing AddIconFilter: {ex.Message}");
            }

            // Salva la cartella di lavoro modificata
            workbook.Save("AutoFilterMethodAddIconFilterWithInt32IconSetTypeInt32Demo.xlsx");
        }
    }
}
```

### Vedi anche

* enum [IconSetType](../../iconsettype/)
* class [AutoFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


