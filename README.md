Mon process

1. VM Ubuntu Server + Docker  
sudo apt install docker.io docker-compose -y

sudo usermod -aG docker $USER

2. Création du docker-compose.yaml + création du nginx.conf

   3 Conteneurs :
- MariaDB  
- WordPress 
- Nginx

3. Volume commun
wp_data est partagé : nginx / wordpress

4. Déploiement
docker-compose up -d


5. Vérifications
- docker ps : 3 conteneurs fonctionnels  
- Test IP sur navigateur de la machine hôte : WordPress installé  
- docker volume ls : persistance wp_data / db_data

Les fichiers de conf sont consultables ainsi que les captures d'écrans en piéce jointe.
