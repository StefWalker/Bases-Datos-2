## 1. Explique el concepto de shard, replica y partition.
- Shard 
    Se da al dividir una tabla en subtablas para querys especificos o busquedas simplificadas.
    Cada subtabla contiene informacion distinta a las consecuentes subtablas.
- Replica
    La replicacion se da al realizar una copia y distrubucion de datos y objetos de base de datos, de una base a otra, para la sincronizacion de datos y permanencia de los mismos en distintas bases.
- Partition
    La particion se da al separar una tabla grande en tablas mas pequeñas, disminuyendo el tiempo de las consultas a solo una fraccion del tiempo y simplificando el scaneo de datos.
    Este se diferencia de los Shard debido a que los shards son solo para realizar querys y las particiones si afectas la forma de las tablas.

## 2. Explique la diferencia entre Strong Consistency Eventual Consistency.
- Strong Consistency 
    Esta dice que los datos deben ser altamente consistentes todo el tiempo, todos los servidores interconectados se requieren que tengan los datos actualizados en todo momento, la forma optima de aplicar este caso es con el bloqueo de nodos en el momento de realizar un update.
- Eventual Consistency
    Permite que los datos esten altamente disponibles, tambien se conoce como replicacion optimistica, esto se logra manteniendo una red de servidores que se apoyan entre si cuando uno de estos presenta una falla.

## 3. ¿En que consiste warm replicas y hot replicas?
- Warm
    Este se da cuando se quiere trabajar con una imagen casi identica a la de los datos dados en produccion, este se da combinando con alta disponibilidad, este ayuda a una transicion casi perfecta de la solucion dada.
- Hot
    Este ayuda a dar soluciones comerciales no criticas, estan implican poca latencia y dan el para lograr un trabajo adecuado para las operaciones comerciales.

## 4. ¿En que consiste consiste switch over y fail over?
- Switch over
    Un Switchover es la operación de intercambio de roles entre la base de datos primaria y la base de datos segundaria. Se garantiza que no hay perdida de datos y se realiza normalmente para tareas de mantenimiento.
- Fail over
    El Failover es la transación de una Data base segundaria a una primaria. Cuando hay un fallo en la base primaria o no se puede acceder por alguna razón.
