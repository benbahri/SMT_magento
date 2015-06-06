# SMT_magento
SMT_magento est un module Magento de paiement en ligne pour SPS Monétique Tunis

	Installation

1- Téléchargez le .zip du module depuis Github et décompressez le

2- Insérez le dans votre projet

3- Vérifiez qu'il est est bien visible depuis le back office et qu'il est activé : admin -> Système -> Configuration -> Ventes -> Mode de paiement -> My Gateway

4- Dans le fichier app/design/frontend/base/default/template/mygateway/redirect.phtml:
	-Modifiez l'URL d'envoi des données du formulaire (http://196.203.11.74/paiement/ pour la phase du test exigés par Monétique Tunisie et https://www.smt-sps.com.tn/clicktopay/ après validation des tests et passage à la version production).
	-Intégrez le numéro d'affiliation chez la société Monétique Tunisie dans la value du champs affilie.
	
5- Dans le fichier notification.php faites attention aux noms des tables de la votre base de données
