# JavaRMI_Calculator


![image](https://user-images.githubusercontent.com/83409958/152502588-d7ae3efc-c940-43fa-86ea-d55dff9b5d0b.png)


Calculator est le contrat qui est donc une interface java contenant les methodes qui devront être exportées.

1- rmiregistry qui demarre le service de naming sur le localhost sur le port 1099 (qui est le port par defaut)

2- on demarre le server qui fait un rebind pour changer le nom rmiregistry associé a l'objet CalculatorImpl instancié

3- le client fait alors un lookup de ce nom pour obtenir dynamiquement le stub et ensuite il invoque les methodes add, mul, div, sub. L'implementation de ces methodes est faite du coté du serveur.

