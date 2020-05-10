# Auteur :  ABOUBAKAR AHAMADA								 
# Date : 08/05/2020											 
# Lieu : Casablanca											 

# Projet :
Une application web de gestion des comptes bancaires en Java/ JEE et Spring.	

# D�mo 
- Pour voir une d�mo de l'application en image, visitez la page wiki :
 https://github.com/AboubakarAhamada/Gestion-des-comptes-bancaires/wiki 
						 
# Sp�cificit�s fonctionnelles :
- Chaque compte appaertient � un client.
- Un compte bancaire peut �tre un compte courant ou un compte epargne.
- L'application doit permettre de :
	0. Cr�e un compte
	1. Consulter le compte d'un client
	2. Effectuer un versement
	3. Effectuer un retrait et dans ce cas le motant � retirer ne doit pas depasser le solde du compte. 
	4. Effectuer un virement d'un compte vers un autre compte. Il faut encore verifier le montant pour le virement
	5. Consulter les op�rations d'un compte 

# Specificit� techniques : 
- Pour la consultation des op�ration, les op�rations doivent
 s'afficher dans des pages. On doit utiliser la pagination, c'est � dire qu'on ne veut pas afficher
 toutes les op�rationd sur la meme page. 
- L'application doit �tre s�curis�e. Seuls les personnes identifi�es qui sont autoris�es � 
effectuer les op�rations ci-dessus mentionn�es.
- L'application doit g�rer les erreurs li�es � l'utilisateur
- L'application doit �tre responsive pour diff�rentes terminaux

# Architeure de l'application 
- L'application est bas�e sur une architecutre en couche � savoir :
 1. Une couche DAO pour l'acc�s aux donn�es. Ici on cr�e les interfaces ClientRepository,
 CompteRepository et OperationRepository qui heritent de l'interface JpaRepository.
 2. Une couche Entities o� on cr�e nos entit�s (classes) que seront mapp�es avec les tables dans la base de donn�es
 3.Une couche metier o� on cr�e une interface IbanqueMetier qui d�finit les op�rations ci-dessous mentionn�es et 
 une classe IbanqueMetierImpl qui implemente cette classe
 4. Une couche web (pr�sentation) o� on g�re tout ce qui est web (View)
 
 # Exigence techniques :
 - Utilisation de de Java et Spring Boot (Spring Data JPA, Spring Web, etc)
 - SGBD: MySQL
 - View (UI) : Thymeleaf, Bootstrap3
 
 # Outis de d�veloppement: 
 - IDE : Eclipse 
 - Gestion des d�pendences : Maven
 - Autre : Spring-boot-devtools





