### Selezionare tutti gli uffici, ordinati per nazione
```` SQL
SELECT country FROM newschema.offices
GROUP BY country
````

### Selezionare tutti gli uffici, ordinati per nazione e per città
```` SQL
SELECT country,city FROM newschema.offices
GROUP BY country,city
````

### Selezionare tutti gli impiegati, ordinati per titolo e per nome
```` SQL
SELECT title, lastname, name FROM newschema.employees
GROUP BY title, lastname, name
````

### Contare quanti impiegati condividono lo stesso ufficio
```` SQL
SELECT office_id, COUNT(*) AS numero_uffici FROM newschema.employees
GROUP BY office_id
````

### Contare quanti impiegati condividono la stessa estensione
```` SQL
SELECT extension, COUNT(*) AS numero_estensione FROM newschema.employees
GROUP BY extension
````

### Selezionare tutti i prodotti con quantità inferiore a 500 pezzi
```` SQL
SELECT name, qty FROM newschema.products
GROUP BY name, qty HAVING qty < 500
````

### Selezionare tutti i prodotti Ford
```` SQL
SELECT * FROM newschema.products
WHERE name LIKE '%Ford%'
````

### Contare quanti prodotti Ford hanno quantità inferiore a 500 pezzi
```` SQL

````

### Per ogni impiegato mostrare il suo diretto superiore (tip: usa un alias quando fai la join)
```` SQL

````

### Per ogni impiegato mostrare il numero di telefono completo (numero ufficio + estensione)
```` SQL

````

### Selezionare i 10 ordini più recenti
```` SQL

````

### Per ogni cliente mostrare il numero di ordini che ha fatto (tip: attenzione al tipo di JOIN e al campo usato per il COUNT)
```` SQL

````

### Per ogni cliente mostrare la quantità di prodotti acquistati in ogni ordine, mostrando anche il nome del prodotto (tip: attenzione al tipo di JOIN)
  ## Ordinare per quantità
  ## Ordinare per nome o ID cliente
```` SQL

````
### Per ogni cliente mostrare il totale speso sulla piattaforma, il costo sostenuto per ogni prodotto ed il guadagno netto per la piattaforma (tip: la colonna MSRP indica il prezzo a cui è stato venduto il singolo prodotto)