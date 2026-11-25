---
title: "IconSet.Reverse"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà IconSet. Ottieni o imposta il flag che indica se invertire l'ordine predefinito delle icone in questo set di icone. Il valore predefinito è false"
type: docs
url: /it/net/aspose.cells/iconset/reverse/
---
## IconSet.Reverse property

Ottieni o imposta il flag che indica se invertire l'ordine predefinito delle icone in questo set di icone. Il valore predefinito è false.

```csharp
public bool Reverse { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class IconSetPropertyReverseDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].PutValue(30);
            worksheet.Cells["A4"].PutValue(40);
            worksheet.Cells["A5"].PutValue(50);

            // Aggiungi formattazione condizionale
            ConditionalFormattingCollection cfs = worksheet.ConditionalFormattings;
            int index = cfs.Add();
            FormatConditionCollection cf = cfs[index];
            
            // Imposta l'intervallo
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.EndRow = 4;
            area.StartColumn = 0;
            area.EndColumn = 0;
            cf.AddArea(area);

            // Crea formattazione condizionale per il set di icone
            cf.AddCondition(FormatConditionType.IconSet);
            IconSet iconSet = cf[0].IconSet;
            
            // Configura il set di icone
            iconSet.Type = IconSetType.Arrows3;
            iconSet.ShowValue = true;
            
            // Dimostra la proprietà Reverse
            Console.WriteLine("Original IconSet Reverse value: " + iconSet.Reverse);
            iconSet.Reverse = true;
            Console.WriteLine("Modified IconSet Reverse value: " + iconSet.Reverse);

            // Salva la cartella di lavoro
            workbook.Save("IconSetPropertyReverseDemo_out.xlsx");
        }
    }
}
```

### Vedi anche

* class [IconSet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


