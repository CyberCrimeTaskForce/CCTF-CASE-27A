# Unicode Reference

**Unicode** is a standard used to represent characters from different writing systems. Each character is assigned a unique **code point**.

Unicode code points are commonly written in the format:

```text
U+XXXX
```

For example:

```text
U+0041 → A
U+0042 → B
U+0043 → C
```

## Uppercase Letters

| Character | Unicode  | Character | Unicode  |
| :-------: | :------: | :-------: | :------: |
|     A     | `U+0041` |     N     | `U+004E` |
|     B     | `U+0042` |     O     | `U+004F` |
|     C     | `U+0043` |     P     | `U+0050` |
|     D     | `U+0044` |     Q     | `U+0051` |
|     E     | `U+0045` |     R     | `U+0052` |
|     F     | `U+0046` |     S     | `U+0053` |
|     G     | `U+0047` |     T     | `U+0054` |
|     H     | `U+0048` |     U     | `U+0055` |
|     I     | `U+0049` |     V     | `U+0056` |
|     J     | `U+004A` |     W     | `U+0057` |
|     K     | `U+004B` |     X     | `U+0058` |
|     L     | `U+004C` |     Y     | `U+0059` |
|     M     | `U+004D` |     Z     | `U+005A` |

## Lowercase Letters

| Character | Unicode  | Character | Unicode  |
| :-------: | :------: | :-------: | :------: |
|     a     | `U+0061` |     n     | `U+006E` |
|     b     | `U+0062` |     o     | `U+006F` |
|     c     | `U+0063` |     p     | `U+0070` |
|     d     | `U+0064` |     q     | `U+0071` |
|     e     | `U+0065` |     r     | `U+0072` |
|     f     | `U+0066` |     s     | `U+0073` |
|     g     | `U+0067` |     t     | `U+0074` |
|     h     | `U+0068` |     u     | `U+0075` |
|     i     | `U+0069` |     v     | `U+0076` |
|     j     | `U+006A` |     w     | `U+0077` |
|     k     | `U+006B` |     x     | `U+0078` |
|     l     | `U+006C` |     y     | `U+0079` |
|     m     | `U+006D` |     z     | `U+007A` |

## Numbers

| Character | Unicode  | Character | Unicode  |
| :-------: | :------: | :-------: | :------: |
|     0     | `U+0030` |     5     | `U+0035` |
|     1     | `U+0031` |     6     | `U+0036` |
|     2     | `U+0032` |     7     | `U+0037` |
|     3     | `U+0033` |     8     | `U+0038` |
|     4     | `U+0034` |     9     | `U+0039` |

## Common Symbols

| Character | Unicode  | Character | Unicode  |
| :-------: | :------: | :-------: | :------: |
|   Space   | `U+0020` |    `!`    | `U+0021` |
|    `"`    | `U+0022` |    `#`    | `U+0023` |
|    `$`    | `U+0024` |    `%`    | `U+0025` |
|    `&`    | `U+0026` |    `'`    | `U+0027` |
|    `(`    | `U+0028` |    `)`    | `U+0029` |
|    `+`    | `U+002B` |    `,`    | `U+002C` |
|    `-`    | `U+002D` |    `.`    | `U+002E` |
|    `/`    | `U+002F` |    `:`    | `U+003A` |
|    `;`    | `U+003B` |    `=`    | `U+003D` |
|    `?`    | `U+003F` |    `@`    | `U+0040` |
|    `[`    | `U+005B` |    `\`    | `U+005C` |
|    `]`    | `U+005D` |    `_`    | `U+005F` |

## Example

A sequence such as:

```text
U+0041 U+0045 U+0054 U+0048 U+0045 U+0052
```

can be decoded as:

```text
A E T H E R
```

**Result: `AETHER`**

## Quick Reference

For standard English characters:

```text
A–Z → U+0041–U+005A
a–z → U+0061–U+007A
0–9 → U+0030–U+0039
```

When a sequence begins with **`U+`**, it may be worth checking whether it represents Unicode code points.
