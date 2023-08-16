Nombre de la asignación: Docker+Kubernetes - Módulo 3 - Grupo 2 - Reto Integrador
Participantes

Nombre Esau Carreo, Citlali Matz, Carlos Gaytan, Efrain Melgarejo, Yesenia Castellanos
Actividades

Actividad:liveness probe
Comandos

kubectl get svc rng


kubectl get events -w
httping <ClusterIP>

kubectl get pods -w
$ ab -c 10 -n 1000 http://10.97.150.117/1

Comandos: 
Recursos externos

Recurso externo: 
Artifactos

Anexar artifactos al directorio de respuesta

$ ab -c 10 -n 1000 http://10.97.150.117/1

This is ApacheBench, Version 2.3 <$Revision: 1879490 $>
Copyright 1996 Adam Twiss, Zeus Technology Ltd, http://www.zeustech.net/
Licensed to The Apache Software Foundation, http://www.apache.org/

Benchmarking 10.97.150.117 (be patient)
Completed 100 requests
Completed 200 requests
Completed 300 requests
Completed 400 requests
Completed 500 requests
apr_socket_recv: Connection reset by peer (104)
Total of 552 requests completed

$ kubectl get pods -w
NAME                      READY   STATUS    RESTARTS      AGE
hasher-65db859b66-gjwjr   1/1     Running   0             46m
redis-6ff7cd7598-v7jrp    1/1     Running   0             46m
rng-5c9cd7744c-jj5hn      1/1     Running   1 (37s ago)   10m
webui-6969bf568c-lrll9    1/1     Running   0             46m
worker-6bbc87d469-f6cmg   1/1     Running   0             46m

