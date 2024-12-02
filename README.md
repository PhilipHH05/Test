# Regex för att hitta fakturanummer som slutar på siffran "3"

Den här filen förklarar en **regex** (regelbundna uttryck) som hittar rader i en text där ett fakturanummer slutar på siffran "3". Du kan använda denna regex för att filtrera eller hitta specifika rader i fakturalistor eller liknande data.

## Regex-kod

```regex

^\s*FakturaNr: \d*3\s*$
^: Början av raden. Vi börjar söka från första tecknet.
\s*: Matchar alla mellanslag i början av raden.
FakturaNr:: Exakt texten "FakturaNr:". Vi letar efter denna text.
\d*: Matchar alla siffror som kommer efter "FakturaNr:".
3: Matchar siffran 3. Fakturanumret måste sluta på denna siffra.
\s*: Matchar eventuella mellanslag efter siffran "3".
$: Slutet av raden. Vi ser till att inget kommer efter siffran "3".
