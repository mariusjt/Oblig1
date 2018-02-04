**1. Fyll ut manglende tall i tabell**

<table>
  <tr>
    <td>Binære tall (mest signifikant bit til venstre</td>
    <td>Hexadesimaltall</td>
    <td>Desimaltall</td>
  </tr>
  <tr>
    <td>1101</td>
    <td>0xD</td>
    <td>13</td>
  </tr>
  <tr>
    <td>110111101010</td>
    <td>DEA </td>
    <td>3562</td>
  </tr>
  <tr>
    <td>0000 0000 1010 1111 0011 0100</td>
    <td>0xAF34</td>
    <td>44852 </td>
  </tr>
  <tr>
    <td> 1111111111111111</td>
    <td>FFFF </td>
    <td>65535</td>
  </tr>
  <tr>
    <td>10001011110001010 </td>
    <td> 1178A</td>
    <td>71562</td>
  </tr>
</table>


 

**Oppgave A**

**Beskriv kort metode for å gå fra binære tall til hexadesimale tall og motsatt. Beskriv kort metoden for å gå fra binære tall til desimaltall og motsatt.**

 

*Hexadesimale tall (også kalt sekstentallsystemet) består av 16 ulike siffer: 0,1,2,3,4,5,6,7,8,9,A,B,C,D,E og F.*

 

 

**Hexa -> binær -> hexa**

For å gå fra hexadesimaletall til binære og motsatt setter vi det ønskelige tallet inn i en tabell. 

For eksempel tallet ABC12. A = 10, B = 11, C = 12, 1 = 1, 2 = 2

<table>
  <tr>
    <td>Hexa</td>
    <td>Binær</td>
    <td>Desi</td>
  </tr>
  <tr>
    <td>A</td>
    <td>1010</td>
    <td>10</td>
  </tr>
  <tr>
    <td>B</td>
    <td>1011</td>
    <td>11</td>
  </tr>
  <tr>
    <td>C</td>
    <td>1100</td>
    <td>12</td>
  </tr>
  <tr>
    <td>1</td>
    <td>0001</td>
    <td>1</td>
  </tr>
  <tr>
    <td>2</td>
    <td>0010</td>
    <td>2</td>
  </tr>
</table>


Når vi har satt opp denne tabellen må vi lime sammen de binære tallene. Det er også viktig at alle de binæretallene har fire sifre. 

1010 + 1011 + 1100 + 0001 + 0010 = 101010111100110. 

Merk at her adderer vi ikke, men setter tallene sammen. Her er det viktig at vi startet med det det binæretallet som tilsvarer det første sifferet i hexadesimaltallet. Dvs, at vi i dette eksempelet starter med A, deretter B, osv.

For å gå fra binære til hex bruker vi så og si samme metode, bare baklengs. Istedenfor å gjøre et hexadesimalt siffer om til et firesifret binærtall, gjør vi et firesifret binærtall om til et hexadesimalt siffer. I motsetning til å starte med det første sifferet, starter vi denne gangen med de fire bakerste. Vi snur ikke om på tallene, men vi leser fra høyre til venstre. 

For eksempel 11 1011 1011:Første tallet blir da 1011, andre blir 1011 og det tredje blir da 0011 (her legger vi på nuller for å få tallet til å bli firesifret). Deretter er det bare å sette de inn i tabellen og finne det tilsvarende hexadesimal sifferet som tilsvarer hvert av de binæretallene

<table>
  <tr>
    <td>Hexa</td>
    <td>Binær</td>
    <td>Desi</td>
  </tr>
  <tr>
    <td>B</td>
    <td>1011</td>
    <td>11</td>
  </tr>
  <tr>
    <td>B</td>
    <td>1011</td>
    <td>11</td>
  </tr>
  <tr>
    <td>3</td>
    <td>0011</td>
    <td>3</td>
  </tr>
</table>


Det hexadesimaletallet blir da BB3

 

**Binær -> desimal -> binær**

 

Å konvertere binærtall til desimal kan bli gjort på følge måte: Lag en tabell hvor du starter med tallet 1 helt til høyre, samt tallet 2 til venstre for det. Det neste tallet i tabellen får du ved å gange det forrige tallet med 2. Tabellen vil da se slik ut:

<table>
  <tr>
    <td>128</td>
    <td>64</td>
    <td>32</td>
    <td>16</td>
    <td>8</td>
    <td>4</td>
    <td>2</td>
    <td>1</td>
  </tr>
  <tr>
    <td> </td>
    <td> </td>
    <td> </td>
    <td> </td>
    <td> </td>
    <td> </td>
    <td> </td>
    <td> </td>
  </tr>
</table>


 

For å få et desimaltall må vi bare sette inn binærtallet i denne tabellen og summere de sammen. For eksempel 110011

 

 

<table>
  <tr>
    <td>128</td>
    <td>64</td>
    <td>32</td>
    <td>16</td>
    <td>8</td>
    <td>4</td>
    <td>2</td>
    <td>1</td>
  </tr>
  <tr>
    <td> </td>
    <td> </td>
    <td>1</td>
    <td>1</td>
    <td>0</td>
    <td>0</td>
    <td>1</td>
    <td>1</td>
  </tr>
</table>


 

Svaret blir da 32+16+2+1= 51

 

 

 

For å gå fra desimal til binær kan vi bruke samme metode som nevnt tidligere, bare vi må gå motsatt vei. Da starter vi med å ta det høyest mulige tallet i tabellen i forhold til desimaltallet vi vil konvertere. Videre er det bare å summere tallene ut i fra tabellen til du oppnår samme sum som desimaltallet

Eksempel på tallet : 203

<table>
  <tr>
    <td>128</td>
    <td>64</td>
    <td>32</td>
    <td>16</td>
    <td>8</td>
    <td>4</td>
    <td>2</td>
    <td>1</td>
  </tr>
  <tr>
    <td>1</td>
    <td>1</td>
    <td>0</td>
    <td>0</td>
    <td>1</td>
    <td>0</td>
    <td>1</td>
    <td>1</td>
  </tr>
</table>


128+64+32+8+2+1=203

 

 

**Oppgave B**

**Beskriv kort metoden for å gå fra hexadesimale tall til desimaltall og motsatt.**

 

**Hex -> desimal -> hex**

 

Metoden vi bruker for å gå fra hex til desimal er å ta det det bakerste sifferet og gange det med grunntallet (16) i nulte potens, det nest bakerste tallet ganger vi med grunntallet i første potens og det tredje tallet ganges med grunntallet i andre potens.

 

Eksempel på tallet BBC:

BBC = ( 11x162 + 11x161 + 12x160) = (2816 + 176 + 12) = 3004

 

Å konvertere desimaltall til hex er litt mer krevende enn den motsatte veien. Det første vi må tenke på er hvor mange sifre det heksadesimale tallet kommer til å ha. Som nevnt ovenfor bruker vi grunntallet 16 og dens potens når vi regner på hexadecimal tall - 162 (256),161, 160. Vi ser ut i fra disse potensene at hvis et desimaltall er mindre enn 256 vil det kun ha to hexadesimale sifre.

La oss ta utgangspunkt i desimaltallet 74. 

Vi starter da med å finne ut hvor mange ganger 16 går opp i 74 (her skal vi ha et helt tall). 

74/16 = 4,625 | Tallet blir da 4 her.

Videre ganger vi det tallet vi fikk (4) med 16.

4*16 = 64

Nå må vi finne differansen mellom 64 og desimaltallet vi skal finne frem til, som er 10. Så langt har vi funnet sifrene 4 og 10. Begge disse sifrene kan skrives på hexadesimaltall. 4 = 4 og 10 = A. Vi ligger disse to sammen og finner svaret 4A. 74 = 4A

