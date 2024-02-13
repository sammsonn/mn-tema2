**Nume: SAMSON Alexandru-Valentin** 
**Grupă: 312CC** 
 
 
## Tema 2 – Metode Numerice pentru funcții 
 
 
### Descriere: 
 
## Task 1 
 
* Se aplică algoritmul de descompunere în valori singulare (SVD) asupra matricei 
"photo", rezultând trei matrice: "U", "S" și "V". 
 
* Matricile "U", "S" și "V" sunt utilizate pentru a calcula matricile reduse: 
"U_k" (conține primele k coloane ale lui U), "S_k" (conține submatricea de 
dimensiune k x k din partea stânga-sus a lui S) și "V_k" (conține primele k 
coloane ale lui V). 
 
* Aproximarea matricei inițiale "photo", denumită "new_X", este calculată prin 
înmulțirea matricilor "U_k", "S_k" și transpusa lui "V_k". 
 
## Task 2 
 
* Se calculează media fiecărui rând al matricei "photo" și se stochează 
rezultatul în variabila "mean_row". 
 
* Matricea "photo" este ajustată prin scăderea mediei de pe fiecare rând. 
 
* Se construiește matricea "Z" ca transpusa matricei ajustate "photo". 
 
* Se aplică descompunerea în valori singulare (SVD) matricei "Z", obținându-se 
trei matrici: "U", "S" și "V". 
 
* Se construiește matricea "W" din primele "pcs" coloane ale matricei "V". 
 
* Se calculează matricea "Y" ca produsul dintre transpusa matricei "W" și 
matricea ajustată "photo". 
 
* Se aproximează matricea inițială, "new_X", prin înmulțirea matricelor "W" și 
"Y" și adăugarea mediei pe fiecare rând. 
 
## Task 3 
 
* Se calculează media fiecărui rând al matricei "photo" și se stochează 
rezultatul în variabila "mean_row". 
 
* Matricea "photo" este ajustată prin scăderea mediei de pe fiecare rând. 
 
* Se calculează matricea de covarianță "Z" prin înmulțirea matricei ajustate 
"photo" cu transpusa sa și împărțirea rezultatului la (n - 1), unde "n" 
reprezintă numărul de coloane al matricei. 
 
* Se calculează vectorii și valorile proprii ale matricei de covarianță "Z" 
utilizând funcția "eig". 
 
* Valorile proprii sunt ordonate în ordine descrescătoare, iar matricea "V" 
este construită astfel încât să conțină vectorii proprii corespunzători 
valorilor proprii ordonate. 
 
* Se păstrează doar primele "pcs" coloane din matricea "V". 
