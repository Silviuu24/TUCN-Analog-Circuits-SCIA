# Interfață de Condiționare a Semnalelor Analogice ⚡📉

![LTspice](https://img.shields.io/badge/Simulare-LTspice-red)
![Hardware](https://img.shields.io/badge/Hardware-Breadboard-blue)
![Curs](https://img.shields.io/badge/Curs-SCIA_UTCN-green)

## 📌 Descrierea Proiectului
Acest repository conține proiectarea, simularea și implementarea fizică a unui circuit analogic format din patru etaje distincte. 

Proiectul a fost realizat în cadrul disciplinei **Sisteme cu Circuite Integrate Analogice (SCIA)**, anul III, la Universitatea Tehnică din Cluj-Napoca (UTCN). Obiectivul principal este condiționarea unui semnal analogic trecându-l prin etaje de amplificare, filtrare activă și redresare, confirmând teoria prin simulări și măsurători practice.

## 🏗️ Arhitectura Sistemului
Circuitul este compus din următoarele 4 etaje în cascadă:
1. **Etajul 1 - Amplificator de instrumentație:** Realizat cu 2 AO (inversor), configurat pentru a oferi un câștig liniar de 3.
2. **Etajul 2 - Filtru activ Sallen-Key Trece-Jos:** Proiectat pentru o frecvență de tăiere de 7 kHz, un factor de calitate Q = 1 și un câștig liniar în banda de trecere de 1.
3. **Etajul 3 - Amplificator cu câștig programabil (PGA):** Configurație serie, neinversoare, ce oferă 4 trepte de amplificare selectabile cu ajutorul unui multiplexor: 8 dB, 10 dB, 12 dB și 14 dB.
4. **Etajul 4 - Redresor monoalternanță:** Amplifică exclusiv alternanța pozitivă a semnalului cu un câștig de 2.

## 🛠️ Componente și Unelte Utilizate
* **Software Simulare:** LTspice (Analize .op, AC Sweep, Transient, Fourier / THD)
* **Implementare Hardware:** Breadboard, sursă de alimentare diferențială, generator de semnal, osciloscop.
* **Componente Active (Practic):** Amplificatoare operaționale OP482, LT1357, AMP03 și multiplexor MAX4617.
* **Componente Pasive:** Rezistențe cu toleranță mică (1%) și condensatoare ceramice.

## 📸 Implementare Hardware
![Circuit](https://github.com/user-attachments/assets/43a2c387-4cb0-4ada-ae12-e1e4b7010afe)

## 📊 Rezultate și Documentație Tehnică
Sistemul a fost caracterizat complet, analizându-se atât teoretic (Bode, CMRR, PSRR, Slew Rate, THD), cât și practic influența elementelor parazite și a toleranțelor componentelor fizice. Funcționarea circuitului respectă cu mare precizie specificațiile inițiale.

Pentru detalii complete despre calculele de dimensionare (matematice), schemele LTspice și analiza erorilor, vă rog să consultați documentația integrală:
📄 [Documentație Completă Proiect SCIA (PDF)](Docs/Proiect_SCIA.pdf)
