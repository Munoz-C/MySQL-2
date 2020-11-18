# MySQL-2
Utilisation de SQL dans PHPMyAdmin avec la base de donné " sakila "

Premier exercice en utilisant phpMyAdmin:

Pour écrire la demande qui permet d'afficher les noms de famille et l'adresse email de tous des consommateurs de " sakila ".

 SELECT last_name, email FROM customer 

   " SELECT (le ou les column Name, column Name) FROM "de" (la table que l'on cherche) ".

Deuxieme exercice en utilisant phpMyAdmin:
Pour écrire la demande qui permet d'afficher toutes les transactions du 23/08/2005.

 SELECT * FROM paiement                        
 WHERE DATE (date_paiement) = '2005-08-23'     
   
  " SELECT (le ou les column Name, column Name) FROM "de" (la table que l'on cherche) ".
  " WHERE  ( " où "pour filtrer les enregistrements.) ((la column Name)) Opérateurs de comparaisons et ce qui est rechercher.

Troisieme exercice en utilisant phpMyAdmin: 
Pour selectionner seulement les quinze premiers paiements pour la date du 14/02/2006.

 SELECT * FROM paiement                          
 WHERE DATE (date_paiement) = '2006-02-14'      
 ORDER BY payment_date ASC                       
 LIMITE 15                                       

  " SELECT (le ou les column Name, column Name) FROM "de" (la table que l'on cherche) ".
  " WHERE  ( " où "pour filtrer les enregistrements.) ((la column Name)) Opérateurs de comparaisons et ce qui est rechercher.
  " ORDER BY ( permet de trier les lignes dans un résultat. ) la column puis DESC (inverser l’ordre) ou ASC (classés par ordre ascendant)
  " LIMT (pour spécifier le nombre maximum de résultats que l’ont souhaite obtenir.) puis le nombre .
