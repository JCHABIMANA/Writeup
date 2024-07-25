# AZURE AD
## DIFFERENCE ENTRE AZURE AD et AD DS
- AD DS: On premise AD
> - Authentification
> -  Kerberos
> -  NTLM
> -  RDAP
> -  Arborescence (arbres-OU)
				
- AZURE AD: On line access via web
> - API, Pas d'arbrorescence, Les requetes http, Des token, Authentification, SAML 2.0,
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
AZURE a commencé par immigration d'ex-change dans le cloud
L'AZURE AD n'est pas un AD, il est en cours d'évolution

## COMMENTAIRES
### AZURE AD
 Pay as you go services
 Single Sign-on
 MFA
 Public, hybride, prive

### AD
Prix d'achat du materiel
Prix d'exploitation (éléctricité, logiciels et maintenance)


## En audit AD et audit AZURE AD, quelle la difference?
local vs cloud

Objectif : 
L'audit dans les deux systèmes se concentre sur les activités de sécurité et de gestion des identités, mais utilise des outils et des méthodes différents en fonction de l'environnement 

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
