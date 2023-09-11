# Active-Directory-Group-Policy-Object-GPO-

### Configuration d'une GPO via le Gestionnaire de serveur

1. **Ouvrir le Gestionnaire de serveur**

ON clique sur "Outils" dans le coin supérieur droit, puis ON sélectionne "Gestion des stratégies de groupe".

2. **Créer une nouvelle GPO**

   - Dans la fenêtre de l'éditeur de GPO, sous "Forêt", faites un clic droit, puis sélectionnez "Créer un objet GPO dans ce domaine, et la lier ici...".

   - Donnez un nom à votre GPO, Comme dans cette exemple, "Bloquer le panneau de configuration".
  
  ![image](https://github.com/manmaryem/Active-Directory-Group-Policy-Object-GPO-/assets/137881827/a525cc89-4dfb-4d46-8f48-d3df6c88fa40)

   - Cliquez sur "OK" pour créer la GPO.

3. **Modifier la GPO pour configurer les restrictions**
   
   - Dans la fenêtre de l'éditeur de GPO, faites un clic droit sur la GPO que vous venez de créer ("Bloquer le panneau de configuration") et sélectionnez "Modifier".

4. **Configurer les paramètres de restriction**

   - Dans la fenêtre de l'éditeur de GPO, naviguez dans la section "Configuration de l'ordinateur" pour les paramètres de l'ordinateur ou "Configuration de l'utilisateur" pour les paramètres de l'utilisateur.

     ![image](https://github.com/manmaryem/Active-Directory-Group-Policy-Object-GPO-/assets/137881827/74546f31-538b-43e0-8c03-8ae6512d03c3)


   - Par exemple, pour restreindre l'accès au Panneau de configuration, vous pouvez naviguer jusqu'à "Configuration de l'utilisateur -> Modèles d'administration -> Panneau de configuration" et configurer les paramètres pertinents, par exemple, "Masquer l'icône Panneau de configuration" en double-cliquant dessus, puis en sélectionnant "Activé".
     
  ![image](https://github.com/manmaryem/Active-Directory-Group-Policy-Object-GPO-/assets/137881827/297ce9d9-e611-4d41-91d8-19fbd55fc590)

  ![image](https://github.com/manmaryem/Active-Directory-Group-Policy-Object-GPO-/assets/137881827/6a02f354-ca47-46dc-8a5f-2edff25c0069)


5. **Vérifier et tester la GPO**

   - Pour vérifier si la GPO s'applique correctement, vous pouvez attendre que la mise à jour des stratégies de groupe se fasse automatiquement ou forcer une mise à jour en exécutant la commande `gpupdate /force` sur les ordinateurs clients.

   - Connectez-vous à un ordinateur en tant qu'utilisateur pour lequel la GPO est censée s'appliquer et vérifiez que les restrictions sont en place et que l'icône du Panneau de configuration est masquée.
   - 
![image](https://github.com/manmaryem/Active-Directory-Group-Policy-Object-GPO-/assets/137881827/eadaf601-8a76-4d7d-a3de-823832a04f16)

