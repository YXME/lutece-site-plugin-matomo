![](https://dev.lutece.paris.fr/jenkins/buildStatus/icon?job=site-plugin-matomo-deploy)
# Plugin Matomo

![](https://dev.lutece.paris.fr/plugins/plugin-matomo/images/matomo-logo.jpg)

## Introduction

Ce plugin vous permet d'ajouter un tracker Matomo dans toutes les pages du site

Il offre �galement une interface de consultation du tableau de bord Matomo

## Configuration

D�finir dans les Propri�t�s du site :
 
* L'ID du site
* L'URL du serveur HTTP Matomo
* L'URL du serveur HTTPS Matomo
* The widget Authentication Token (optionnal)


Les valeurs initiales peuvent �tre configur�es dans le fichier **matomo.properties** comme suit :


```

# matomo properties file

matomo.default.site.id=15
matomo.default.server.http.url=http://www.example.com/matomo/
matomo.default.server.https.url=https://www.example.com/matomo/
matomo.default.widget.auth.token=6b34579abd8b74a12b87a809ef060185                    
                    
```


Ajouter le signet `matomo` dans un template du site, typiquement **page_frameset.html** 


```

<!-- matomo include -->
${matomo}                        
                    
```



[Maven documentation and reports](https://dev.lutece.paris.fr/plugins/plugin-matomo/)



 *generated by [xdoc2md](https://github.com/lutece-platform/tools-maven-xdoc2md-plugin) - do not edit directly.*