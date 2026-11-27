---
title: "Cell.PutValue"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Cell-metod. Lägger in ett booleskt värde i cellen"
type: docs
url: /sv/net/aspose.cells/cell/putvalue/
---
## PutValue(bool) {#putvalue}

Sätter ett booleskt värde i cellen.

```csharp
public void PutValue(bool boolValue)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| boolValue | Boolean |  |

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodPutValueWithBooleanDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Lägg in ett booleskt värde i cell B3 (rad 2, kolumn 2)
            cells[2, 2].PutValue(true);

            // Verifiera att värdet har satts korrekt
            Console.WriteLine("Cell B3 value: " + cells[2, 2].Value);
        }
    }
}
```

### Se även

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## PutValue(int) {#putvalue_2}

Sätter ett heltalsvärde i cellen.

```csharp
public void PutValue(int intValue)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| intValue | Int32 | Ange värde |

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodPutValueWithInt32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            
            // Använd PutValue med Int32‑parametrar
            cells[0, 0].PutValue(10);
            cells[1, 0].PutValue(20);
            cells[2, 0].PutValue(30);
            
            // Beräkna summan av värdena
            cells[3, 0].Formula = "=SUM(A1:A3)";
            workbook.CalculateFormula();
            
            Console.WriteLine("Sum of values: " + cells[3, 0].IntValue);
        }
    }
}
```

### Se även

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## PutValue(double) {#putvalue_1}

Sätter ett double-värde i cellen.

```csharp
public void PutValue(double doubleValue)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| doubleValue | Double | Ange värde |

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodPutValueWithDoubleDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            
            // Ange double‑värden med PutValue‑metoden
            cells[0, 0].PutValue("Item");
            cells[0, 1].PutValue("Price");
            cells[1, 0].PutValue("Apple");
            cells[1, 1].PutValue(0.69);
            cells[2, 0].PutValue("Banana");
            cells[2, 1].PutValue(0.49);
            cells[3, 0].PutValue("Orange");
            cells[3, 1].PutValue(0.29);

            // Spara arbetsboken
            workbook.Save("PutValueWithDoubleDemo.xlsx");
        }
    }
}
```

### Se även

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## PutValue(string, bool, bool) {#putvalue_7}

Sätter ett värde i cellen, om lämpligt kommer värdet att konverteras till annan datatyp och cellens talformat återställas.

```csharp
public void PutValue(string stringValue, bool isConverted, bool setStyle)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| stringValue | String | Ange värde |
| isConverted | Boolean | True: konverterad till annan datatyp om lämpligt. |
| setStyle | Boolean | True: sätt talformatet till cellens stil vid konvertering till annan datatyp |

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodPutValueWithStringBooleanBooleanDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Kom åt första arbetsbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Hämta cell B3
            Cell cell = worksheet.Cells["B3"];
            
            // Ställ in datavalidering för ålder (måste vara ett positivt tal)
            Validation validation = cell.GetValidation();
            validation.Type = ValidationType.WholeNumber;
            validation.Operator = OperatorType.GreaterThan;
            validation.Formula1 = "0";
            
            // Ange värde med konvertering och valideringskontroll
            cell.PutValue("-60", true, false);
            
            // Beräkna formler (även om det inte behövs i detta enkla fall)
            workbook.CalculateFormula();
            
            // Kontrollera om värdet är giltigt
            bool isValid = cell.GetValidationValue();
            Console.WriteLine("Is value valid? " + isValid);
            
            // Spara arbetsbok
            workbook.Save("output.xlsx");
        }
    }
}
```

### Se även

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## PutValue(string, bool) {#putvalue_6}

Sätter ett strängvärde i cellen och konverterar värdet till annan datatyp om lämpligt.

```csharp
public void PutValue(string stringValue, bool isConverted)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| stringValue | String | Ange värde |
| isConverted | Boolean | True: konverterad till annan datatyp om lämpligt. |

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodPutValueWithStringBooleanDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Demonstrera PutValue med sträng‑ och booleska parametrar
            cells["B2"].PutValue("123", true);  // String value with conversion flag
            cells["C2"].PutValue("456", false); // String value without conversion
            
            // Verifiera värdena
            Console.WriteLine("B2 value (converted): " + cells["B2"].Value); // Should show 123 as number
            Console.WriteLine("C2 value (raw): " + cells["C2"].Value);       // Should show "456" as string

            workbook.Save("PutValueDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Se även

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## PutValue(string) {#putvalue_5}

Sätter ett strängvärde i cellen.

```csharp
public void PutValue(string stringValue)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| stringValue | String | Ange värde |

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodPutValueWithStringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            
            // Använd PutValue med strängparametrar
            cells[0, 0].PutValue("Product");
            cells[0, 1].PutValue("Category");
            cells[0, 2].PutValue("Price");
            
            cells[1, 0].PutValue("Laptop");
            cells[1, 1].PutValue("Electronics");
            cells[1, 2].PutValue(999.99);
            
            cells[2, 0].PutValue("Desk Chair");
            cells[2, 1].PutValue("Furniture");
            cells[2, 2].PutValue(199.50);
            
            // Spara arbetsboken
            workbook.Save("PutValueStringDemo.xlsx");
        }
    }
}
```

### Se även

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## PutValue(DateTime) {#putvalue_3}

Sätter ett DateTime-värde i cellen.

```csharp
public void PutValue(DateTime dateTime)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| dateTime | DateTime | Ange värde |

### Anmärkningar

Att sätta ett DateTime‑värde för en cell betyder inte att cellen automatiskt kommer att formateras som datum/tid. DateTime‑värdet behölls som ett numeriskt värde i datamodellen för både MS Excel och Aspose.Cells. Om det numeriska värdet kommer att tolkas som själva det numeriska värdet eller som datum/tid beror på det talformat som tillämpas på denna cell. Om denna cell inte har formaterats som datum/tid kommer den att visas som ett numeriskt värde även om du har angett ett DateTime‑värde.

### Exempel

Detta exempel visar hur man sätter ett DateTime‑värde i en cell och får det att visas som datum/tid.

```csharp
[C#]

Workbook excel = new Workbook();
Cells cells = excel.Worksheets[0].Cells;

//Sätt datum/tid i en cell
Cell cell = cells[0, 0];
cell.PutValue(new DateTime(2023, 5, 15));
Style style = cell.GetStyle(false);
style.Number = 14;
cell.SetStyle(style);
```

### Se även

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## PutValue(object) {#putvalue_4}

Sätter ett objektvärde i cellen.

```csharp
public void PutValue(object objectValue)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| objectValue | Object | indatavärde |

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodPutValueWithObjectDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            
            // PutValue med DateTime‑objekt
            DateTime dt = new DateTime(2008, 2, 2);
            cells[0, 0].PutValue((object)dt);
            
            // PutValue med strängobjekt
            cells[1, 0].PutValue((object)"Hello World");
            
            // PutValue med numeriskt objekt
            cells[2, 0].PutValue((object)123.45);
            
            // Spara arbetsboken
            workbook.Save("PutValueWithObjectDemo.xlsx");
        }
    }
}
```

### Se även

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


