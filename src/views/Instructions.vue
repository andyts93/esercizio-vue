<template>
  <div class="instructions">
      <el-card>
          <div slot="header">
              <h3 class="m-0">Indicazioni generali</h3>
          </div>
          <ul>
              <li>Dovranno essere utilizzati gli elementi messi a disposizione della libreria <a href="https://element.eleme.io/#/en-US/component/installation" target="_blank">Element</a></li>
              <li>L'installazione della libreria è già stata effettuata</li>
              <li>Siete liberi di installare componenti/librerie aggiuntive</li>
              <li>Siete liberi di integrare quanto richiesto con delle migliorie</li>
              <li>Generare una chiave lanciando dal terminale questo comando: <code>head -n 4096 /dev/urandom | openssl sha1 | cut -c1-8</code></li>
              <li>Il lavoro dovrà essere svolto su un branch apposito partendo da master e chiamandolo <em><strong>esercizio/[chiave]</strong></em></li>
          </ul>
      </el-card>
    <el-card class="mt-2">
      <div slot="header">
        <h3 class="m-0">Tabella</h3>
      </div>
      <ol>
        <li>Creare una nuova pagina e linkarla nel menu</li>
        <li>
          All'interno inserire una tabella con le seguenti colonne:
          <ul>
            <li>Nome</li>
            <li>Cognome</li>
            <li>Età</li>
            <li>Email</li>
            <li>Telefono</li>
              <li>Data apertura conto</li>
            <li>Conto (formattato in valuta euro)</li>
          </ul>
        </li>
        <li>
          Ogni elemento della tabella dovrà essere selezionabile tramite una
          checkbox
        </li>
        <li>Ogni colonna dovrà essere ordinabile</li>
        <li>Inserire un filtro su nome, cognome e email</li>
      </ol>
    </el-card>
    <el-card class="mt-2">
      <div slot="header">
        <h3 class="m-0">Form</h3>
      </div>
      <ol>
        <li>
          Aggiungere un bottone alla pagina <em>Tabella</em> per aggiungere un
          nuovo utente
        </li>
        <li>
          Al click dovrà aprirsi un <em>dialog</em> con il form di aggiunta, dal
          quale sarà possibile inserire tutti i campi utente
        </li>
        <li>
          Tutti i campi dovranno essere obbligatori e i dati dovranno essere
          così verificati:
          <ul>
            <li>Nome: campo di testo con massimo 20 caratteri</li>
            <li>Cognome: campo di testo con massimo 30 caratteri</li>
            <li>Età: campo numerico, l'utente dovrà avere almeno 18 anni</li>
            <li>Email: campo email</li>
            <li>Telefono: campo numerico</li>
              <li>Data apertura conto: datepicker</li>
            <li>
              Conto: campo numerico, l'utente dovrà avere un conto che va da un
              minimo di 100€ a un massimo di 2000€
            </li>
          </ul>
          <strong
            >Nel caso non vengano rispettate queste regole l'utente non potrà
            essere salvato.</strong
          >
        </li>
      </ol>
    </el-card>
      <el-card class="mt-2">
          <div slot="header">
              <h3 class="m-0">Operazioni tabella</h3>
          </div>
          <ol>
              <li>Aggiungere una colonna alla tabella per effettuare operazioni sulle righe</li>
              <li>Inserire in questa colonna un bottone per eliminare e uno per modificare l'utente</li>
              <li>Il bottone di eliminazione dovrà chiedere conferma prima di eliminare l'utente</li>
              <li>Il bottone di modifica dovrà aprire il <em>dialog</em> creato in precedenza con i dati dell'utente pre-compilati e il salvataggio dovrà andare a modificare l'utente</li>
          </ol>
      </el-card>
  </div>
</template>
