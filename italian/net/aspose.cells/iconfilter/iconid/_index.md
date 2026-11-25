---
title: "IconFilter.IconId"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà IconFilter. Ottiene e imposta l'indice basato su zero di un'icona in un set di icone"
type: docs
url: /it/net/aspose.cells/iconfilter/iconid/
---
## IconFilter.IconId property

Ottiene e imposta l'indice basato su zero di un'icona in un set di icone.

```csharp
public int IconId { get; set; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class IconFilterPropertyIconIdDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Popola dati di esempio
            for (int i = 0; i < 10; i++)
            {
                worksheet.Cells[i, 0].PutValue(i + 1);
            }

            // Applica la formattazione condizionale del set di icone
            ConditionalFormattingCollection conditionalFormattings = worksheet.ConditionalFormattings;
            int index = conditionalFormattings.Add();
            FormatConditionCollection formatConditionCollection = conditionalFormattings[index];
            int conditionIndex = formatConditionCollection.AddCondition(FormatConditionType.IconSet);
            FormatCondition formatCondition = formatConditionCollection[conditionIndex];
            formatCondition.IconSet.Type = IconSetType.TrafficLights31;
            
            // Imposta l'intervallo usando CellArea
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.EndRow = 9;
            area.StartColumn = 0;
            area.EndColumn = 0;
            formatConditionCollection.AddArea(area);

            // Crea un filtro automatico con filtro icona
            worksheet.AutoFilter.Range = "A1:A10";
            FilterColumn filterColumn = worksheet.AutoFilter.FilterColumns[0];
            filterColumn.FilterType = FilterType.IconFilter;
            
            // Ottieni il filtro esistente invece di creare una nuova istanza
            IconFilter iconFilter = (IconFilter)filterColumn.Filter;
            iconFilter.IconSetType = IconSetType.TrafficLights31;
            iconFilter.IconId = 0;

            Console.WriteLine("Current IconId value: " + iconFilter.IconId);

            // Modifica IconId per filtrare icone diverse
            iconFilter.IconId = 1;

            workbook.Save("PropertyIconIdDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [IconFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


