---
title: "Enum CellsUnitType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Aspose.Cells.CellsUnitType enum. Specifica l'unità di misura"
type: docs
url: /it/net/aspose.cells/cellsunittype/
---
## CellsUnitType enumeration

Specifica l'unità di misura.

```csharp
public enum CellsUnitType
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| Pixel | `1` | La misura è in pixel. |
| Point | `2` | La misura è in punti. Un punto rappresenta 1/72 di pollice. |
| Inch | `4` | La misura è in pollici. |
| Cm | `6` | La misura è in centimetri. |
| Character | `7` | In unità di caratteri. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsClassCellsUnitTypeDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook per la dimostrazione
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Dimostra l'uso di valori diversi dell'enumerazione CellsUnitType
                Console.WriteLine("Available CellsUnitType values:");

                // Visualizza tutti i valori dell'enumerazione
                Console.WriteLine("Pixel: " + CellsUnitType.Pixel);
                Console.WriteLine("Point: " + CellsUnitType.Point);
                Console.WriteLine("Inch: " + CellsUnitType.Inch);
                Console.WriteLine("Cm: " + CellsUnitType.Cm);
                Console.WriteLine("Character: " + CellsUnitType.Character);

                // Esempio di utilizzo: Imposta la larghezza della colonna usando unità diverse
                worksheet.Cells.SetColumnWidthPixel(0, 100); // Using Pixel unit
                worksheet.Cells.SetColumnWidthInch(1, 2.0);  // Using Inch unit

                // Salva la cartella di lavoro per dimostrare un flusso completo
                workbook.Save("CellsUnitTypeDemo.xlsx");
                Console.WriteLine("Workbook saved successfully with different unit types applied.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with CellsUnitType: {ex.Message}");
            }
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


