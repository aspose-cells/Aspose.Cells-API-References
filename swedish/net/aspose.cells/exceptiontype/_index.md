---
title: "Enum ExceptionType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.ExceptionType enum. Representerar anpassad undantagstypkod"
type: docs
url: /sv/net/aspose.cells/exceptiontype/
---
## ExceptionType enumeration

Representerar anpassad undantagstypkod.

```csharp
public enum ExceptionType
```

### Värden

| Namn | Värde | Beskrivning |
| --- | --- | --- |
| Chart | `0` | Ogiltig diagraminställning. |
| DataType | `1` | Ogiltig inställning för datatyp. |
| DataValidation | `2` | Ogiltig inställning för datavalidering. |
| ConditionalFormatting | `3` | Ogiltig inställning för datavalidering. |
| FileFormat | `4` | Ogiltigt filformat. |
| Formula | `5` | Ogiltig formel. |
| InvalidData | `6` | Ogiltiga data. |
| InvalidOperator | `7` | Ogiltig operator. |
| IncorrectPassword | `8` | Felaktigt lösenord. |
| License | `9` | Licensrelaterade fel. |
| Limitation | `10` | Fel: överskrider MS Excel-begränsning. |
| PageSetup | `11` | Ogiltig sidinställning. |
| PivotTable | `12` | Ogiltig pivottabellsinställning. |
| Shape | `13` | Ogiltig inställning för ritobjekt. |
| Sparkline | `14` | Ogiltig inställning för sparkline-objekt. |
| SheetName | `15` | Ogiltigt bladnamn. |
| SheetType | `16` | Ogiltig bladtyp. |
| Interrupted | `17` | Processen avbryts. |
| IO | `18` | Filen är ogiltig. |
| Permission | `19` | Behörighet krävs för att öppna den här filen. |
| UnsupportedFeature | `20` | Funktionen stöds inte. |
| UnsupportedStream | `21` | Strömmen som ska öppnas stöds inte. |
| UndisclosedInformation | `22` | Filer innehåller viss dold information. |
| FileCorrupted | `23` | Filinnehållet är korrupt. |
| DefinedName | `25` | Ogiltigt definierat namn |
| Font | `26` | Ogiltigt teckensnitt |
| AutoFilter | `27` | Ogiltig inställning för autofilter. |
| FontSubstitution | `28` | Typsnittssubstitutionsvarningstyp när ett typsnitt inte har hittats, denna varningstyp kan hämtas. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ExceptionTypeDemo
    {
        public static void ExceptionTypeExample()
        {
            try
            {
                // Skapa en ny arbetsbok
                Workbook workbook = new Workbook();

                // Försök att ange ett ogiltigt bladnamn för att utlösa ett undantag
                workbook.Worksheets[0].Name = "Invalid/Name";

                // Spara arbetsboken
                workbook.Save("ExceptionTypeExample.xlsx");
            }
            catch (CellsException ex)
            {
                // Hantera CellsException
                Console.WriteLine("An error occurred: " + ex.Message);
                Console.WriteLine("Exception Type Code: " + ex.Code);
                
                // Kontrollera undantagstypen
                switch (ex.Code)
                {
                    case ExceptionType.SheetName:
                        Console.WriteLine("The worksheet name is invalid.");
                        break;
                    case ExceptionType.FileFormat:
                        Console.WriteLine("The file format is invalid.");
                        break;
                    // Lägg till fler fall vid behov för olika undantagstyper
                    default:
                        Console.WriteLine("An unknown error occurred.");
                        break;
                }
            }
            catch (Exception ex)
            {
                // Hantera alla andra undantag
                Console.WriteLine("An unexpected error occurred: " + ex.Message);
            }
        }
    }
}
```

### Se även

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


