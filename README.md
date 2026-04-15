# detekcija-pneumonije-projekt
Kolegij: Obrada slike i računalni vid, diplomski studij Računarstvo, mentor: Marin Benčević

## Opis projekta: 
Ovaj projekt istražuje primjenu aktivnog učenja (Active Learning) u kombinaciji s prijenosnim učenjem (Transfer Learning) za detekciju pneumonije na rendgenskim snimkama pluća. Glavni cilj bio je usporediti učinkovitost pametnog odabira podataka (strategije nesigurnosti) u odnosu na standardno nasumično uzorkovanje.
<img width="1489" height="428" alt="image" src="https://github.com/user-attachments/assets/b75543f1-2615-4103-9e00-a59d45b096e4" />
<img width="1489" height="400" alt="image" src="https://github.com/user-attachments/assets/f7a9233b-5f18-4cf3-b156-87b55a1a243c" />



## Korištene tehnologije: 
- Python
- Google Colab
- PyTorch
- osnovna arhitektura za prijenosno učenje: VGG16
- Kaggle dataset: https://www.kaggle.com/datasets/paultimothymooney/chest-xray-pneumonia

## Glavna motivacija:
Cilj ovog pristupa je razvoj sustava koji od stručnjaka traži intervenciju samo kod graničnih slučajeva, čime se optimizira radni proces u radiologiji.

## Glavne funkcionalnosti:
- Implementacija Aktivnog Učenja (Human-in-the-loop): Razvijen sustav koji iterativno odabire najinformativnije neoznačene primjere za anotaciju, umjesto nasumičnog odabira podataka.
- Strategije nesigurnosti (Uncertainty Sampling): Korištenje naprednih metoda odabira podataka (poput least confidence ili entropy) kako bi model učio na "teškim" slučajevima koje sustav ne prepoznaje s visokom sigurnošću.
- Komparativna analiza performansi: Provedena detaljna usporedba između aktivnog učenja i tradicionalnog učenja (Random Sampling), dokazujući superiornost AL-a u uvjetima s ograničenim brojem podataka.
- Prijenosno učenje (Transfer Learning): Korištenje pretreniranih arhitektura neuronskih mreža optimiziranih za rad s medicinskim slikama (X-ray snimke pluća).
- Robusna evaluacija medicinskih metrika: Analiza modela nije ograničena samo na točnost (Accuracy), već je fokus na odzivu (Recall) i F1-mjeri, što je kritično za smanjenje lažno negativnih rezultata u medicinskoj dijagnostici.
- Efikasnost resursa: Postizanje visokih performansi modela sa svega 100 označenih uzoraka, simulirajući realne uvjete u kojima je rad liječnika (anotatora) skup i vremenski ograničen.
- Vizualizacija rezultata: Integrirani grafički prikazi krivulja učenja koji zorno prikazuju brzinu konvergencije modela kroz iteracije aktivnog učenja.

## Pokretanje projekta:
Poveznica na originalni programski kod i replikaciju eksperimenta: https://colab.research.google.com/drive/1pUwzNZyrKn3oheruNbkOzbNNRQJwGLVQ#scrollTo=ZGmyf6oRUMMq

## Rezultati:
Detaljan opis i analiza rezultata prikazani su u poglavlju pod brojem 3.

<img width="1990" height="1190" alt="image" src="https://github.com/user-attachments/assets/19cee60c-1bed-4e75-833d-e0d9d86bcfb6" />


## Autor:
Ivona Pranjić
