# 🐍 Remote Access Tool (RAT) en Python

Ce projet est un **Remote Access Tool (RAT)** développé en Python. Il permet d’établir une connexion distante entre un client et un serveur, offrant des fonctionnalités avancées comme l’exécution de commandes à distance, le transfert de fichiers, ou encore la prise de captures d’écran. 
 
**by Mariam Cisse et Mike Arthur NYOGA - 4SI4 ESGI**

## 🚀 Fonctionnalités principales

- **Connexion distante** : Établissement d’une liaison sécurisée entre le client et le serveur.
- **Exécution de commandes** : Possibilité d’exécuter des commandes shell sur la machine cliente.
- **Transfert de fichiers** : Upload et download entre le serveur et la machine cliente.
- **Prise de captures d'écran** : Capture et transmission d'images de l'écran du client.
- **Récupération des hachages** :
  - Extraction des mots de passe Windows (SAM dump).
  - Extraction des mots de passe Linux (hashdump du fichier shadow).
- **Recherche et navigation** : Recherche de fichiers spécifiques sur la machine cliente.

---

## 🛠️ Installation

### Pré-requis

- **Python 3.x** : Doit être installé sur les machines serveur et cliente.
- **Bibliothèques Python nécessaires** :
  - Par exemple : `socket`, `subprocess`, `os`, `platform`, `pyautogui`, `Pillow`.

---

### 📦 Installation des dépendances

		
## **Utilisation**

### **Serveur**:
			
1. Exécutez le script server.py sur la machine server en utilisant Python 3.
2. Attendez que le serveur soit en écoute sur l'adresse IP et le port spécifié.
3. Une fois qu'une connexion est établie avec un client, vous pouvez utiliser les commandes disponibles pour interagir avec la machine cliente.

### **Client** :

1. Exécutez le script client.py sur la machine cliente en utilisant Python 3.  
2. Assurez-vous que le client peut se connecter au server en utilisant l'adresse IP et le port spécifiés.  
3. Une fois connecté, vous pouvez recevoir des commandes du server et exécuter des actions sur la machine cliente en fonction de ces commandes.  

	
## **Commandes Disponibles**: 

- **upload**: Permet de téléverser un fichier du serveur vers la machine cliente.  
- **download** <chemin/du/fichier> <nom_du_fichier>: Permet de télécharger un fichier de la machine cliente vers le serveur.  
- **screenshot**: Prend une capture d'écran de la machine cliente et l'envoie au serveur.  
- **shell**: Ouvre un shell interactif sur la machine cliente.  
- **ipconfig/ifconfig**: Obtient la configuration réseau de la machine cliente.  
- **find/search**: Recherche un fichier sur la machine cliente.  
- **hashdump**: Récupère le fichier shadow (sur Linux) de la machine cliente et le stocke sur le serveur.  
- **samdump** :  Récupère la base SAM (sur Windows) 
