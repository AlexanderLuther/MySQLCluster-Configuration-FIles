# MySQLCluster-Configuration-FIles
Archivos de configuración para los nodos que forman parte de un cluster de base de datos utilizando MySQL Cluster.

El cluster esta conformado por dos nodos activos, un nodo pasivo y un nodo de administracion. Los nodos activos y el pasivo tambien son nodos para consultas SQL. Las rutas donde se ubica cada archivo de configuracion son:

+Nodo de Administracion
-/var/lib/mysql-cluster/config.ini
-/etc/systemd/system/ndb_mgmd.service

+Nodo Activo1-SQL y Nodo Activo2-SQL
-/etc/my.cnf
-/etc/systemd/system/ndbd.service

+Nodo Pasivo
-/etc/my.cnf
-/etc/systemd/system/ndbd.service
