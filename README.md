
# Scraping and analysis of gastronomic data  

## Explanatory note
This project makes use of these distinctions to clarify the theology of the approach:
   - Course: a set of recipes relating to the same type, e.g. first courses, side dishes, desserts...
   - Recipe: main analysis object of which we want to obtain information from the site
   - Ingredients: set of foods needed to make the recipe


# Get a json file with all the details of a course
        
Terminal command example: python [Path]/RecipeScraper/scrapingPortata.py antipasti 1
    
This program takes as input the desired portata and the dormancy time (in seconds) to wait between the analysis of one recipe and the next.

In this regard, the portata.conf file is used in which it is possible, for the non-programmer user, to view links to the various courses, as well as the courses available for analysis.

A json file renamed with the name of the analyzed portata is produced in output, in the "cartella_portate" folder.

If "cartella_portate" does not exist, it is auto-generated by the program.

The output JSON file contains the relative recipes, with data managed in this way:

    "title": name of the recipe
    "description" : accurate description of the recipe
    "instructions": set of steps to be carried out to create the complete dish
    "ingredients" : Array of ingredients with the following fields
        "name" (str)
        "amount" (str)
    "details" : string containing a set of useful information
    "acquisition time": timestamp in which the information was retrieved
    "link": URL of the web page containing the recipe information


## Note esplicative
Questo progetto fa uso di queste distinzioni per rendere più chiara la tetodologia di approccio :  
   - Portata : Un insieme di ricette attinenti alla stessa tipologia, es. primi piatti, contorni, dolci ...
   - Ricetta : Oggetto di analisi principale della quale vogliamo ottenere le informazioni dal sito
   - Ingredienti : insieme di alimenti necessari per la realizzazione della ricetta 


# Ottenere un file json con tutti i dettagli di una portata
        
Esempio comando da terminale : python [Percorso]/RecipeScraper/scrapingPortata.py antipasti 1
    
Viene eseguito il programma scrapingPortata.py che prende in ingresso la portata desiderata ed il tempo (in secondi) di dormienza che si desidera attendere tra l'analisi di una ricetta e la sucessiva. 

A tal proposito viene usato il file portata.conf in cui è possibile, per l'utente non programmatore, andare a visionare 
i link alle varie portate, come anche le portate disponibili all'analisi. 

Viene prodotto in output, nella cartella "cartella_portate" un file json rinominato con il nome della portata analizzata. 

Se "cartella_portate" non esistesse, viene auto generata dal programma. 

Il file JSON in output, contiene le relative ricette, con dati gestiti in questo modo :

    "title" : nome della ricetta
    "description" : desccrizione accurata della ricetta
    "instructions" : insieme di passi da svolgere per creare il piatto ompleto
    "ingredients" : array di ingredienti con i seguenti campi 
        "name" (str) 
        "amount" (str) 
    "details" : stringa contenente un insieme di informazioni utili
    "acquisition time": timestamp in cui le informazioni sono state reperite
    "link": URL della pagina web in cui sono presenti le informazioni delle ricetta
    

# Installation

Le libreie python, richieste per l'eseuzione del codice, sono presenti all'interno del file "requirement.txt" 


# Authors and acknowledgment

- code author : https://github.com/EdordoPng
