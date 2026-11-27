---
title: "Cell.SetArrayFormula"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Cell‑metod. Anger en matrisformel för ett område av celler"
type: docs
url: /sv/net/aspose.cells/cell/setarrayformula/
---
## SetArrayFormula(string, int, int, bool, bool) {#setarrayformula_3}

Ställer in en matrisformel för ett cellområde.

```csharp
[Obsolete("Use FormulaParseOptions for more options instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public void SetArrayFormula(string arrayFormula, int rowNumber, int columnNumber, bool isR1C1, 
    bool isLocal)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| arrayFormula | String | Matrisformel. |
| rowNumber | Int32 | Antal rader för att fylla resultatet av matrisformeln. |
| columnNumber | Int32 | Antal kolumner för att fylla resultatet av matrisformeln. |
| isR1C1 | Boolean | om formeln är en R1C1-formel |
| isLocal | Boolean | om formeln är lokalanpassad |

### Anmärkningar

OBS: Den här klassen är nu föråldrad. Använd istället Cell.SetArrayFormula(string,int,int,FormulaParseOptions). Denna egenskap kommer att tas bort 12 månader senare sedan december 2019. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellMethodSetArrayFormulaWithStringInt32Int32BooleanBooleanDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();

            // Åtkomst till det första kalkylbladet
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till lite exempeldata
            worksheet.Cells["A1"].Value = 10;
            worksheet.Cells["A2"].Value = 20;
            worksheet.Cells["A3"].Value = 30;

            try
            {
                // Hämta målcell där vi vill ange matrisformeln
                Cell targetCell = worksheet.Cells["B1"];

                // Ange en matrisformel som multiplicerar värdena i A1:A3 med 2
                // Parametrar: (formula, rowNumber=3, columnNumber=1, isR1C1=false, isLocal=false)
                targetCell.SetArrayFormula("=A1:A3*2", 3, 1, false, false);

                // Beräkna arbetsboken för att se resultaten
                workbook.CalculateFormula();

                // Visa resultaten
                Console.WriteLine($"B1 value: {targetCell.Value}");
                Console.WriteLine($"B2 value: {worksheet.Cells["B2"].Value}");
                Console.WriteLine($"B3 value: {worksheet.Cells["B3"].Value}");

                // Spara arbetsboken
                workbook.Save("SetArrayFormulaDemo.xlsx");
                Console.WriteLine("Array formula set successfully and workbook saved.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error setting array formula: {ex.Message}");
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

## SetArrayFormula(string, int, int) {#setarrayformula}

Ställer in en matrisformel (äldre matrisformel som matas in via CTRL+SHIFT+ENTER i MS Excel) för ett cellområde.

```csharp
public void SetArrayFormula(string arrayFormula, int rowNumber, int columnNumber)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| arrayFormula | String | Matrisformel. |
| rowNumber | Int32 | Antal rader för att fylla resultatet av matrisformeln. |
| columnNumber | Int32 | Antal kolumner för att fylla resultatet av matrisformeln. |

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodSetArrayFormulaWithStringInt32Int32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            Cell cell = cells["A1"];
            cell.SetArrayFormula("=FREQUENCY({\"79\",\"85\",\"78\",\"85\",\"50\",\"81\",\"95\",\"88\",\"97\"},{70,79,89})", 4, 1);

            workbook.CalculateFormula();

            for (int i = 0; i < 4; i++)
            {
                Console.WriteLine($"Cell A{i+1} value: {cells[i, 0].IntValue}");
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

## SetArrayFormula(string, int, int, FormulaParseOptions) {#setarrayformula_1}

Ställer in en matrisformel för ett cellområde.

```csharp
public void SetArrayFormula(string arrayFormula, int rowNumber, int columnNumber, 
    FormulaParseOptions options)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| arrayFormula | String | Matrisformel. |
| rowNumber | Int32 | Antal rader för att fylla resultatet av matrisformeln. |
| columnNumber | Int32 | Antal kolumner för att fylla resultatet av matrisformeln. |
| alternativ | FormulaParseOptions | Alternativ för att tolka formeln. |

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodSetArrayFormulaWithStringInt32Int32FormulaParseOpDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok
            Workbook workbook = new Workbook();
            
            // Kom åt första arbetsbladet
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Placera exempeldata i cellerna C1:E1
            cells["C1"].PutValue(10);
            cells["D1"].PutValue(20);
            cells["E1"].PutValue(30);

            // Ange matrisformel i cell A1 som kommer att spilla över till 2 rader och 3 kolumner
            cells["A1"].SetArrayFormula("=TRANSPOSE(C1:E1)", 2, 1, new FormulaParseOptions());

            // Beräkna formler
            workbook.CalculateFormula();

            // Skriv ut resultaten
            Console.WriteLine("Array formula results:");
            for (int row = 0; row < 2; row++)
            {
                for (int col = 0; col < 3; col++)
                {
                    Cell cell = cells[row, col];
                    Console.WriteLine($"Cell {cell.Name}: {cell.Value}");
                }
            }
        }
    }
}
```

### Se även

* class [FormulaParseOptions](../../formulaparseoptions/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## SetArrayFormula(string, int, int, FormulaParseOptions, object[][]) {#setarrayformula_2}

Ställer in en matrisformel för ett cellområde.

```csharp
public void SetArrayFormula(string arrayFormula, int rowNumber, int columnNumber, 
    FormulaParseOptions options, object[][] values)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| arrayFormula | String | Matrisformel. |
| rowNumber | Int32 | Antal rader för att fylla resultatet av matrisformeln. |
| columnNumber | Int32 | Antal kolumner för att fylla resultatet av matrisformeln. |
| alternativ | FormulaParseOptions | Alternativ för att tolka formeln. |
| värden | Object[][] | värden för dessa celler med given matrisformel |

### Se även

* class [FormulaParseOptions](../../formulaparseoptions/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


