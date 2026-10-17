# Beispiele zum Kurs: [Souveränes Platform Engineering mit Kubernetes](https://www.digicomp.ch/d/platen)

Nutze Kubernetes, Backstage und OpenChoreo für souveränes Platform Engineering. Lerne, wie integrierte Developer Platforms aufgebaut sind und erfahre, wie du durch offene Standards Kontrolle und Portabilität sicherstellst.

### Lernziele

* Einordnen der Entwicklung von DevOps zu Platform Engineering
* Beurteilen der Prinzipien einer souveränen Developer Platform
* Nutzen von Kubernetes als offene Basis für Platform Engineering
* Gestalten von Golden Paths und Self-Service für Entwicklungsteams
* Einsetzen von Backstage als zentralen Developer Hub
* Einordnen von OpenChoreo als integrierte Developer Platform
* Reduzieren von Vendor Lock-in und gezieltes Fördern der Portabilität

### Quick Start

Installiert [Git/Bash](https://git-scm.com/downloads), [Multipass](https://multipass.run/) und [Terraform](https://www.terraform.io/).

Git/Bash Kommandozeile (CLI) starten und dieses Repository clonen.

    git clone https://github.com/mc-b/platen
    cd platen
    
Terraform Initialisieren und VMs erstellen

    terraform init
    terraform apply
    
Terraform verwendet [Multipass](https://multipass.run/) um mehrere VMs zu erstellen.

Nach erfolgreicher Installation werden weitere Informationen für den Zugriff auf die VMs angezeigt.

### Deployment auf lernvirt Umgebungen
  
    cd lernvirt
    helm install platen . -n platen --create-namespace -f ${HELM_VALUES_HOST} -f ../platen/lernvirt-values.yaml 
    
Deinstallation
    
    helm uninstall platen -n platen && kubectl delete ns platen

### Beispiele und Übungen

* [Jupyter Notebooks](data/jupyter/)
* [Auto Shop GmbH – Übersicht](https://gitlab.com/ch-mc-b/autoshop-ms)

### Lizenz (Attribution-NonCommercial-ShareAlike 4.0 International)

![](http://www.creativecommons.ch/wp-content/uploads/2014/03/by-nc-sa1.png)

Quelle [Creative Commons](https://creativecommons.org/licenses/by-nc-sa/4.0/deed.de)

- - -

* Name muss genannt werden
* keine kommerzielle Nutzung erlaubt
* gleiche Lizenz vorgeschrieben

* Copyright (c) Marcel Bernet, Zürich
