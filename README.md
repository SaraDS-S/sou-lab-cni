# sou-lab-cni
# Creazione di un progetto multinodo automatica

Questo progetto serve a creare e configurare un infrastruttura multinodo utilizzando Vagrant, il tutto automatizzato tramite Ansible.


## Funzionalità

- Creazione automatizzata delle macchine virtuali
- Configurazione completa delle macchine tramite template ansible
- Bilanciamento del carico con HaProxy
- Monitoraggio con Prometheus e visualizzazione metriche con Grafana


## Lista delle tecnologie utilizate

- Vagrant: gestione delle VM e infrastruttura multinodo
- Ansible: automatizzare la creazione e configurazione delle VM
- HaProxy: bilanciatore per Prometheus & Grafana
- Prometheus: monitoraggio del sistema
- Grafana: visualizzazione dei dati di monitoraggio raccolti da Prometheus


## Prerequisiti

Installa Vagrant e VirtualBox tramite i loro siti ufficiali.


### Ansible

In questo caso è stato creato un role in modo da gestire playbook multipli per la configurazione delle macchine.



### Installazione e avvio

1. Avvia la creazione delle macchine virtuali attraverso l'utilizzo del terminale, spostandoti nel path /sou-lab-cni/vagrant/ e digitando 'vagrant up'

2. Da questo momento in poi tutta l'installazione è automatizzata. Nel caso si volesse fermare la VM avviata, digitare 'vagrant suspend' seguito dal nome della VM da stoppare

3. Nel caso si volesse cancellare la VM digitare 'vagrant destroy' seguito dal nome della VM da eliminare

4. Tutti i file di configurazione delle macchine vengono generati automaticamente dai playbook