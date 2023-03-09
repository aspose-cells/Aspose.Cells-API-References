---
title: ReConnectionMethodType enumeración
second_title: Aspose.Cells for Python via .NET API Referencias
description:
type: docs
weight: 130
url: /es/python-net/aspose.cells.externalconnections/reconnectionmethodtype/
is_root: false
---
##  ReConnectionMethodType enumeración
Especifica lo que debe hacer la aplicación de hoja de cálculo cuando falla una conexión.



El tipo ReConnectionMethodType expone los siguientes miembros:

###  Campos
| Campo| Descripción|
| :- | :- |
| REQUIRED | Al actualizar, use la información de conexión existente y si termina siendo inválida<br/> luego obtenga información de conexión actualizada, si está disponible desde el archivo de conexión externo.|
| ALWAYS | En cada actualización, obtenga información de conexión actualizada del archivo de conexión externo,<br/> si está disponible, y utilícelo en lugar de la información de conexión existente.<br/> En este caso, la actualización de datos fallará si el archivo de conexión externa no está disponible.|
| NEVER | Nunca obtenga información de conexión actualizada del archivo de conexión externo<br/> incluso si está disponible e incluso si la información de conexión existente no es válida|



###  Ver también
* módulo [aspose.cells.externalconnections](..)
