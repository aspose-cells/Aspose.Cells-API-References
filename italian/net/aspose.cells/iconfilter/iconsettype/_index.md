---
title: "IconFilter.IconSetType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà IconFilter. Ottiene e imposta quale set di icone è usato per questo criterio di filtro"
type: docs
url: /it/net/aspose.cells/iconfilter/iconsettype/
---
## IconFilter.IconSetType property

Ottiene e imposta quale set di icone è usato per questo criterio di filtro.

```csharp
public IconSetType IconSetType { get; set; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class IconFilterPropertyIconSetTypeDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Popola dati di esempio
            for (int i = 0; i < 10; i++)
            {
                worksheet.Cells[i, 0].PutValue(i * 10);
            }

            // Crea filtro automatico
            worksheet.AutoFilter.Range = "A1:A10";
            FilterColumn filterColumn = worksheet.AutoFilter.FilterColumns[0];
            filterColumn.FilterType = FilterType.IconFilter;

            // Ottieni il filtro icona
            IconFilter iconFilter = (IconFilter)filterColumn.Filter;

            // Visualizza l'IconSetType corrente (il valore predefinito è None)
            Console.WriteLine("Current IconSetType: " + iconFilter.IconSetType);

            // Imposta al set di icone a 3 frecce
            iconFilter.IconSetType = IconSetType.Arrows3;
            iconFilter.IconId = 1; // Show only middle arrow

            // Applica la formattazione condizionale per visualizzare le icone
            ConditionalFormattingCollection conditionalFormattings = worksheet.ConditionalFormattings;
            int index = conditionalFormattings.Add();
            FormatConditionCollection formatConditionCollection = conditionalFormattings[index];
            int conditionIndex = formatConditionCollection.AddCondition(FormatConditionType.IconSet);
            FormatCondition formatCondition = formatConditionCollection[conditionIndex];
            formatCondition.IconSet.Type = IconSetType.Arrows3;
            
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.EndRow = 9;
            area.StartColumn = 0;
            area.EndColumn = 0;
            formatConditionCollection.AddArea(area);

            // Cambia al set di icone semafori
            iconFilter.IconSetType = IconSetType.TrafficLights31;
            iconFilter.IconId = 2; // Show only green light

            // Salva il risultato
            workbook.Save("PropertyIconSetTypeDemo.xlsx");
        }
    }
}
```

### Vedi anche

* enum [IconSetType](../../iconsettype/)
* class [IconFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


