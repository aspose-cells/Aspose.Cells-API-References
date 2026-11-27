---
title: "Cell.SetFormula"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Cell-metod. Ställ in formeln och det beräknade resultatet av formeln"
type: docs
url: /sv/net/aspose.cells/cell/setformula/
---
## SetFormula(string, object) {#setformula_3}

Ställ in formeln och värdet (beräknat resultat) för formeln.

```csharp
public void SetFormula(string formula, object value)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| formel | String | Formeln. |
| värde | Object | Värdet (beräknade resultatet) av formeln. |

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodSetFormulaWithStringObjectDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Ställ in formel med sträng- och objektparametrar
            cells["A1"].SetFormula("=SUM(1,2)", 4); // Will display 4 until calculation
            cells["A2"].SetFormula("=AVERAGE(5,10)", 7.5); // Will display 7.5 until calculation

            // Visa värden före beräkning
            Console.WriteLine("Before Calculation:");
            Console.WriteLine("A1: " + cells["A1"].StringValue);
            Console.WriteLine("A2: " + cells["A2"].StringValue);

            // Beräkna formler
            workbook.CalculateFormula();

            // Visa värden efter beräkning
            Console.WriteLine("\nAfter Calculation:");
            Console.WriteLine("A1: " + cells["A1"].IntValue); // Should show 3
            Console.WriteLine("A2: " + cells["A2"].DoubleValue); // Should show 7.5
        }
    }
}
```

### Se även

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## SetFormula(string, FormulaParseOptions) {#setformula}

Ställ in formeln och värdet (beräknat resultat) för formeln.

```csharp
public void SetFormula(string formula, FormulaParseOptions options)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| formel | String | Formeln. |
| alternativ | FormulaParseOptions | Alternativ för att tolka formeln. |

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodSetFormulaWithStringFormulaParseOptionsDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Åtkomst till det första kalkylbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Hämta en specifik cell (B2 i detta fall)
            Cell cell = worksheet.Cells["B2"];
            
            // Ställ in några initiala värden för demonstration
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["B1"].PutValue(30);
            
            // Exempel 1: Ställ in en enkel formel med standardtolkningsalternativ
            cell.SetFormula("=SUM(A1:A2)", new FormulaParseOptions());
            Console.WriteLine("Formula with default options: " + cell.Formula);
            
            // Exempel 2: Ställ in formel med R1C1-stil med hjälp av FormulaParseOptions
            FormulaParseOptions options = new FormulaParseOptions();
            options.Parse = true;
            options.R1C1Style = true;
            
            cell.SetFormula("=SUM(R[-1]C[-1]:R[0]C[-1])", options);
            Console.WriteLine("Formula with R1C1 style: " + cell.Formula);
            
            // Exempel 3: Ställ in formel med tolkningsalternativ som bevarar R1C1-formatet
            options = new FormulaParseOptions();
            options.Parse = true;
            options.R1C1Style = true;
            cell.SetFormula("=R1C1+R2C2", options);
            Console.WriteLine("Formula preserved as R1C1: " + cell.Formula);
            
            // Beräkna arbetsboken för att se resultat
            workbook.CalculateFormula();
            Console.WriteLine("Calculated value: " + cell.Value);
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

## SetFormula(string, bool, bool, object) {#setformula_2}

Ange formeln och formelns värde.

```csharp
[Obsolete("Use FormulaParseOptions for more options instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public void SetFormula(string formula, bool isR1C1, bool isLocal, object value)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| formel | String | Formeln. |
| isR1C1 | Boolean | Om formeln är en R1C1-formel. |
| isLocal | Boolean | Om formeln är lokalt formaterad. |
| värde | Object | Värdet av formeln. |

### Anmärkningar

OBS: Den här klassen är nu föråldrad. Använd istället Cell.SetFormula(string,FormulaParseOptions,object). Den här egenskapen kommer att tas bort 12 månader senare sedan december 2019. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellMethodSetFormulaWithStringBooleanBooleanObjectDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till lite exempeldata
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["B1"].PutValue(30);
            worksheet.Cells["B2"].PutValue(40);

            // Hämta målcell där vi kommer att ställa in formeln
            Cell cell = worksheet.Cells["C1"];

            try
            {
                // Ställ in en formel med alla parametrar
                // Parametrar: formelsträng, isR1C1, isLocal, värde
                cell.SetFormula("=SUM(A1:B2)", false, false, null);

                // Beräkna formeln
                workbook.CalculateFormula();

                // Visa resultatet
                Console.WriteLine($"Formula set successfully. Result: {cell.Value}");

                // Spara arbetsboken
                workbook.Save("SetFormulaDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error setting formula: {ex.Message}");
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

## SetFormula(string, FormulaParseOptions, object) {#setformula_1}

Ställ in formeln och värdet (beräknat resultat) för formeln.

```csharp
public void SetFormula(string formula, FormulaParseOptions options, object value)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| formel | String | Formeln. |
| alternativ | FormulaParseOptions | Alternativ för att tolka formeln. |
| värde | Object | Värdet (beräknade resultatet) av formeln. |

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodSetFormulaWithStringFormulaParseOptionsObjecDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];

            // Ställ in initial formel med tilläggsreferens
            sheet.Cells[0, 0].Formula = "'externalDS.xlam'!dsfun(B1)";
            Console.WriteLine("Initial formula: " + sheet.Cells[0, 0].Formula);

            // Använd SetFormula för att åsidosätta utan att kontrollera tillägg
            sheet.Cells[0, 0].SetFormula("=dsfun(B1)", new FormulaParseOptions() { CheckAddIn = false }, null);
            Console.WriteLine("After SetFormula: " + sheet.Cells[0, 0].Formula);

            // Återställ till tilläggsformel
            sheet.Cells[0, 0].Formula = "'externalDS.xlam'!dsfun(B1)";
            Console.WriteLine("Reset to add-in formula: " + sheet.Cells[0, 0].Formula);

            // Skapa ny arbetsbok och kopiera bladet
            Workbook wb2 = new Workbook();
            wb2.Worksheets[0].Cells[0, 0].Formula = "'externalDS.xlam'!dsfunnew(C1)";
            wb2.Worksheets[0].Copy(sheet);
            Console.WriteLine("After copy: " + wb2.Worksheets[0].Cells[0, 0].Formula);
        }
    }
}
```

### Se även

* class [FormulaParseOptions](../../formulaparseoptions/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


