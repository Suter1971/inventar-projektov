OSOBNÉ PROJEKTY – OSTRÁ VERZIA 0.7 (balík č. 23)

Východisko: používateľova ostrá verzia 0.6 (ZIP inventar-projektov-main.zip).

Nové funkcie:
1. Povinný termín dokončenia pri vytváraní/úprave úlohy.
2. Nedokončené úlohy zoradené podľa najbližšieho termínu.
3. Dokončené úlohy na konci zoznamu; pri opätovnom otvorení sa správne zaradia.
4. Nedokončené úlohy po termíne majú svetločervené pozadie a červený termín.
5. Nové označenie cache Service Workera pre bezpečnejšiu aktualizáciu PWA.

ODLOŽENÉ: push notifikácie, registrácia telefónov a pondelkové e-maily.
NIE SÚ súčasťou tohto balíka, nezobrazujú sa ich nefunkčné prepínače.

ZACHOVANÉ: pôvodná vizuálna identita, používateľská databáza, Google prihlasovanie,
Firestore kolekcia changes, lokálny/offline režim, detekcia konfliktov,
JSON import/export a ostatné existujúce funkcie.

NASADENIE:
- Pred nasadením uchovať pôvodný ZIP 0.6 a aktuálny JSON export produkčných údajov.
- Rozbaliť ZIP a nahrať SÚBORY z koreňa balíka do ostrého repozitára
  Suter1971/inventar-projektov (nie do testovacieho).
- Commit changes; vyčkať na publikovanie GitHub Pages (bez záruky presného času).
- Po opätovnom otvorení PWA má byť v pätičke text "Verzia 0.7 PWA · balík 23".
- PWA môže krátko zobrazovať starú verziu v závislosti od cache a aktualizácie SW.

POZOR: Vstupné JSON dáta a Firestore dokumenty týmto balíkom nijako nemeníme.
Existujúce úlohy bez termínu zostanú zachované. Povinný termín sa uplatní
pri vytváraní novej úlohy a pri úprave existujúcej úlohy.

Ak treba vrátiť predchádzajúcu aplikáciu, obnoviť pôvodné súbory 0.6
v ostrom repozitári. Pred prípadnou obnovou údajov zvážiť, že import JSON
prepisuje súčasnú inventúru. Samotný návrat kódu databázu nevracia.
