# <p align = "center">DistilBERT model i analiza sentimenta teksta</p> 

Projekat ima za cilj da predstavi DistilBERT model mašinskog učenja koji se koristi za obradu prirodnog jezika (NLP) i demonstrira primenu istog prilikom analize sentimenta teksta.

Ovaj rad predstavlja završni projekat kursa Mašinsko učenje 2022. godine na Matematičkom fakultetu, Univerziteta u Beogradu.

**Autori:** Jelena Radojević (broj indeksa: 1007/2021) i Ilija-Petar Milić (broj indeksa: 1053/2021)



## <p align = "center">Sadržaj:</p> 

### 01 - Teorija

Na samom početku uvode se osnovni koncepti: mehanizam pažnje, enkoder i transformeri, koji čine temelj za dalji rad. U nastavku, oslanjajući se na prethodno definisane pojmove, formalno se uvodi BERT (Bidirectional Encoder Representations from Transformers) model i opisuje način na koji on funkcioniše. Definiše se opšti postupak destilacije modela mašinskog učenja i prikazuje njegova primena na BERT model što za rezultat daje DistilBERT.

### 02 - Analiza podataka

Podaci sa kojima se radi predstavljaju komentare sa stranice [*Wikipedia*](https://www.wikipedia.org/) koji su klasifikovani, od strane ljudi, u zavisnosti od tipa neprikladnosti njihovog sadržaja. Reč je o multi-labelarnoj klasifikaciji, ona podrazumeva da svaka instanca može istovremeno biti član jedne ili više klasa. Sam skup podataka korišćen je prilikom takmičenja [*Toxic Comment Classification Challenge*](https://www.kaggle.com/c/jigsaw-toxic-comment-classification-challenge/) na platformi *Kaggle*. Ovaj deo rada posvećen je analizi skupa podataka koja obuhvata određivanje relevantnih (statističkih) svojstava koja će biti od koristi prilikom formiranja modela u nastavku.


### 03 - Model

Na samom početku obavljena je odgovarajuća priprema i podela podataka na koji će se koristiti prilikom treninga i evaluacije modela. U nastavku je definisana arhitektura DistilBERT modela konfigurisanog za problem analize sentimenta teksta, odnosno u ovom slučaju klasifikaciju neprikladnih komentara. U nastavku se model trenira i vrši se evaluacija njegovih performansi uz analizu dobijenih rezultata.


## <p align = "center">Pokretanje:</p> 
Rad je implementiran u sklopu jupyter svesaka i pre pokretanja samog koda neophodno je instalirati nestandardne biblioteke sledećim komandama:

`pip install transformers`

`pip install scikit-multilearn`



## <p align = "center">Literatura:</p> 

[Attention Is All You Need](https://arxiv.org/abs/1706.03762)

[BERT: Pre-training of Deep Bidirectional Transformers for Language Understanding](https://arxiv.org/abs/1810.04805v2)

[DistilBERT, a distilled version of BERT: smaller, faster, cheaper and lighter](https://arxiv.org/abs/1910.01108)

[Smaller, faster, cheaper, lighter: Introducing DistilBERT, a distilled version of BERT](https://medium.com/huggingface/distilbert-8cf3380435b5)

[A Beginner’s Guide to Exploratory Data Analysis (EDA) on Text Data](https://www.analyticsvidhya.com/blog/2020/04/beginners-guide-exploratory-data-analysis-text-data/)

