frontend  -  веб-приложение с  NodePort
backend   -  PostgreSQL с Volume (emptyDir)
config data - ConfigMap

Проверить работу: 
 1. пробросить порт - kubectl port-forward pods/app-deployment-68b89dcbc-sbc8z 8080:8080  // app-deployment-68b89dcbc-sbc8z -  это меняется
    , либо kubectl port-forward  -n homeworking service/app-service  8090:8090
 2. вызвать на лосальном хосте в браузере: http:\\localhost:8090
    