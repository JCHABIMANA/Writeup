# AZURE AD avec Vincent Le Toux, l’auteur de Ping Castle (un outil permettant d’auditer son AD)
## DIFFERENCE ENTRE AZURE AD et AD DS
- AD DS: On premise AD
> - Authentification
> - Kerberos
> - NTLM:protocole NT LAN Manager
> - RDAP:Registration Data Access Protocol
> -  Arborescence (arbres-OU)
				
- AZURE AD: On line access via web
> - API(Application Programming Interface), Pas d'arbrorescence, Les requetes http, Des token, Authentification, SAML 2.0,
> - OAuth 2.0, OpenID connect, WS-Federation, DFS,  Strategie de securité, il y les conditions d'accès pour gérer les mesures de sécurité (comment va s'authentifier les gens, d'ou ils viennent...)
						 								  
## AD et AZURE AD ont en commun 
> - Les utilisateurs
> -  Les groupes
> -  Authentification
> -  Autorisation
								  
## ATTENTION
Si on ajoute les postes Windows, ça n'ont pas les meme fonctionalité que AD
S'appelle AZURE AD mais c'est different
Là aussi c'est confisant, tu peux héberger ton AD DS, s'appelle AD, pas AZURE AD

## Pourquoi choisir AZURE AD?
> - Une gestion des identités et des accès robuste-
> - Sécurité renforcée-MFA
> - Expérience utilisateur améliorée-SSO (Single Sign-on)
> - Modelinisation (Public, hybride, prive)
> - Pay as you go services....

### AD
> - Prix d'achat du materiel
> - Prix d'exploitation (éléctricité, logiciels et maintenance)


## En audit AD et audit AZURE AD, quelle la difference?
   Infrastructure local vs cloud
- Objectif
> - L'audit dans les deux systèmes se concentre sur les activités de sécurité et de gestion des identités, mais utilise des outils et des méthodes différents en fonction de l'environnement 

## LES OUTILS AD-DS et AZURE AD
- AD-DS
> - Active Directory Users and Computers (ADUC) :Ajout, suppression, modification et gestion des propriétés des objets dans le domaine.
> - Group Policy Management Console (GPMC):Gestion avancée des utilisateurs, des groupes, des unités d'organisation et des stratégies de mot de passe.
> - Active Directory Sites and Services:Gestion des sites, des sous-réseaux et de la topologie de réplication.
> - PowerShell:Gestion automatisée des objets AD, des GPOs, et des audits de sécurité à l'aide de modules comme ActiveDirectory et GroupPolicy.

- AZURE AD
> - Azure Portal:Interface web pour gérer les services Azure, y compris Azure AD.
> - Azure AD Admin Center: Portail spécifique pour la gestion d'Azure AD.
> - Azure AD Connect:Outil pour synchroniser les identités entre AD DS on-premises et Azure AD
> - Azure PowerShel:Automatisation des tâches de gestion d'Azure AD, telles que la création et la gestion des utilisateurs, des groupes, des rôles et des applications.
> - Azure CLI:Interface en ligne de commande pour gérer les services Azure
> - Microsoft Sentinel-SIEM

## POUR ALLER PLUS LOIN
https://www.microsoft.com/fr-fr/security/business/identity-access/microsoft-entra-id
