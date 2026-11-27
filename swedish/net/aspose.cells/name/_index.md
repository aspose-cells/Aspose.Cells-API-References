---
title: "Klassnamn"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Name‑klass. Representerar ett definierat namn för ett cellområde"
type: docs
url: /sv/net/aspose.cells/name/
---
## Name class

Representerar ett definierat namn för ett cellområde.

```csharp
public class Name
```

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [Comment](../../aspose.cells/name/comment/) { get; set; } | Hämtar och anger kommentaren för namnet. Gäller endast för Excel 2007 eller senare versioner. |
| [FullText](../../aspose.cells/name/fulltext/) { get; } | Hämtar namnets fullständiga text för objektet med omfångsinställningen. |
| [IsReferred](../../aspose.cells/name/isreferred/) { get; } | Anger om detta namn refereras av andra formler. |
| [IsVisible](../../aspose.cells/name/isvisible/) { get; set; } | Anger om namnet är synligt. |
| [R1C1RefersTo](../../aspose.cells/name/r1c1refersto/) { get; set; } | Hämtar eller anger en R1C1‑referens för `Name`. |
| [RefersTo](../../aspose.cells/name/refersto/) { get; set; } | Returnerar eller anger formeln som namnet är definierat att referera till, inledningsvis med ett likhetstecken. |
| [SheetIndex](../../aspose.cells/name/sheetindex/) { get; set; } | Anger att detta namn tillhör Workbook eller Worksheet. 0 = Globalt namn, annars index till blad (en‑baserat) |
| [Text](../../aspose.cells/name/text/) { get; set; } | Hämtar namntexten för objektet. |

## Metoder

| Namn | Beskrivning |
| --- | --- |
| [GetRange](../../aspose.cells/name/getrange/#getrange)() | Hämtar området om detta namn refererar till ett område. |
| [GetRange](../../aspose.cells/name/getrange/#getrange_1)(bool) | Hämtar området om detta namn refererar till ett område |
| [GetRange](../../aspose.cells/name/getrange/#getrange_2)(int, int, int) | Hämtar området om detta namn refererar till ett område. Om referensen för detta namn inte är absolut kan området vara olika för olika celler. |
| [GetRanges](../../aspose.cells/name/getranges/#getranges)() | Hämtar alla områden som refereras av detta namn. |
| [GetRanges](../../aspose.cells/name/getranges/#getranges_1)(bool) | Hämtar alla områden som refereras av detta namn. |
| [GetReferredAreas](../../aspose.cells/name/getreferredareas/)(bool) | Hämtar alla referenser som refereras av detta namn. |
| [GetRefersTo](../../aspose.cells/name/getrefersto/#getrefersto)(bool, bool) | Hämta referensen för detta Name. |
| [GetRefersTo](../../aspose.cells/name/getrefersto/#getrefersto_1)(bool, bool, int, int) | Hämta referensen för detta Name baserat på angiven cell. |
| [SetRefersTo](../../aspose.cells/name/setrefersto/)(string, bool, bool) | Ange referensen för detta Name. |
| override [ToString](../../aspose.cells/name/tostring/)() | Returnerar en sträng som representerar det aktuella Range-objektet. |

### Exempel

```csharp

[C#]

//Instansiering av ett Workbook-objekt
Workbook workbook = new Workbook();
//Åtkomst till det första kalkylbladet i Excel-filen
Worksheet worksheet = workbook.Worksheets[0];
//Skapa ett namngivet område
Range range = worksheet.Cells.CreateRange("B4", "G14");
//Ställa in namnet på det namngivna området
range.Name = "TestRange";
//Spara den modifierade Excel-filen i standardformat (det vill säga Excel 2000)
workbook.Save("output.xls");   

[Visual Basic]

'Instantiating a Workbook object
Dim workbook As Workbook = New Workbook()
'Accessing the first worksheet in the Excel file
Dim worksheet As Worksheet = workbook.Worksheets(0)
'Creating a named range
Dim range As Range = worksheet.Cells.CreateRange("B4", "G14")
'Setting the name of the named range
range.Name = "TestRange"
'Saving the modified Excel file in default (that is Excel 2000) format
workbook.Save("output.xls")
```

### Se även

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


