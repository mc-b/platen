Platform Engineering mit Backstage.io: Einführung und Anwendung
===============================================================

Umgebung zum Kurs: [Platform Engineering mit Backstage.io: Einführung und Anwendung](https://www.digicomp.ch/d/platen).

Dashboard bzw. neu Headlamp
---------------------------

Das Kubernetes Dashboard/Headlamp ist wie folgt erreichbar:

    https://${fqdn}:30443
    http://${fqdn}:30444
    
Zugriffstoken für Headlamp erstellen:

    kubectl create token Headlamp-admin -n kube-system   

Beispiele
---------

Die Umgebung beinhaltet eine Vielzahl von Beispielen als Juypter Notebooks. Die Jupyter Lab Oberfläche ist wie folgt erreichbar:

    http://${fqdn}:18888/lab/tree/platen    - Jupyter Lab Oberfläche
    http://${control}:9999                  - GitLab (User: root, Password: sudo cat /etc/gitlab/initial_root_password  | grep Password:)
    