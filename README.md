Sistem Expert pentru Recomandarea unui Plan Alimentar Personalizat

Acest proiect reprezintă un sistem expert bazat pe reguli conceput pentru a genera recomandări nutriționale personalizate.
Sistemul utilizează algoritmul de inferență Forward Chaining pentru a procesa datele utilizatorului și a oferi un plan alimentar orientativ, incluzând necesarul caloric, distribuția macronutrienților și recomandări de hidratare.

🚀 Caracteristici principale
Calcul de indicatori biometrici: Determină automat BMI, BMR și TDEE pe baza profilului utilizatorului.
Motor de inferență: Implementează un algoritm de tip Forward Chaining în JavaScript care rulează până la atingerea unui punct fix.
Bază de cunoștințe flexibilă: Regulile sunt stocate extern într-un format JSON, permițând actualizarea ușoară a logicii nutriționale.
Interfață React Modernă: Formular intuitiv cu validare de date și afișare dinamică a rezultatelor sub formă de carduri.
Transparență (Inference Log): Utilizatorul poate vizualiza jurnalul detaliat al pașilor de inferență și regulile care au fost activate.

🛠️ Tehnologii utilizate
Frontend: React (Hooks, Functional Components).
Logica de calcul: JavaScript (ES6+).Stocare date: JSON pentru baza de cunoștințe.
Stilizare: Componente personalizate (ChoiceCard, SelectButtonGroup).

📋 Structura Sistemului
1. Baza de Cunoștințe (JSON)
Este structurată în trei secțiuni:
facts_schema: Definește tipurile de date și domeniile de valori.
intermediate_facts: Conține formulele matematice pentru derivarea datelor (ex: formula pentru BMR diferențiată pe sex).
rules:Un set de 17 reguli IF-THEN cu priorități diferite (1–7) ce acoperă clasificarea BMI, ajustările de vârstă și distribuția macronutrienților.

2. Mașina de Inferență
Funcționează în patru etape principale:
Calcul inițial: Generarea faptelor intermediare din datele brute.
Sortare: Ordonarea regulilor după prioritate.
Execuție (While Loop): Aplicarea repetată a regulilor prin funcțiile ruleMatches() și applyConclusion().
Ajustare finală: Aplicarea corecțiilor specifice (ex: vârstă).

⚠️Limitări și Atenționări
Sistemul este un instrument educațional și oferă estimări cu marjă de eroare.
Nu înlocuiește consultul medical specializat, neavând reguli pentru cazuri precum diabetul, boli cardiovasculare sau sarcină.
Nu ia în calcul alergiile sau preferințele alimentare specifice.

🔮 Dezvoltări ulterioare
Extinderea bazei de cunoștințe pentru cazuri medicale.
Generarea automată a unui plan de mese săptămânal.
Implementarea unui sistem de autentificare și istoric al progresului.

