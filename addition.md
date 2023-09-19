# Addition of two numbers

## addition of two numbers if carry is generated

| **Size** | **Label** | **Instructions** | **Hex code** | **Addresses** |
| ----------- | ----------- | ----------- | ----------- | ---------- |
| 2 |  | MVI C,00H | 0E, 00H | 2000 |
| 3 |  | LDA 2050H | 3A, 50, 20 | 2002 |
| 1 |  | MOV B,A | 47 | 2005 |
| 3 |  | LDA 2051H | 3A, 51, 20 | 2006 |
| 1 |  | ADD B | 80 | 2009 |
| 3 |  | JNC SKIP | D2, 0E, 20 | 200A |
| 1 |  | INR C | 0C | 200D |
| 3 | SKIP | STA 2055H | 32, 55, 20 | 200E |
| 1 |  | MOV A, C | 79 | 2011 |
| 3 |  | STA 2056H | 32, 56, 20 | 2012 |
| 1 |  | HLT | 76 | 2015 |
| -- |
| 22 |