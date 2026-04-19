# Quest---Requete-dig -


### 1. Adresses IP version 4 de la wild code school :


Dig A [www.wildcodeschool.com](http://www.wildcodeschool.com/ "http://www.wildcodeschool.com")
    
![[Capture d'écran 2026-04-19 112629.png]](Quete-DNS-avec-dig-1.png)



www.wildcodeschool.com. 72 IN CNAME 2902314.group14.sites.hubspot.net.

2902314.group14.sites.hubspot.net. 72 IN CNAME group14.sites.hscoscdn10.net.

group14.sites.hscoscdn10.net. 72 IN A 199.60.103.31

group14.sites.hscoscdn10.net. 72 IN A 199.60.103.225



### 2. Adresses IPv6 du site odyssey :


Dig AAAA [odyssey](http://www.odyssey/ "http://www.odyssey").wildcodeschool.com


![[Capture d'écran 2026-04-19 113554 1.png]](Quete-DNS-avec-dig-2.png)



odyssey.wildcodeschool.com. 300 IN CNAME ghs.googlehosted.com.

ghs.googlehosted.com. 289 IN AAAA 2a00:1450:4007:80f::2013

L’hébergeur d’odyssey est Google.

### 3. Noms de serveur faisant autorité

Les noms des serveurs de noms faisant autorité sur le domaine wildcodeschool.com 

![[Capture d'écran 2026-04-19 115428.png]](Quete-DNS-avec-dig-3.png)


#### Les serveurs d’autorité sont :

- ns1.google.com
    
- Et dns-admin.google.com
    


#### Le serveur primaire est : googlehosted.com


![[Capture d'écran 2026-04-19 120759.png]](Quete-DNS-avec-dig-4.png)






4. 

(Bonus) Refaire les requêtes précédentes en précisant l'utilisation du serveur récursif **quad9** (9.9.9.9 ou 2620:fe::9)

#### IPv4 de la wildcodeschool

dig @9.9.9.9 A www.wildcodeschool.com

![[Pasted image 20260419123327.png]](Quete-DNS-avec-dig-5.png)


#### IPv6 de odyssey

![[Pasted image 20260419123442.png]](Quete-DNS-avec-dig-6.png)

Le chemin du serveur récursif quad9 est bien précisé dans la "Statistic section".



#### Reverse DNS 

dig -x 2a00:1450:4007:816::2013

![[Pasted image 20260419124626.png]](Quete-DNS-avec-dig-7.png)

ensuite 

![[Pasted image 20260419124602.png]](Quete-DNS-avec-dig-8.png)


En passant par le serveur récursif qad9 

![[Pasted image 20260419124803.png]](Quete-DNS-avec-dig-9.png)

le serveur d'autorité est : 
in
