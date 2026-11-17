---
title: "Clase LowCodeSaveOptions"
linktitle: "LowCodeSaveOptions"
second_title: "Aspose.Cells for Go via C++ API Reference"
description: "Clase LowCodeSaveOptions. Encapsula el objeto que representa lowcodesaveoptions en Go."
type: docs
weight: 200
url: /es/go-cpp/lowcodesaveoptions/
---

## LowCodeSaveOptions class

Options for saving generated results in low code way.

```go

type LowCodeSaveOptions struct  {
	ptr unsafe.Pointer
}

```
## Constructors

| Method | Description |
| --- | --- |
| [NewLowCodeSaveOptions](./newlowcodesaveoptions/) | Default constructor. |

## Methods

| Method | Description |
| --- | --- |
| [IsNull](./isnull/) | Checks whether the implementation object is nullptr. |
| [GetOutputFile](./getoutputfile/) | Gets and sets the file(with path if needed) for saving the generated data.When setting this property with value other than null or empty string, OutputStream will be ignored. |
| [SetOutputFile](./setoutputfile/) | Gets and sets the file(with path if needed) for saving the generated data.When setting this property with value other than null or empty string, OutputStream will be ignored. |
| [GetOutputStream](./getoutputstream/) | Gets and sets the Stream for writing the generated data to.When setting this property with value other than null, OutputFile will be ignored. |
| [SetOutputStream](./setoutputstream/) | Gets and sets the Stream for writing the generated data to.When setting this property with value other than null, OutputFile will be ignored. |
| [GetSaveFormat](./getsaveformat/) | Obtiene y establece el formato de guardado para la salida.Generalmente, para procesos específicos en modo low code, solo se permiten algunos formatos específicos.Por favor, especifique el formato correcto para el proceso correspondiente, de lo contrario se pueden producir resultados inesperados o incluso una excepción. |
| [SetSaveFormat](./setsaveformat/) | Obtiene y establece el formato de guardado para la salida.Generalmente, para procesos específicos en modo low code, solo se permiten algunos formatos específicos.Por favor, especifique el formato correcto para el proceso correspondiente, de lo contrario se pueden producir resultados inesperados o incluso una excepción. |
