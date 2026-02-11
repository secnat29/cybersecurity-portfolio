# Progetto: Configurazione VLAN e ACL su Packet Tracer

## Descrizione
In questo laboratorio ho implementato una rete locale suddivisa in diverse **VLAN** per migliorare la sicurezza e l'efficienza del traffico. Ho inoltre configurato delle **ACL (Access Control Lists)** per filtrare il traffico tra i vari dipartimenti.

## Obiettivi Tecnici
* **Segmentazione della rete:** Creazione di VLAN per separare i reparti (es. Admin, Ospiti, Vendite).
* **Inter-VLAN Routing:** Configurazione del router per permettere la comunicazione controllata tra le sottoreti.
* **Sicurezza con ACL:** Implementazione di regole per bloccare accessi non autorizzati a server sensibili.

## Cosa contiene questa cartella
* `vlan-router-on-a-stick.pkt`: Il file sorgente di Packet Tracer.
* `router.txt` / `switch.txt`: Gli script di configurazione CLI estratti.
* `topology.png`: Lo schema visivo della rete.

## Comandi principali utilizzati
```bash
# Esempio di creazione VLAN
vlan 10
name Amministrazione

# Esempio di ACL applicata
access-list 101 permit tcp any host 192.168.1.10 eq 80
