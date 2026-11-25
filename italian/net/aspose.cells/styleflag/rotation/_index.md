---
title: "StyleFlag.Rotation"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà StyleFlag. L'impostazione Rotation verrà applicata"
type: docs
url: /it/net/aspose.cells/styleflag/rotation/
---
## StyleFlag.Rotation property

L'impostazione di rotazione sarà applicata.

```csharp
public bool Rotation { get; set; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class StyleFlagPropertyRotationDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Accedi alla cella A1 e imposta del testo
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Rotated Text");

            // Ottieni lo stile della cella
            Style style = workbook.CreateStyle();

            // Imposta nuovo valore di rotazione (45 gradi)
            style.RotationAngle = 45;

            // Mostra valore di rotazione corrente
            Console.WriteLine("Current Rotation value: " + cell.GetStyle().RotationAngle);            

            // Crea un flag di stile e abilita il flag di rotazione
            StyleFlag styleFlag = new StyleFlag();
            styleFlag.Rotation = true;

            // Applica lo stile con rotazione alla cella
            cell.SetStyle(style, styleFlag);

            Console.WriteLine("after setting style, rotation value: " + cell.GetStyle().RotationAngle);
           
            // Salva il risultato
            workbook.Save("PropertyRotationDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [StyleFlag](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


