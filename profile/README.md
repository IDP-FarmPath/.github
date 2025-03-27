## Proiect IDP – FarmPath

### 1.	Descrierea aplicației
**FarmPath** este o platformă online destinată închirierii utilajelor agricole, funcționând ca un marketplace unde fermierii și proprietarii de utilaje pot interacționa eficient. Aplicația utilizează o arhitectură bazată pe microservicii pentru a asigura scalabilitate, securitate și gestionare eficientă a componentelor.

### 2.	Arhitectura aplicației

#### Microservicii:
•	**FarmPath-Auth-Service**

Responsabil pentru autentificare și autorizare, utilizând protocoale precum OAuth și JWT.


•	**FarmPath-Business-Logic-Service**

Gestionază funcționalitățile principale ale marketplace-ului, cum ar fi închirierea de utilaje, procesarea plăților, gestionarea notificărilor și alte procese esențiale.


•	**Microserviciu pentru Baza de Date**

Se ocupă cu stocarea informațiilor despre utilizatori, utilaje și tranzacții. Este posibil ca acesta să fie deja implementat sau să necesite adăugarea sa în arhitectura curentă.


#### Componente Suport:
•	**Bază de Date**

Cel puțin un sistem de baze de date este necesar pentru stocarea informațiilor aplicației.


•	**Utilitar pentru Baze de Date**

Se poate utiliza un tool precum Adminer, PgAdmin sau orice alt instrument de gestionare a bazelor de date.


•	**FarmPath-Kong (API Gateway)**

Asigură expunerea securizată a rutelor publice, oferind un control centralizat asupra interacțiunilor externe ale aplicației.


•	**FarmPath-Portainer (UI pentru gestionarea containerelor și clusterului)**

Oferă o interfață ușor de utilizat pentru gestionarea și monitorizarea containerelor și a clusterului de aplicații.


•	**FarmPath-Grafana (Monitorizare și Observabilitate)**

Permite monitorizarea performanței și a sănătății aplicației, integrând posibil și Prometheus pentru metrici și Loki pentru loguri.


•	**CI/CD (GitLab CI/CD sau alt tool similar)**
Automatizează procesul de deployment și livrare continuă, facilitând actualizările rapide și sigure ale aplicației.


### 3.	Diagrama arhitecturii
![farmpath drawio](https://github.com/user-attachments/assets/40b229c7-3ba4-4391-ba9b-6632a683410a)
