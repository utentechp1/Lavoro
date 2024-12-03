# Lavoro

https://bitbucket.org/
https://www.sourcetreeapp.com/

Logo di Sourcetree  
Scarica gratis  
Prossimo: Impara Sourcetree con Bitbucket  

### Passaggio 1: Crea un repository Git  

#### Passaggio 1: Crea il repository  
Come nuovo amministratore della stazione spaziale Bitbucket, è importante essere organizzati. Quando crei file per la tua stazione spaziale, vorrai tenerli in un unico posto e condividerli con il tuo team, ovunque essi siano nell'universo. In Bitbucket, questo significa aggiungere tutto a un repository. Creiamone uno!  

##### Creare il repository  
Il repository che crei in Bitbucket sarà inizialmente vuoto, senza codice. Va bene così, perché presto inizierai ad aggiungere file. Questo repository sarà il centro di gestione per i tuoi file, accessibile ad altri se darai loro il permesso. Copierai una versione del repository nel tuo sistema locale, così da poter aggiornare e sincronizzare i cambiamenti tra i due.  

**Procedura:**  

1. In Bitbucket, clicca sull'icona `+` nella barra laterale globale e seleziona **Repository**. Verrà visualizzata la pagina **Crea un nuovo repository**.  
2. Inserisci **BitbucketStationSupplies** nel campo **Nome**. Bitbucket utilizzerà questo nome nell'URL del repository (ad es. `https://bitbucket.org/utente/repository`).  
3. Mantieni le altre opzioni di default:  
   - **Livello di accesso**: Assicurati che la casella **Repository privato** sia selezionata.  
   - **Includere un file README?**: Scegli un'opzione **Sì** per iniziare con un file.  
   - **Sistema di controllo di versione**: Se non sei sicuro, lascia Git come opzione.  
4. Clicca su **Crea repository**. Bitbucket creerà il repository e ne mostrerà la pagina **Sorgente**.  

---

### Passaggio 2: Copia il tuo repository e aggiungi file  

Per gestire i tuoi file, hai bisogno di copiarli sul tuo sistema locale. Sourcetree definisce questo processo "clonare" un repository.  

#### Passaggio 1: Clona il repository  

1. Crea una cartella chiamata `repos` sul tuo sistema locale per organizzare i tuoi repository.  
2. In Bitbucket, vai al repository **BitbucketStationSupplies** e clicca su **Clona**.  
3. Nella finestra **Clona questo repository**, seleziona **Clona in Sourcetree**.  
4. Nella finestra di dialogo **Clone New**, aggiorna il percorso di destinazione alla cartella appena creata.  
5. Clicca su **Clona**.  

Ora hai clonato il repository sul tuo sistema locale.  

---

### Passaggio 3: Usa i branch di Sourcetree per fondere un aggiornamento  

I branch ti consentono di lavorare su aggiornamenti separati senza interferire con il lavoro principale. Quando sei pronto, puoi unire il branch al branch principale.  

#### Passaggio 1: Crea un branch  

1. In Sourcetree, clicca su **Branch**.  
2. Assegna al branch il nome `wish-list`.  
3. Aggiungi un elemento al file `supplyrequest` (ad es. **anti-gravity speakers**) e salvalo.  
4. Effettua il commit delle modifiche nel branch.  

#### Passaggio 2: Unisci i cambiamenti  

1. Torna al branch principale in Sourcetree.  
2. Clicca su **Unisci** e seleziona il commit da unire.  
3. Completa il processo di merge e clicca su **Commit** (se necessario).  

---

Ora che hai familiarizzato con Bitbucket e Sourcetree, sei pronto per gestire le attività della tua stazione spaziale in modo più efficiente!
