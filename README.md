# Descripción
Proyecto que permite visualizar los cambios ocurridos en un microservicio
ya sea que no esta disponible por un cambio publicado desde git con GitAction.

# Arquitectura
Arquitectura Hexagonal

# Flujo CI/CD

kubectl get all
Muestra todos los recursos en el namespace actual (pods, servicios, despliegues, etc.).

kubectl describe  
Muestra información detallada y eventos relacionados con un recurso específico, útil para detectar errores o estados anómalos.

kubectl logs 
Muestra los logs de un pod, fundamental para entender qué está ocurriendo dentro del contenedor.

kubectl exec -it  -- /bin/bash
Accede de manera interactiva a un pod (si tiene bash/sh), permitiéndote investigar en el entorno del contenedor.

kubectl top pod
Muestra el uso de CPU y memoria de los pods en ejecución, útil para detectar cuellos de botella.

kubectl get events
Lista eventos del clúster, como errores o avisos relacionados con recursos.

