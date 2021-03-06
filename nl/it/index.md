---

copyright:
  years: 2016, 2018
lastupdated: "2018-05-08"

---

{:new_window: target="_blank"}
{:shortdesc: .shortdesc}
{:screen: .screen}
{:codeblock: .codeblock}
{:pre: .pre}

# Introduzione a {{site.data.keyword.iot_short_notm}}
{: #gettingstartedtemplate}

{{site.data.keyword.iot_full}} per {{site.data.keyword.Bluemix_notm}} ti fornisce un toolkit versatile che include i dispositivi gateway, la gestione del dispositivo e l'accesso all'applicazione potente. Utilizzando {{site.data.keyword.iot_short_notm}}, puoi collegare i dati dei dispositivi connessi ed eseguire analisi dei dati in tempo reale per la tua organizzazione.
{:shortdesc}

## Prima di cominciare
{: #byb}

Prima di collegare i dispositivi utilizzando i dati, registra un account {{site.data.keyword.Bluemix_notm}} e crea un'istanza del servizio {{site.data.keyword.iot_short_notm}} nella tua organizzazione {{site.data.keyword.Bluemix_notm}}. Puoi creare un'istanza {{site.data.keyword.iot_short_notm}} direttamente dalla pagina [{{site.data.keyword.iot_short_notm}} nel catalogo dei servizi IBM Cloud ![Icona link esterno](../../icons/launch-glyph.svg "Icona link esterno")](https://console.{DomainName}/catalog/services/internet-of-things-platform/){:new_window}.  

Per informazioni dettagliate su come registrare un account in {{site.data.keyword.Bluemix_notm}}, configura le regioni e le altre impostazioni di gestione dell'account, consulta [Gestione del tuo account IBM Cloud](https://console.ng.bluemix.net/docs/admin/account.html#signup).

Puoi configurare la tua istanza {{site.data.keyword.iot_short_notm}} dal dashboard. Per aprire il dashboard, vai alla tua istanza del servizio {{site.data.keyword.iot_short_notm}} in  {{site.data.keyword.Bluemix_notm}} e fai quindi clic su **Launch**.

## Informazioni su quest'attività

Le seguenti istruzioni illustrano come puoi velocemente iniziare ad utilizzare il tuo servizio {{site.data.keyword.iot_short_notm}}.

È anche disponibile una serie più dettagliata di guide introduttive e di applicazioni di esempio che guidano attraverso le basi dello sviluppo di un sistema prototipo IoT end-to-end pronto per la produzione con {{site.data.keyword.iot_short_notm}}. Se sei uno sviluppatore che non ha dimestichezza con l'utilizzo di {{site.data.keyword.iot_short_notm}}, utilizza i processi passo dopo passo nella sezione [Guide introduttive](https://console.bluemix.net/docs/services/IoT/getting_started/getting-started-iot-overview.html#getting-started).

## Passo 1: Collega i tuoi dispositivi
{: #up_and_running}

Per essere operativo con il servizio, esplora le seguenti opzioni in base alla tua situazione.

|  |   Il servizio è stato distribuito | Il servizio non è stato distribuito
 | -------------| ------------- | -------------
  |**Ho un dispositivo da collegare** | [Collega il tuo dispositivo a {{site.data.keyword.iot_short_notm}}](iotplatform_task.html#iotplatform_task).| Esplora la connessione del dispositivo in [Play with {{site.data.keyword.iot_short_notm}} ![Icona link esterno](../../icons/launch-glyph.svg "Icona link esterno")](http://discover-iot.eu-gb.mybluemix.net/?cm_mc_uid=44491599487314618721024&cm_mc_sid_50200000=1462798151#/play){:new_window}.
  |**Non ho un dispositivo da collegare** | [Crea e collega un simulatore del dispositivo Node-RED](nodereddevice_sample.html){:new_window}. O [Connect your Smartphone ![Icona link esterno](../../icons/launch-glyph.svg "Icona link esterno")](http://discover-iot.eu-gb.mybluemix.net/?cm_mc_uid=44491599487314618721024&cm_mc_sid_50200000=1462798151#/play/device/smartphone){:new_window}. | Introduzione a [Watson IoT Platform Starter](https://console.bluemix.net/docs/starters/IoT-starter/iot500.html).
  
Per ulteriori informazioni su come collegare tipi di dispositivi specifici a {{site.data.keyword.iot_short_notm}}, consulta [developerWorks recipes ![Icona link esterno](../../icons/launch-glyph.svg "Icona link esterno")](https://developer.ibm.com/recipes/tutorials/category/internet-of-things-iot/){:new_window}.  

Per la documentazione dello sviluppatore per la connessione del dispositivo, consulta:
- [Connettività MQTT per i dispositivi](devices/mqtt.html).
- [Connettività MQTT per i gateway](gateways/mqtt.html).

<!--
## Step 2: Analyze your device data
{: #analyzing_data}
Start exploring the real-time data that the devices are sending to {{site.data.keyword.iot_short_notm}}.
{{site.data.keyword.iot_short_notm}} includes the following analytics tools:  
- [Boards and cards](data_visualization.html) to visualize your real-time device data.
- [Rules and actions](analytics.html) that are triggered by real-time device data.
For a quick getting started example, see the [Using Rules and Actions with IBM Watson IoT Platform Cloud Analytics ![External link icon](../../icons/launch-glyph.svg "External link icon")](https://developer.ibm.com/recipes/tutorials/using-rules-and-actions-with-ibm-watson-iot-platform-cloud-analytics/){:new_window} developerWorks recipe.
-->

## Passo 2: Crea applicazioni che utilizzano i tuoi dati del dispositivo
{: #develop_applications}

Crea e collega le tue applicazioni per utilizzare i dati del dispositivo. 

Per ulteriori informazioni, consulta i seguenti argomenti:   
- Esplora la [documentazione dello sviluppatore dell'applicazione](applications/api.html) e la documentazione API [{{site.data.keyword.iot_short_notm}}](reference/api.html).
- Esplora le [librerie client {{site.data.keyword.iot_short_notm}}](iot_platform_client_lib.html) che forniscono gli strumenti e i file per creare e sviluppare il codice per l'integrazione e la connettività dei tuoi dispositivi e applicazioni.
- [Collega il servizio {{site.data.keyword.cloudantfull}}](cloudant_connector.html) al tuo {{site.data.keyword.iot_short_notm}} per archiviare i dati del dispositivo cronologici.
- Crea le tue regole utilizzando la nuova funzione delle [regole integrate (Beta)](information_management/im_rules.html).
