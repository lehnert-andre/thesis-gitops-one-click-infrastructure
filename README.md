# Masterarbeit zum Einsatz von DevOps und GitOps Prinzipien in der privaten Cloud

- Arbeitstitel: ``` ```
- Student: ``` ```
- Matrikelnummer: ``` ```
- Datum der Erstellung: ``` ```
- Betreuender Professor: ``` ```
- Betrieb: 
  ```
  eXXcellent solutions
  consulting & software gmbh
  Industriestraße 48
  70565 Stuttgart
  ```
- Betreuer im Betrieb: ```Andre Lehnert```

---

## Kontext und Gegenstand der Arbeit

__„Was ist?“ etwa ½ Seite Text über den Startzustand: das Umfeld, den Stand der Wissenschaft und das Problem, das mit der Arbeit zu lösen sein soll.__

Die eXXcellent solutions consulting & software GmbH berät, konzipiert und entwickelt mit ihren Kunden individuelle datengetriebener Softwaresysteme. In der heutigen Zeit werden diese Systeme mehrheitlich in Cloud-Umgebungen betrieben. Je nach Kategorisierung der verarbeiteten Daten werden die Systeme in einer privaten oder öffentlichen Cloud-Umgebung bereitgestellt. Dem cloud-native Gedanken folgend, basieren die Systeme auf einer Microservice-Architektur, die entsprechend eines agilen Projektvorgehens von Scrum-Teams entwickelt wird.

Die Abschlussarbeit findet im Kontext eines Projekts mit unternehmenskritischen Daten statt. Das System wird in einer privaten und nativen Kubernetes-Umgebung betrieben. Ein Build- und Deployment-Pipeline (CI/CD) aus dem DevOps-Kontext entspricht nicht den Sicherheitsanforderungen des Projekts, da die Pipeline Zugangsdaten zur Cloud-Umgebung benötigt, um dort Software zu deployen. Diese Herausforderung soll mit der GitOps-Methodik begegenet werden, die ihrerseits Schwachstellen bei der Integration in den Entwicklungsprozess aufweist.

Die Arbeit widmet sich der GitOps-Methodik und dessen _Single Source of Truth_-Prinzips. In der Praxis führt diese Prinzip zu einer hohen Kopplung zwischen den Microservice-Teams und mindestens einem weiteren GitOps Repository, das den Infrastrukturcode enthält. Die GitOps-Methodik ist in dieser Hinsicht kritisch zu betrachten und entsprechend der Prinzipien guter Softwareentwicklung - hohe Kohäsion, lose Kopplung - zu bewerten.

## Ziele

__„Was soll?“ etwa ½ Seite abstrakt: Welche Forschungsfragen sollen beantwortet werden? Was soll erreicht werden? Welche wissenschaftlichen Erkenntnisse sollen gewonnen werden?__

Das Ziel der Arbeit besteht in der Beschreibung und Einordnung von GitOps in die Themen _DevOps_ und _DevSecOps_ im Kontext einer cloud-native Microservice-Landschaft. Die GitOps-Prinzipen und Lösungsmuster werden vorgestellt und kritisch beurteilt. Insbesondere die Prinzipen aus der _Microservice-Entwicklung_, wie die Unabhängigkeit der einzelnen Teams, werden hier berücksichtigt.

Im Verlauf der Arbeit soll die GitOps-Methodik zu einem hybriden Model weiterentwickelt werden, das die Akzeptanz in der Praxis fördert.
Die Ausarbeitung eines Kompromisses und die Skizzierung eines Lösungswegs über eine Referenzimplementierung steht hier im Mittelpunkt.

## Artefakte

__„Was soll?“ konkret: Stichpunktartig formuliert, welche konkreten Dinge produziert werden sollen. Dazu gehört stets das Thesisdokument, ggf. Programme wie Spezifikationen, Implementationen, Prototypen, Handbücher, oder Videos, Filme.__

- Spezifikation einer cloud-native Referenzarchitektur zum Betrieb von Microservice-Systemen
  Wünschenswert sind typische Infrastruktur-Bestandteile:
  - Betrieb eines gestellten Microservice-Systems
  - GitOps Operator zur Realisierung des Continuous Delivery nach dem Pull-Prinzip
  - Secret Management
- Erstellung eines open-source GitOps Repositories mit einer Referenzimplementierung
  - Ensprechend der GitOps-Methodik besteht die Referenzimplementierung vornehmlich aus .yaml-Dateien zur Konfiguration der Kubernetes-Infrastruktur
- Weitere optionale Repositories zur Simulation der Microservices-Repositories



## Aufgaben

__„Wie soll?“: Stichpunktartig einzelne Aufgabenpakete, die vom Start bis zu den Zielen zu bearbeiten sind. Ggf. Vorgehensweisen, Methoden, Lösungsansätze nennen. Ggf. Umfang abschätzen, Reihenfolgen festlegen, Prioritäten setzen.__

Vorbereitung:

- Bereitstellung eines Beispiel Microservice-Systems durch den Betrieb
- Definition von Mindestanforderungen durch das Projekt.
  Die Anforderungen ergeben sich über diese Schwerpunkte:
  - Betrieb
  - Sicherheitsaspekte
  - Inegration in den Entwicklungsprozess
  - Wartbarkeit
  - Übertragbarkeit

Durchführung:

- Vorstellung des Themas, der Motivation und des Projekts
- Herstelllung der theoretischen Wissensbasis
  - Microservices
  - Cloud-Technologien
  - Agile Software-Entwicklung
  - DevOps inkl. Automatisierungslösungen, wie CI/CD
  - DevSecOps
  - GitOps
- Ausarbeitung und Vorstellung von mindestens zwei Lösungswegen
- Validierung der ausgearbeiteten Lösungswege bzw. Referenzarchitekturen gegenüber den Mindestanforderungen (erfüllt/ nicht erfüllt)
- Ausarbeitung einer Referenzimplementierung für einen Lösungsweg
- Gegenüberstellung der Referenzimplementierung und des resultierenden Entwicklungsprozesses mit dem bisherigen Vorgehen
- Fazit

Die Referenzimplementierung und die Verprobung kann lokal oder auf einer bereitgestellten Kubernetes-Umgebung erfolgen.



## Literatur

__Bücher, Artikel, elektronische Quellen zum Thema__

- Domain-Driven Design Distilled; Vernon, Vaughn; Addison-Wesley; ISBN 978-0-13-443442-1
  deutsche Übersetzung: ISBN 978-3-86490-439-4
- https://ddd-referenz.de/
- Clean Architecture; Martin, Robert C.; Pearson; ISBN 978-0-13-449416-6
  Hier die Themen: "Component Cohesion" und "Component Coupling"
- https://www.gitops.tech/
  Das Buch zumr Thema: ISBN 978-3982112688
- GitOps and Kubernetes: Continuous Deployment with Argo CD, Jenkins X, and Flux; Yuen, Billy; et al.; ISBN 978-1617297274
- ...

