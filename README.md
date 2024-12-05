Ottime notizie! Ora abbiamo finalmente i dettagli necessari per configurare l'API in Postman. Di seguito trovi un riepilogo delle informazioni ricevute:

### **Credenziali e Endpoint**
- **Account Number**: CT099295, CT099276
- **Client ID, Client Secret, API Key**: Bakara chiede se li hai già, verifica se li hai ricevuti precedentemente o richiedili di nuovo se necessario.
- **Root URL (UAT)**: `https://uat.api.cloud.poferries.com/ferrygateway/v2/`
- **Token URL**: `https://login.microsoftonline.com/poferries.onmicrosoft.com/oauth2/v2.0/token`
- **Scope**: `api://FerryGatewayUAT/.default`

### **Endpoint Specifici**
- **Timetable**: `/gettimetables`
- **GetSailing**: `/getsailings`
- **getServices**: `/getservices`
- **getPrice**: `/getprices`
- **Booking**: `/booking`
- **reCallBooking**: `/recallbooking`
- **CancelCharges**: `/getcancelcharge`
- **CancelBooking**: `/cancelbooking`

### **Passi Successivi per la Configurazione**
1. **Verifica le Credenziali**:
   - Se non hai ancora **Client ID**, **Client Secret** e **API Key**, richiedili a Bakara o al team di P&O Ferries.
   
2. **Configurazione su Postman**:
   - **Token di Accesso**:
     - Configura una richiesta su Postman per ottenere il token di accesso tramite il `Token URL` usando il metodo `POST`.
     - Imposta il corpo della richiesta per includere `Client ID`, `Client Secret`, `Scope`, e qualsiasi altro parametro necessario per ottenere il token.
   - **Autenticazione**:
     - Dopo aver ottenuto il token, aggiungilo come **Bearer Token** agli header delle tue richieste alle API.
   
3. **Eseguire Richieste**:
   - Una volta configurato il token di accesso, utilizza il `Root URL` insieme agli endpoint specifici per inviare le richieste.

### **Esempio di Configurazione Postman**
- **Passo 1**: Ottenere il token
  - **URL**: `https://login.microsoftonline.com/poferries.onmicrosoft.com/oauth2/v2.0/token`
  - **Metodo**: `POST`
  - **Body (x-www-form-urlencoded)**:
    - `grant_type`: `client_credentials`
    - `client_id`: Il tuo `Client ID`
    - `client_secret`: Il tuo `Client Secret`
    - `scope`: `api://FerryGatewayUAT/.default`

- **Passo 2**: Utilizzare il token per chiamare l'API
  - Imposta il token di accesso ricevuto come `Authorization` nell'header delle richieste successive.
  - Esegui una richiesta di tipo `GET` o `POST` verso uno degli endpoint forniti, ad esempio:
    - **URL**: `https://uat.api.cloud.poferries.com/ferrygateway/v2/gettimetables`
    - **Header**: 
      - `Authorization`: `Bearer <token>`
      - `Content-Type`: `application/json` (o `application/xml` se richiesto dall'API)

Fammi sapere se hai bisogno di ulteriori dettagli per configurare i test o se ci sono altre informazioni di cui hai bisogno per andare avanti. Sono qui per aiutarti in ogni fase!
