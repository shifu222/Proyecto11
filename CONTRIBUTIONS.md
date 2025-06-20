# Contribuciones de Gabriel Castillejo

Estos commits son del repositorio de [Repositorio - Proyecto11-gitflow](https://github.com/Software-Dev-CC3S2-Team-11/url-shortener-git-flow) pero practicamente son los mismos avances en el otro repositorio por lo que solo listo los commits de este repositorio y no del  [Repositorio-Proyecto11-trunk-project](https://github.com/Software-Dev-CC3S2-Team-11/url-shortener-trunk-based)

## Sprint 1

- 2025-06-08 : Cree un archivo para el template de los issues
  Commit: `chore: update issue templates`
- 2025-06-08 : Modifiqué el script `run_app.sh`
para que detecte la existencia del archivo `config.json`
 Commit: `feat: add configuration file and update script to verify if file exists`  
 Pull request: #8

- 2025-06-08 : Agregué las dependencias a usar en el archivo `requirements.txt`
Commit: `chore: add new dependencies in requirements.txt`
Pull request: #10

- 2025-06-08 : Agregué un endpoint GET /slug a `app.py` que redirecciona de acuerdo al parametro slug
  Commit: `feat: add GET /{slug} endpoint to redirect using url_mapping as database`  
 Pull Request: #10

- 2025-06-09 : Modifiqué `config.json` para agregar las variables del servidor `HOST` y `PORT`
Commit: `feat: update configuration file to configure port and host`
Pull Request: #11

- 2025-06-09 : Agregue el archivo de index.html y result.html
  Commit: `feat: add Jinja2 templates for form and shorter`
Pull Request: #11

- 2025-06-09 (00:31): Modifique app.py para que lea las configuraciones desde un config.json y acepte jinja
 Commit: `feat: load host and port from config file and set Jinja2 as template engine`
Pull Request: #11

- 2025-06-09 (00:42): Agregué un endpoint POST /shorter en app.py que renderiza un html con la url acortada
Commit: `feat: add POST /shorter endpoint to generate short url and render response`
Pull Request: #11

- 2025-06-09 (00:44): Agregué un endpoint GET / en app.py que renderiza el formulario inicial
Commit: `feat: add GET / endpoint to render home page`
Pull Request: #10

- 2025-06-09 (06:21): Realizo un PR para hacer merge a develop
Commit: `Merge feature/get_slug_endpoint into develop`  
Pull Request: #10

- 2025-06-09 (06:22): Realizo un PR para hacer merge a develop
Commit: `Merge feature/post_shorter_endpoint into develop`
Pull Request: #11

## Sprint 2

- 2025-06-17 : Reestructure el proyecto en /models /routes /services /templates /database
Commmit: `chore: restructure project layout`  
Pull Request: #22  

- 2025-06-17 (21:12): Merge a develop
Commit : `Merge feature/project-structure into develop`  
Pull request: #22

- 2025-06-18 (16:16): Formatea el código para que sigla las reglas de PEP 8
Commit : `chore: format code to follow PEP 8`  
Pull request: #29

- 2025-06-18 (16:17): Creo un archivo core/setting.py que lee el archivo de configuracion y variables de entorno
Commit: `chore: update configuration files`  
Pull request: #29

- 2025-06-18 (16:20): Mueve los endpoinst de app.py a routes/url.py
Commit: `refactor: move URL endpoints to routes/urls.py`  
Pull Request: #29

- 2025-06-18 (16:22): Crea un token cuando el usuario se registra
  Commit: `feat: generate token on user registration`  
  Pull Request: #29

- 2025-06-18 (16:24): Modifique el navbar.html para que solo aparezca ciertos botones cuando el usuario está o no logeado
  Commit: `feat: toggle login/register buttons based on user session`  
  Pull Request: #29

- 2025-06-18 (16:28): Agregue funciones en `services/shorter_url.py` que hashea la url y genera la metadata asociada a la url
Commit: `feat: add functions to generate slug and build URL object from original URL and username`
  Pull Request:#29

- 2025-06-18 (16:29): Agregue funciones que interactuan con la base de datos considerando las reglas del negocio
Commit: `feat: implement DB methods to store and retrieve URLs`  
  Pull request: #29

- 2025-06-18 (21:37): Resuelven algunos conflictos antes del merge a develop
Commit: `Merge branch 'develop' into feature/shorter_url_service`  
  Pull request: #29

- 2025-06-18 (21:53): Realiza el merge a develop
Commit: `feat: implement business logic for URL creation and database interaction`  
  Pull Request: #29

- 2025-06-19 (16:26): Agrego los archivos inits para que puedan ser importados como módulos
Commit: `chore: add pytest config and init files for module discovery`  
  Pull Request: #34

- 2025-06-19 (16:30): Actualizo los paths para no tener problemas de importación en pytest
Commit: `refactor: update import paths and format files`  
  Pull Request: #34

- 2025-06-19 (16:34): Agrego los test que verifican el funcionamiento de las funciones del servicio de shorter_url
Commit: `test: add tests to validate shorter_url functions`  
  Pull Request: #34

- 2025-06-19 (16:36): Agrego el script ci.sh que verifica que se cumplen las condiciones de flake 8 y verifica la covertura de las pruebas
Commit: `ci: add CI pipeline with flake8 and coverage validation via ci.sh`  
  Pull Request: #34

- 2025-06-19 (17:12): Modifico el ci.yml para que instale las dependencias(requirements.txt)
Commit: `ci: update CI workflow to include requirements installation`  
  Pull Request: #34

- 2025-06-19 (18:27): Formateo el código para que pase la prueba del flake 8
Commit: `style: format code for flake8`  
  Pull Request: #34

- 2025-06-19 (18:28): Agrego las variables de entorno al ci.yml que van a ser leidas desde el action
Commit: `ci: add secrets variables to ci workflow`  
  Pull Request: #34

- 2025-06-19 (22:02): Resuelven algunos conflictos
Commit: `Merge branch 'develop' into test-shorter-url`  
  Pull Request: #34

- 2025-06-19 (23:37): Realiza el merge a develop
Commit: `Merge branch test-shorter-url into develop`  
  Pull Request: #34

- 2025-06-19 (23:40): Realiza el merge a develop
Commit: `Merge branch 'develop' into feature/dash-connection`  
  Pull Request: #32

- 2025-06-19 (23:54): Realiza el merge a develop
Commit: `Merge branch 'develop' into feature/frontend/design-update`  
  Pull Request: #35
