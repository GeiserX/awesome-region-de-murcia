# AGENTS.md — awesome-region-de-murcia

## Propósito

Selección de software open source que da **soporte específico a la Región de Murcia** — su gobierno autonómico (CARM), ayuntamientos, universidades, empresas, infraestructuras y patrimonio. Todo el contenido en español. El foco es la Región de Murcia: el software debe dirigirse específicamente a esta comunidad autónoma o a sus municipios.

## Ámbito

- **45 municipios** de la Región de Murcia están dentro del ámbito.
- Principales ciudades: Murcia (capital), Cartagena, Lorca, Molina de Segura, Alcantarilla, Cieza, Águilas, Yecla, Jumilla, Totana, Mazarrón, Caravaca de la Cruz, San Javier, Torre-Pacheco, San Pedro del Pinatar, Las Torres de Cotillas, Archena, Cehegín, Santomera, Alhama de Murcia, La Unión, Fuente Álamo, Mula, Abanilla, Bullas, Calasparra, Puerto Lumbreras, Beniel, Librilla, Fortuna, Blanca, Abarán, Moratalla, Los Alcázares, Alguazas, Lorquí, Ceutí, Campos del Río, Pliego, Ulea, Villanueva del Río Segura, Ojós, Ricote.
- **Universidades**: UMU (Universidad de Murcia), UPCT (Universidad Politécnica de Cartagena), UCAM (Universidad Católica San Antonio de Murcia).
- **Instituciones**: CARM (Comunidad Autónoma de la Región de Murcia), IMIDA, CHS (Confederación Hidrográfica del Segura), SMS (Servicio Murciano de Salud), CREM (Centro Regional de Estadística de Murcia).

## Criterios de inclusión

### Incluir

- Software que interactúa con la **CARM** o sus organismos (Sede Electrónica, Portal de Transparencia, datos abiertos).
- Herramientas para **ayuntamientos** de la Región de Murcia.
- Software de **universidades murcianas** (UMU, UPCT, UCAM) cuando sea específico de la región o la universidad.
- Herramientas de **datos abiertos** de la Región de Murcia (datosabiertos.regiondemurcia.es, CREM).
- Software relacionado con el **Mar Menor** (monitorización, calidad del agua, medio ambiente).
- Herramientas de **agricultura e IMIDA** (Instituto Murciano de Investigación y Desarrollo Agrario).
- Software de **transporte** murciano (tranvía de Murcia, autobuses LAT, puerto de Cartagena).
- Herramientas de **cartografía y SIG** específicas de la Región de Murcia (IDERM, Cartomur).
- Software sobre **playas y costa** murciana.
- Herramientas de **turismo y patrimonio** de la región.
- Software de **energía y agua** regional (CHS, desaladoras, ESAMUR).
- Proyectos de **smart cities** para ciudades murcianas.
- Software sobre **deportes** murcianos (Real Murcia, FC Cartagena, UCAM Murcia CB/CF).
- Proyectos del **sistema sanitario murciano** (SMS, hospitales).
- Software **educativo** específico de la región (Educarm, centros educativos).
- Herramientas de **meteorología** regional.
- Proyectos de **industria y empresa** murciana.

### No incluir

- Software **genérico** que funciona en toda España sin funcionalidad específica de Murcia — eso pertenece a awesome-spain.
- Software de **ámbito europeo** — eso pertenece a awesome-europe.
- Software de **otras comunidades autónomas** españolas.
- Software creado por murcianos que **no tiene funcionalidad específica** de la región.
- Repositorios **archivados o de solo lectura** — van a `DELETED.md`.
- Repos donde el autor indica que el proyecto está **roto, sin mantenimiento o deprecado**.
- Repos **sin README significativo** o que son claramente repos de test/experimento.
- Ejercicios de clase o trabajos académicos sin utilidad real.

### Zona gris — usar criterio

- Proyectos de universidades murcianas que podrían ser genéricos — incluir si tienen datos o configuración específica de Murcia.
- Software que cubre Murcia junto con otras regiones — incluir si Murcia es un foco principal.

## Estándares de calidad

**Mismo listón que [awesome-spain](https://github.com/GeiserX/awesome-spain):**

- **No repos archivados**: si se descubre archivado tras la inclusión, mover a `DELETED.md` inmediatamente.
- **No repos extremadamente sin mantenimiento**: al menos un commit en los últimos 3 años, salvo que sea un proyecto claramente estable/completo.
- **No repos rotos**: si el README dice «deprecated», «no longer maintained», «use X instead» o similar — no incluir. Mover a `DELETED.md` si ya está listado.
- **Estrellas mínimas**: preferir repos con al menos unas pocas estrellas, pero herramientas nicho excepcionales con 0-1 estrellas pueden incluirse si cubren un hueco importante.
- **Verificar cada repo** antes de añadir: comprobar `archived`, `pushed_at`, `stargazers_count` vía `gh api repos/owner/name`.

## Formato de entrada

```markdown
- [Nombre](https://github.com/owner/repo) [![Stars](...)](stargazers) [![Last Commit](...)](commits) [![Language](...)](repo) [![License](...)](LICENSE) [![Tag](...)](url) - Descripción que empieza en mayúscula y termina con punto.
```

Las insignias se generan automáticamente con `scripts/transform-readme.py`. Para contribuir, basta con añadir la entrada en formato simple:

```markdown
- [Nombre](https://github.com/owner/repo) - Descripción que empieza en mayúscula y termina con punto.
```

- La descripción **no debe empezar con el nombre** del proyecto.
- Máximo una línea por entrada.
- Validar con awesome-lint-extra: `python3 lint.py` o mediante el workflow de CI.
- Entradas en **orden alfabético** dentro de cada categoría.
- Categorías en **orden alfabético** en el índice y en el cuerpo del documento.
- Entradas en `DELETED.md` también en **orden alfabético** dentro de cada sección.

## Verificación antes de añadir

Antes de incluir un repositorio, comprobar:

- **Existe y es público**: el enlace de GitHub funciona y el repo no es privado.
- **No está archivado o de solo lectura**: si archivado, va a `DELETED.md` (sección «Archivados»).
- **No está deprecado**: comprobar si el README dice «deprecated», «unmaintained», «broken», «use X instead».
- **Actividad razonable**: al menos un commit en los últimos 3 años, salvo que sea un proyecto estable/completo.
- **No es un duplicado**: cruzar con `README.md` y `DELETED.md`.
- **Calidad mínima**: tiene documentación (README) y no es un repositorio vacío o de test.

## Pull requests y contribuciones

- Las PRs deben usar la plantilla en `.github/PULL_REQUEST_TEMPLATE.md`.
- **Obligatorio**: incluir en la PR la **URL del servicio, API o institución murciana** a la que el software da soporte.
- Plantillas de issues disponibles para sugerir proyectos (`anadir-proyecto.md`) y solicitar retirada (`retirar-proyecto.md`).

## Estructura

- Secciones con `##`, subsecciones con `###`.
- Índice de contenido al principio entre comentarios `<!--lint disable/enable awesome-list-item-->`.
- Al final: sección Contribuir, Nota y Descargo de responsabilidad (como párrafos en negrita, no encabezados ##).

## Temas prohibidos

No se aceptan proyectos relacionados con: pornografía, contenido NSFW, loterías o apuestas, religión, política partidista.

## Difusión

- Notificar a los propietarios de repos abriendo un issue titulado «Listado en awesome-region-de-murcia» con un breve mensaje en español (tuteo) ofreciendo retirar si lo prefieren. Solo 1 issue por organización/usuario — no spamear repos del mismo propietario.
- Publicar en comunidades murcianas (Reddit, foros de la UMU/UPCT, Telegram de devs murcianos) tras alcanzar masa crítica.
- Enviar PR a [sindresorhus/awesome](https://github.com/sindresorhus/awesome) tras 30 días desde la creación del repo.

## Aprendizajes

- Las búsquedas en GitHub con `"region de murcia"` dan resultados muy limitados. Es más efectivo buscar por instituciones concretas (CARM, UMU, UPCT, UCAM, CHS, IMIDA) y por ciudades principales (Murcia, Cartagena, Lorca).
- Muchos repos de universidades murcianas son ejercicios de clase sin utilidad real — filtrar con criterio.
- La CARM tiene organización GitHub `carm-es` con repos de utilidad real (también 4 archivados en DELETED.md).
- `ffis` es una organización con el proyecto SICI CARM (dashboard de indicadores de cartas de servicios).
- El IMIDA y la CHS no tienen presencia significativa en GitHub.
- La UPCT tiene presencia mínima: `UPCTmakers` (repos de 2015, obsoletos), `ppavon/smartEcoRutas` (Reto-UPCT activo). La mayoría de repos con "UPCT" son ejercicios de clase.
- La UMU tampoco tiene organización oficial en GitHub. Los repos son de estudiantes/profesores individuales. Excepciones útiles: `weso/hercules-sync` (HÉRCULES), `AnaAguilarI/Plantilla-TFG-FIUM`.
- La UCAM no tiene presencia significativa en GitHub.
- El topic `murcia` en GitHub tiene ~8 repos, la mayoría de bajo interés.
- `MurciaDev` es una comunidad de devs murcianos con `murcia-tech-hub` (directorio de empresas tech) como repo más útil.
- `KikeOnRails` tiene 2 apps de transporte en tiempo real para Murcia (buses urbanos y aeropuerto).
- Buscar también en GitLab y Bitbucket para instituciones que no usan GitHub.
- **Rate limits**: con 14 agentes paralelos, el API de búsqueda de GitHub (30 req/min) se agota inmediatamente. Estrategia efectiva: usar `gh api repos/...` (core API, 5000/h) para verificar repos conocidos, y WebFetch o curl desde distintas IPs (watchtower, geiserback) para búsquedas.
- **Cartagena**: la mayoría de resultados de búsqueda son sobre Cartagena de Indias (Colombia). Filtrar siempre.
- Repos de deportes de Real Murcia: `ManuelFranco/contadorAbonados` (scraper abonados, activo), `Renilla/checklist-real-murcia` (cromos, activo). FC Cartagena y ElPozo sin presencia.
- GitLab no tiene repos significativos sobre la Región de Murcia.
- **CenticMurcia**: Centro Tecnológico de las TIC de la Región de Murcia. Tiene repos pero son cursos/charlas genéricas (no específicas de Murcia). curso-ciencia-datos (59★) y charla-mcp (11★) descartados por contenido genérico.
- **MurciaLab**: Laboratorio de innovación del Ayuntamiento de Murcia. Repos útiles: ICA_Diario_2025 (calidad del aire CARM), seguimiento (propuestas urbanas), PMP (proyectos anunciados).
- **editum**: Servicio de Publicaciones de la UMU. JATSWizard y docxtojats-pipeline son herramientas activas y específicas de EDITUM.
- **SMARTLAGOON**: Proyecto H2020 con boya de monitorización ambiental en el Mar Menor. SMLG_Buoy_Data con datos de alta frecuencia.
- **pedrosc1967/diccionario_panocho**: Diccionario del panocho (dialecto de la Huerta de Murcia). Sin actividad desde 2021 pero es proyecto estable/completo. 3★.
- **TabErrans/sierra-minera-spatial-dataset**: Datos geoquímicos de la Sierra Minera de Cartagena-La Unión. Muy reciente, con DOI en Zenodo.
- **aconesac/molino-lo-negrete**: Sitio web del patrimonio del Molino de Viento Lo Negrete en Cartagena. Proyecto de restauración catalogado en el Plan Director de Molinos de Viento de la Región de Murcia.
- **SoniaRuiz/marine-forecast**: Previsión marítima para La Manga y Cartagena (también Torrevieja, que es Alicante — incluido porque 2 de 3 zonas son murcianas).

---

*Generated by [LynxPrompt](https://lynxprompt.com) CLI*
