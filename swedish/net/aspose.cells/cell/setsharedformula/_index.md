---
title: "Cell.SetSharedFormula"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Cell-metod. Anger en formel för ett cellområde."
type: docs
url: /sv/net/aspose.cells/cell/setsharedformula/
---
## SetSharedFormula(string, int, int, bool, bool) {#setsharedformula_3}

Anger en formel för ett cellområde.

```csharp
[Obsolete("Use FormulaParseOptions for more options instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public void SetSharedFormula(string sharedFormula, int rowNumber, int columnNumber, bool isR1C1, 
    bool isLocal)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| sharedFormula | String | Delad formel. |
| rowNumber | Int32 | Antal rader för att fylla i formeln. |
| columnNumber | Int32 | Antal kolumner för att fylla i formeln. |
| isR1C1 | Boolean | om formeln är en R1C1-formel |
| isLocal | Boolean | om formeln är lokalanpassad |

### Anmärkningar

OBS: Denna klass är nu föråldrad. Använd istället Cell.SetSharedFormula(string,int,int,FormulaParseOptions). Denna egenskap kommer att tas bort 12 månader efter december 2019. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellMethodSetSharedFormulaWithStringInt32Int32BooleanBooleanDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok och öppna det första kalkylbladet
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;
            // Fyll i exempeldata i kolumn A
            for (int row = 0; row < 5; row++)
            {
                cells[row, 0].Value = row + 1; // A1-A5: 1-5
            }

            // Hämta målcell B1 för att ange delad formel
            Cell targetCell = cells[0, 1]; // B1

            try
            {
                // Ställ in delad formel för att beräkna kvadraten av värden i kolumn A
                // Parametrar: (formula, rowCount=5, columnCount=1, isR1C1=false, isLocal=false)
#pragma warning disable 0618 // Disable obsolete warning for demonstration
                targetCell.SetSharedFormula("=A1^2", 5, 1, false, false);
#pragma warning restore 0618

                // Verifiera formelpropagering
                Console.WriteLine($"B1 formula: {targetCell.Formula}");
                Console.WriteLine($"B5 formula: {cells[4, 1].Formula}");

                // Beräkna arbetsbok för att uppdatera formelresultat
                workbook.CalculateFormula();

                Console.WriteLine($"A1 value: {cells["A1"].Value}");
                Console.WriteLine($"A5 value: {cells["A5"].Value}");
                Console.WriteLine($"B1 value: {targetCell.Value}");
                Console.WriteLine($"B5 value: {cells[4, 1].Value}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error setting shared formula: {ex.Message}");
                return;
            }

            // Spara den modifierade arbetsboken
            workbook.Save("SetSharedFormulaDemo.xlsx");
            Console.WriteLine("Spreadsheet saved successfully.");
        }
    }
}
```

### Se även

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## SetSharedFormula(string, int, int) {#setsharedformula}

Ställer in delade formler för ett cellområde.

```csharp
public void SetSharedFormula(string sharedFormula, int rowNumber, int columnNumber)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| sharedFormula | String | Delad formel. |
| rowNumber | Int32 | Antal rader för att fylla i formeln. |
| columnNumber | Int32 | Antal kolumner för att fylla i formeln. |

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodSetSharedFormulaWithStringInt32Int32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Ställ in en delad formel i kolumn B från B1 till B20
            cells["B1"].SetSharedFormula("=C1*2", 20, 1);

            // Ange några värden i kolumn C för att demonstrera formelberäkningen
            for (int i = 0; i < 20; i++)
            {
                cells[i, 2].PutValue(i + 1); // Column C values (C1=1, C2=2...)
            }

            // Beräkna formler
            workbook.CalculateFormula();

            // Skriv ut resultat för verifiering
            for (int i = 0; i < 5; i++) // Display first 5 results
            {
                Console.WriteLine($"B{i+1} value: {cells[i, 1].Value}");
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

## SetSharedFormula(string, int, int, FormulaParseOptions) {#setsharedformula_1}

Ställer in delade formler för ett cellområde.

```csharp
public void SetSharedFormula(string sharedFormula, int rowNumber, int columnNumber, 
    FormulaParseOptions options)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| sharedFormula | String | Delad formel. |
| rowNumber | Int32 | Antal rader för att fylla i formeln. |
| columnNumber | Int32 | Antal kolumner för att fylla i formeln. |
| alternativ | FormulaParseOptions | Alternativ för att tolka formeln. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellMethodSetSharedFormulaWithStringInt32Int32FormulaParseOpDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok och öppna det första kalkylbladet
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fyll i exempeldata i kolumn A
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].PutValue(30);

            // Hämta målcell där vi ska sätta den delade formeln
            Cell targetCell = worksheet.Cells["B1"];

            try
            {
                // Skapa alternativ för formeltolkning med standardinställningar
                FormulaParseOptions options = new FormulaParseOptions();

                // Ställ in delad formel för 3 rader och 2 kolumner med start i B1
                targetCell.SetSharedFormula("=A1*2", 3, 2, options);

                Console.WriteLine("Shared formula set successfully for B1:C3 range");
                Console.WriteLine("B1 formula: " + worksheet.Cells["B1"].Formula);
                Console.WriteLine("C3 formula: " + worksheet.Cells["C3"].Formula);

                workbook.CalculateFormula();
                Console.WriteLine("B3 value: " + worksheet.Cells["B3"].Value);
                Console.WriteLine("B1 value: " + worksheet.Cells["B1"].Value);
                Console.WriteLine("C3 value: " + worksheet.Cells["C3"].Value);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error setting shared formula: {ex.Message}");
            }

            // Spara den modifierade arbetsboken
            workbook.Save("SetSharedFormulaDemo.xlsx");
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

## SetSharedFormula(string, int, int, FormulaParseOptions, object[][]) {#setsharedformula_2}

Ställer in delade formler för ett cellområde.

```csharp
public void SetSharedFormula(string sharedFormula, int rowNumber, int columnNumber, 
    FormulaParseOptions options, object[][] values)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| sharedFormula | String | Delad formel. |
| rowNumber | Int32 | Antal rader för att fylla i formeln. |
| columnNumber | Int32 | Antal kolumner för att fylla i formeln. |
| alternativ | FormulaParseOptions | Alternativ för att tolka formeln. |
| värden | Object[][] | värden för de cellerna med given delad formel |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Collections;

    public class CellMethodSetSharedFormulaWithStringInt32Int32FormulaParseOpDemo1
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok och öppna det första kalkylbladet
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ange exempelvärde i cell A1
            worksheet.Cells["A1"].PutValue(5);

            // Hämta målcell B2 där den delade formeln kommer att sättas
            Cell cell = worksheet.Cells["B2"];

            try
            {
                // Definiera parametrar för delad formel
                string formula = "=A1*2";
                int totalRows = 2;
                int totalColumns = 2;
                FormulaParseOptions parseOptions = new FormulaParseOptions();
                object[][] presetValues = new object[2][]
                {
                    new object[] { 10, 10 },
                    new object[] { 10, 10 }
                };

                // Ställ in delad formel för 2x2-område med start i B2 med förinställda värden
                cell.SetSharedFormula(formula, totalRows, totalColumns, parseOptions, presetValues);

                Console.WriteLine("Shared formula set successfully. Cells B2:C3 contain values 10");
                workbook.CalculateFormula();
                Aspose.Cells.Range range = worksheet.Cells.CreateRange("B2", "C3");
                IEnumerator iter = range.GetEnumerator();
                while(iter.MoveNext()) 
                {
                    Cell temp = (Cell)iter.Current;
                    Console.WriteLine(temp.Name + "  " + temp.Value);
                }

            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error setting shared formula: {ex.Message}");
            }

            // Spara den modifierade arbetsboken
            workbook.Save("SetSharedFormulaDemo.xlsx");
        }
    }
}
```

### Se även

* class [FormulaParseOptions](../../formulaparseoptions/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


