# <p align = "center">DistilBERT model i analiza sentimenta teksta</p> 

Projekat ima za cilj da predstavi DistilBERT model mašinskog učenja koji se koristi za obradu prirodnog jezika (NLP) i demonstrira primenu istog prilikom analize sentimenta teksta.

Ovaj rad predstavlja završni projekat kursa [Mašinsko učenje](http://ml.matf.bg.ac.rs) 2022. godine na [Matematičkom fakultetu](http://www.matf.bg.ac.rs/), [Univerziteta u Beogradu](https://bg.ac.rs/).

**Autori:** Jelena Radojević (broj indeksa: 1007/2021) i Ilija-Petar Milić (broj indeksa: 1053/2021)



## <p align = "center">Sadržaj:</p> 

### 01 - Teorija

Na samom početku uvode se osnovni koncepti: mehanizam pažnje, enkoder i transformeri, koji čine temelj za dalji rad. U nastavku, oslanjajući se na prethodno definisane pojmove, formalno se uvodi [BERT](https://en.wikipedia.org/wiki/BERT_(language_model)) (Bidirectional Encoder Representations from Transformers) model i opisuje način na koji on funkcioniše. Definiše se opšti postupak destilacije modela mašinskog učenja i prikazuje njegova primena na BERT model što za rezultat daje DistilBERT model.

### 02 - Analiza podataka

Podaci sa kojima se radi predstavljaju komentare sa stranice [*Wikipedia*](https://www.wikipedia.org/) koji su klasifikovani, od strane ljudi, u zavisnosti od tipa neprikladnosti njihovog sadržaja. Reč je o multi-labelarnoj klasifikaciji, ona podrazumeva da svaka instanca može istovremeno biti član jedne ili više klasa. Sam skup podataka korišćen je prilikom takmičenja [*Toxic Comment Classification Challenge*](https://www.kaggle.com/c/jigsaw-toxic-comment-classification-challenge/) na platformi *Kaggle*. Ovaj deo rada posvećen je analizi skupa podataka koja obuhvata određivanje relevantnih (statističkih) svojstava koja će biti od koristi prilikom formiranja modela u nastavku.


### 03 - Model

Na samom početku obavljena je odgovarajuća priprema i podela podataka na koji će se koristiti prilikom treninga i evaluacije modela. U nastavku je definisana arhitektura DistilBERT modela konfigurisanog za problem analize sentimenta teksta, odnosno u ovom slučaju klasifikaciju neprikladnih komentara. U nastavku se model trenira i vrši se evaluacija njegovih performansi uz analizu dobijenih rezultata.


## <p align = "center">Pokretanje:</p> 
Rad je implementiran u sklopu jupyter svesaka i pre pokretanja samog koda neophodno je instalirati nestandardne biblioteke sledećim komandama:

`pip install transformers`

`pip install scikit-multilearn`



## <p align = "center">Literatura:</p> 

[Attention Is All You Need](https://arxiv.org/pdf/1706.03762.pdf)

[BERT: Pre-training of Deep Bidirectional Transformers for Language Understanding](https://arxiv.org/pdf/1810.04805v2.pdf)

[DistilBERT, a distilled version of BERT: smaller, faster, cheaper and lighter](https://arxiv.org/pdf/1910.01108.pdf)

[The Illustrated BERT](https://jalammar.github.io/illustrated-bert/)

[A Visual Guide to Using BERT for the First Time](https://jalammar.github.io/a-visual-guide-to-using-bert-for-the-first-time/)

[Smaller, faster, cheaper, lighter: Introducing DistilBERT, a distilled version of BERT](https://medium.com/huggingface/distilbert-8cf3380435b5)

[A Beginner’s Guide to Exploratory Data Analysis (EDA) on Text Data](https://www.analyticsvidhya.com/blog/2020/04/beginners-guide-exploratory-data-analysis-text-data/)

[Hugging Face Transformers: Fine-tuning DistilBERT for Binary Classification Tasks](https://towardsdatascience.com/hugging-face-transformers-fine-tuning-distilbert-for-binary-classification-tasks-490f1d192379)


