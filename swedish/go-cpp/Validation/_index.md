---
title: "Validation-klass"
linktitle: "Validation"
second_title: "Aspose.Cells för Go via C++ API-referens"
description: "Validation-klass. Inkapslar objektet som representerar validering i Go."
type: docs
weight: 200
url: /sv/go-cpp/validation/
---

## Validation class

Representerar data valideringsinställningar.

```go

type Validation struct  {
	ptr unsafe.Pointer
}

```
## Konstruktörer

| Metod | Beskrivning |
| --- | --- |

## Metoder

| Metod | Beskrivning |
| --- | --- |
| [IsNull](./isnull/) | Kontrollerar om implementeringsobjektet är nullptr. |
| [GetOperator](./getoperator/) | Representerar operatorn för datavalideringen. |
| [SetOperator](./setoperator/) | Representerar operatorn för datavalideringen. |
| [GetAlertStyle](./getalertstyle/) | Representerar valideringsvarningsstilen. |
| [SetAlertStyle](./setalertstyle/) | Representerar valideringsvarningsstilen. |
| [GetType](./gettype/) | Representerar datavalideringstypen. |
| [SetType](./settype/) | Representerar datavalideringstypen. |
| [GetInputMessage](./getinputmessage/) | Representerar inmatningsmeddelandet för datavalidering. |
| [SetInputMessage](./setinputmessage/) | Representerar inmatningsmeddelandet för datavalidering. |
| [GetInputTitle](./getinputtitle/) | Representerar titeln på inmatningsdialogrutan för datavalidering. |
| [SetInputTitle](./setinputtitle/) | Representerar titeln på inmatningsdialogrutan för datavalidering. |
| [GetErrorMessage](./geterrormessage/) | Representerar felmeddelandet för datavalidering. |
| [SetErrorMessage](./seterrormessage/) | Representerar felmeddelandet för datavalidering. |
| [GetErrorTitle](./geterrortitle/) | Representerar titeln på fel-dialogrutan för datavalidering. |
| [SetErrorTitle](./seterrortitle/) | Representerar titeln på fel-dialogrutan för datavalidering. |
| [GetShowInput](./getshowinput/) | Anger om inmatningsmeddelandet för datavalidering ska visas när användaren markerar en cell i datavalideringsområdet. |
| [SetShowInput](./setshowinput/) | Anger om inmatningsmeddelandet för datavalidering ska visas när användaren markerar en cell i datavalideringsområdet. |
| [GetShowError](./getshowerror/) | Anger om felmeddelandet för datavalidering ska visas när användaren anger ogiltiga data. |
| [SetShowError](./setshowerror/) | Anger om felmeddelandet för datavalidering ska visas när användaren anger ogiltiga data. |
| [GetIgnoreBlank](./getignoreblank/) | Anger om tomma värden tillåts av datavalideringen för området. |
| [SetIgnoreBlank](./setignoreblank/) | Anger om tomma värden tillåts av datavalideringen för området. |
| [GetFormula1_Bool_Bool](./getformula1_bool_bool/) | Hämtar värdet eller uttrycket som är associerat med denna validering. |
| [GetFormula2_Bool_Bool](./getformula2_bool_bool/) | Hämtar värdet eller uttrycket som är associerat med denna validering. |
| [GetFormula1_Bool_Bool_Int_Int](./getformula1_bool_bool_int_int/) | Hämtar värdet eller uttrycket som är associerat med denna validering för en specifik cell. |
| [GetFormula2_Bool_Bool_Int_Int](./getformula2_bool_bool_int_int/) | Hämtar värdet eller uttrycket som är associerat med denna validering för en specifik cell. |
| [SetFormula1_String_Bool_Bool](./setformula1_string_bool_bool/) | Ställer in värdet eller uttrycket som är associerat med denna validering. |
| [SetFormula2_String_Bool_Bool](./setformula2_string_bool_bool/) | Ställer in värdet eller uttrycket som är associerat med denna validering. |
| [GetFormula1](./getformula1/) | Representerar värdet eller uttrycket som är associerat med datavalideringen. |
| [SetFormula1_String](./setformula1_string/) | Representerar värdet eller uttrycket som är associerat med datavalideringen. |
| [GetFormula2](./getformula2/) | Representerar värdet eller uttrycket som är associerat med datavalideringen. |
| [SetFormula2_String](./setformula2_string/) | Representerar värdet eller uttrycket som är associerat med datavalideringen. |
| [GetListValue](./getlistvalue/) | Hämta värdet för listan av valideringen för den angivna cellen. |
| [GetValue1](./getvalue1/) | Representerar det första värdet som är associerat med datavalideringen. |
| [SetValue1](./setvalue1/) | Representerar det första värdet som är associerat med datavalideringen. |
| [GetValue2](./getvalue2/) | Representerar det andra värdet som är associerat med datavalideringen. |
| [SetValue2](./setvalue2/) | Representerar det andra värdet som är associerat med datavalideringen. |
| [GetValue](./getvalue/) | Hämta värdet för valideringen på den specifika cellen. |
| [GetInCellDropDown](./getincelldropdown/) | Anger om datavalidering visar en rullgardinslista som innehåller godkända värden. |
| [SetInCellDropDown](./setincelldropdown/) | Anger om datavalidering visar en rullgardinslista som innehåller godkända värden. |
| [GetAreas](./getareas/) | Hämtar alla CellArea som innehåller datavalideringsinställningarna. |
| [AddArea_CellArea](./addarea_cellarea/) | Tillämpar valideringen på området. |
| [AddArea_CellArea_Bool_Bool](./addarea_cellarea_bool_bool/) | Tillämpar valideringen på området. |
| [AddAreas](./addareas/) | Tillämpar valideringen på angivna områden. |
| [RemoveArea](./removearea/) | Ta bort valideringsinställningarna i området. |
| [RemoveAreas](./removeareas/) | Tar bort denna validering från angivna områden. |
| [RemoveACell](./removeacell/) | Ta bort valideringsinställningarna i cellen. |
| [Copy](./copy/) | Copy validation. |
