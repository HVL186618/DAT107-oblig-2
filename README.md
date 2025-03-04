# DAT107-oblig-2

Medlem
	• medlemsnr (Primærnøkkel)
		○ varchar
	• fornavn
		○ varchar
	• etternavn
		○ varchar
	• tlf
		○ varchar
	• epost
		○ varchar
	• husnr
		○ int

LokalLag
	• lagnavn
		varchar
	• Ledernavn
		○ varchar
	• postnummer
		○ char
	• husnr
		○ int

MedlemAvgift
	• betalt
		○ varchar
	• år
		○ int
	
	

MedlemAvGift tilhører Medlem
Medlem tilhører LokalLag


Normalisering
1NF: Alle tabellene har atomære verdier, ikke en liste inni en annen.
2NF: 
	• I listen "Medlem": Etternavn er avhengi av Fornavn som ikke er en primærnøkkel.
		○ En kolonne for primærnøkkel.
	• I listen "LokalLag": Lagnavn avhengi av Fornavn/Etternavn?
		○ Hvis man bare har fornavn og det er flere med samme Fornavn i "Medlem" kan det skape forvirrelse.
3NF:
	• "LokalLag" og "MedlemAvgift" har ikke primærnøkkel?
	• Hvis Etternavn er Avhengi av Fornavn som ikke er primærnøkkel så fyller den vel ikke 3NF?

Notater: Usikker på hva jeg skal putte som primær og fremmed på de 3 listene og hva som er avhengig av hva på hva måte.![image](https://github.com/user-attachments/assets/80d52684-3e0c-4170-a1c1-39debd9d9bcf)
