---
title: "Cell.GetLeafs"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Cell-metod. Hämta alla celler som refererar till denna cell direkt och som måste uppdateras när cellen ändras"
type: docs
url: /sv/net/aspose.cells/cell/getleafs/
---
## GetLeafs() {#getleafs}

Hämta alla celler som refererar till denna cell direkt och som måste uppdateras när cellen ändras.

```csharp
[Obsolete("Use GetDependentsInCalculation(bool) instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public IEnumerator GetLeafs()
```

### Returvärde

Enumerator för att enumerera alla beroende celler (Cell)

### Anmärkningar

OBS: Den här klassen är nu föråldrad. Använd istället Cell.GetDependentsInCalculation(bool) för att hämta alla beroenden i beräkningskedjan. Den här egenskapen kommer att tas bort 12 månader senare från och med maj 2022. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Collections;

    public class CellMethodGetLeafsDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till lite data och formler för att skapa beroenden
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["B1"].Formula = "=A1+A2";
            worksheet.Cells["C1"].Formula = "=B1*2";

            try
            {
                // Hämta cellen som har beroenden
                Cell cell = worksheet.Cells["B1"];

                // Anropa GetLeafs för att hämta alla celler som refererar till den här cellen direkt
                IEnumerator leafs = cell.GetLeafs();

                Console.WriteLine("Cells that directly reference B1:");
                while (leafs.MoveNext())
                {
                    Cell leafCell = leafs.Current as Cell;
                    if (leafCell != null)
                    {
                        Console.WriteLine($"Cell: {leafCell.Name}, Formula: {leafCell.Formula}");
                    }
                }

                // Spara arbetsboken
                workbook.Save("GetLeafsDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling GetLeafs: {ex.Message}");
            }
        }
    }
}
```

### Se även

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetLeafs(bool) {#getleafs_1}

Hämta alla celler som kommer att uppdateras när den här cellen ändras.

```csharp
[Obsolete("Use GetDependentsInCalculation(bool) instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public IEnumerator GetLeafs(bool recursive)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| rekursiv | Boolean | Anger om de löv som inte refererar till den här cellen direkt men refererar till andra löv för den här cellen returneras |

### Returvärde

Enumerator för att enumerera alla beroende celler (Cell)

### Anmärkningar

OBS: Den här klassen är nu föråldrad. Använd istället Cell.GetDependentsInCalculation(bool) för att hämta alla beroenden i beräkningskedjan. Den här egenskapen kommer att tas bort 12 månader senare från och med maj 2022. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Collections;

    public class CellMethodGetLeafsWithBooleanDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();

            // Åtkomst till det första kalkylbladet
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till lite data med formler för att skapa beroenden
            worksheet.Cells["A1"].Value = 10;
            worksheet.Cells["A2"].Value = 20;
            worksheet.Cells["B1"].Formula = "=A1+A2";
            worksheet.Cells["C1"].Formula = "=B1*2";

            try
            {
                // Hämta cellen som har beroenden
                Cell cell = worksheet.Cells["A1"];

                // Anropa GetLeafs med den rekursiva parametern satt till true
                IEnumerator leafs = cell.GetLeafs(true);

                // Visa resultaten
                Console.WriteLine("Leaf cells found:");
                while (leafs.MoveNext())
                {
                    Cell leaf = (Cell)leafs.Current;
                    Console.WriteLine($"Cell: {leaf.Name}, Value: {leaf.Value}");
                }

                // Spara arbetsboken
                workbook.Save("GetLeafsDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling GetLeafs: {ex.Message}");
            }
        }
    }
}
```

### Se även

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


