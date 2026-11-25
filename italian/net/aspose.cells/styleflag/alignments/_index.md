---
title: "StyleFlag.Alignments"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà StyleFlag. L'impostazione di allineamento verrà applicata"
type: docs
url: /it/net/aspose.cells/styleflag/alignments/
---
## StyleFlag.Alignments property

L'impostazione di allineamento verrà applicata.

```csharp
public bool Alignments { get; set; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class StyleFlagPropertyAlignmentsDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Accedi alla cella A1 e imposta del testo
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Sample Text");

            // Crea un oggetto stile e imposta le proprietà di allineamento
            Style style = workbook.CreateStyle();
            style.HorizontalAlignment = TextAlignmentType.Center;
            style.VerticalAlignment = TextAlignmentType.Center;
            style.RotationAngle = 45;

            // Crea un flag di stile e abilita le proprietà di allineamento
            StyleFlag styleFlag = new StyleFlag();
            styleFlag.Alignments = true;

            // Applica lo stile alla cella con il flag di stile
            cell.SetStyle(style, styleFlag);

            // Mostra le impostazioni di allineamento attuali
            Console.WriteLine("Horizontal Alignment: " + cell.GetStyle().HorizontalAlignment);
            Console.WriteLine("Vertical Alignment: " + cell.GetStyle().VerticalAlignment);
            Console.WriteLine("Rotation: " + cell.GetStyle().RotationAngle);

            // Modifica il flag di stile per disabilitare le proprietà di allineamento
            styleFlag.Alignments = false;
            
            // Crea un nuovo stile con un allineamento diverso
            Style newStyle = workbook.CreateStyle();
            newStyle.HorizontalAlignment = TextAlignmentType.Right;
            newStyle.VerticalAlignment = TextAlignmentType.Top;
            newStyle.RotationAngle = 0;

            // Applica il nuovo stile - gli allineamenti non cambieranno perché il flag è false
            cell.SetStyle(newStyle, styleFlag);

            // Mostra le impostazioni di allineamento non modificate
            Console.WriteLine("After applying new style with Alignments=false:");
            Console.WriteLine("Horizontal Alignment: " + cell.GetStyle().HorizontalAlignment);
            Console.WriteLine("Vertical Alignment: " + cell.GetStyle().VerticalAlignment);
            Console.WriteLine("Rotation: " + cell.GetStyle().RotationAngle);

            // Salva la cartella di lavoro
            workbook.Save("StyleFlagAlignmentsDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [StyleFlag](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


