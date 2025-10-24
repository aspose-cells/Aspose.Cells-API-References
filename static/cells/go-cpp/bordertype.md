##BorderType Enum
'BorderType enum. Encapsulates the object that represents bordertype in Go.'
## BorderType Enum
Enumerates the border line and diagonal line types.
```go
type BorderType int32
```
## Fields
| Field | Description |
| --- | --- |
|[LeftBorder](./leftborder/) | Represents left border line. |
|[RightBorder](./rightborder/) | Represents right border line exists. |
|[TopBorder](./topborder/) | Represents top border line. |
|[BottomBorder](./bottomborder/) | Represents bottom border line. |
|[DiagonalDown](./diagonaldown/) | Represents the diagonal line from top left to right bottom. |
|[DiagonalUp](./diagonalup/) | Represents the diagonal line from bottom left to right top. |
|[Vertical](./vertical/) | Only for dynamic style, such as conditional formatting. |
|[Horizontal](./horizontal/) | Only for dynamic style, such as conditional formatting. |
|[SideBorders](./sideborders/) | Indicates the four side borders: <see cref="LeftBorder"/>,<see cref="RightBorder"/>, <see cref="TopBorder"/> and <see cref="BottomBorder"/>. |
|[Diagonal](./diagonal/) | Special combination of multiple borders for user's convenience for some APIs.Indicates diagonal borders of <see cref="DiagonalUp"/> and <see cref="DiagonalDown"/>. |
|[DynamicStyleBorders](./dynamicstyleborders/) | Indicates <see cref="Vertical"/> and <see cref="Horizontal"/> of dynamic style. |
|[None](./none/) | No border has been specified. |
