# spring-cloud-bootstrapping

This project is a sandbox for a blog post on bootstrapping spring cloud config server with service discovery http://www.baeldung.com/spring-cloud-bootstrapping




- le post ne précise pas de test de vérification que tout est ok
- pas de message d'erreur visible sans logging.level.org.springframework.cloud.config=debug
- si git n'est pas dans le path du config serveur ça se bloque et le message d'erreur n'est pas visible sans logging.level.org.eclipse.jgit=debug
- le protocole git n'a pas besoin d'authentification, https utilise user/password

# Idées
## 3.5 : vérification
Une fois le config serveur démarré et la config de discovery disponible on vérifier que tout est ok avec
``` curl http://localhost:8081/discovery-default.properties```



# links

- doc spring cloud : https://cloud.spring.io/spring-cloud-config/spring-cloud-config.html
- spring-cloud-config-server : configurer git : https://docs.pivotal.io/spring-cloud-services/1-3/common/config-server/configuring-with-git.html


