# abes-documentation-api-publish-config
Centralisation des fichiers de configuration du dépôt [abes-documentation-api-publish](https://github.com/abes-esr/abes-documentation-api-publish)

## Structure
### 1. lib/
#### 1.1. scenaripy_api-6.4.0.tar.gz
Une version de l'API scenaripy.

#### 1.2. SCENARIchain-server_6.3final_python.tar.gz
Le package python généré lors de la compilation du serveur scenari qui doit être branché sur l'API (le fichier est généré dans /tmp/scenarichain-server6.3/release/_python_/ lors de la compilation).
Cette partie est versionnée et doit correspondre à son environnement d'exploitation (develop|test|main). **main** correspond à l'environnement de production.

### 2. config/
#### 2.1. generator_types_codes.json
Liste les types de document utilisés et leur générateur scenari associé.

#### 2.2. items_to_purge.json
Liste les noms de fichiers et de dossiers à écraser lors du déploiement sur le serveur web de documentation.

#### 2.3. configuration_noms_chemins_manuels.json
Liste chaque manuel et son type ainsi que les chemins correspondant dans l'atelier scenari et le dossier où la documentation doit être déployée. Cette partie est versionnée et doit correspondre à son environnement d'exploitation (develop|test|main). **main** correspond à l'environnement de production.