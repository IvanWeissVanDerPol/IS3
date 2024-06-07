# Pruebas de inspección de código 
## Complejidad ciclomática
Este análisis se realizó utilizando la herramienta radon

### proyecto_is2\cms\gcloud.py
- `C 6:0 GoogleCloudMediaFileStorage` - A (2)
- `M 11:4 GoogleCloudMediaFileStorage.url` - A (1)

### proyecto_is2\cms\views.py
- `F 12:0 principal` - B (10)
- `F 57:0 obtener_publicaciones` - B (10)
- `F 98:0 ordenamiento` - A (4)
- `F 119:0 publicaciones_categoria` - A (2)

### proyecto_is2\comentarios\apps.py
- `C 4:0 ComentariosConfig` - A (1)

### proyecto_is2\comentarios\forms.py
- `C 4:0 CommentForm` - A (2)
- `M 17:4 CommentForm.__init__` - A (1)

### proyecto_is2\comentarios\models.py
- `C 6:0 Comment` - A (2)
- `M 37:4 Comment.__str__` - A (1)

### proyecto_is2\comentarios\views.py
- `F 9:0 comentar` - A (3)
- `F 39:0 responder` - A (3)
- `F 86:0 verificar` - A (3)
- `F 74:0 nuevo` - A (2)

### proyecto_is2\comentarios\migrations\0001_initial.py
- `C 9:0 Migration` - A (1)

### proyecto_is2\comentarios\migrations\0002_initial.py
- `C 8:0 Migration` - A (1)

### proyecto_is2\comentarios\templatetags\filtro_comentarios.py
- `F 7:0 respuestas` - A (1)
- `F 11:0 cantidad` - A (1)

### proyecto_is2\froala_editor\fields.py
- `C 10:0 FroalaField` - A (2)
- `M 28:4 FroalaField.formfield` - A (2)
- `M 13:4 FroalaField.__init__` - A (1)
- `M 25:4 FroalaField.get_internal_type` - A (1)

### proyecto_is2\froala_editor\views.py
- `F 18:0 image_upload` - A (3)
- `F 44:0 video_upload` - A (3)
- `F 57:0 files_manager_upload` - A (2)
- `F 65:0 file_upload` - A (2)
- `F 11:0 get_storage_class` - A (1)

### proyecto_is2\froala_editor\widgets.py
- `M 21:4 FroalaEditor.get_options` - B (8)
- `M 88:4 FroalaEditor._media` - B (7)
- `C 8:0 FroalaEditor` - A (4)
- `M 9:4 FroalaEditor.__init__` - A (1)
- `M 74:4 FroalaEditor.render` - A (1)
- `M 80:4 FroalaEditor.trigger_froala` - A (1)

### proyecto_is2\kanban\apps.py
- `C 4:0 KanbanConfig` - A (1)

### proyecto_is2\kanban\models.py
- `C 6:0 Registro` - A (2)
- `M 41:4 Registro.__str__` - A (1)

### proyecto_is2\kanban\views.py
- `F 80:0 actualizar` - F (58)
- `F 218:0 motivo` - A (5)
- `F 264:0 historial` - A (3)
- `F 21:0 kanban` - A (1)
- `F 292:0 registrar` - A (1)

### proyecto_is2\kanban\migrations\0001_initial.py
- `C 7:0 Migration` - A (1)

### proyecto_is2\kanban\migrations\0002_initial.py
- `C 8:0 Migration` - A (1)

### proyecto_is2\kanban\migrations\0003_initial.py
- `C 6:0 Migration` - A (1)

### proyecto_is2\kanban\tests\test_apps.py
- `C 5:0 KanbanConfigTest` - A (2)
- `M 7:4 KanbanConfigTest.test_apps_config` - A (1)
- `M 11:4 KanbanConfigTest.test_default_auto_field` - A (1)

### proyecto_is2\kanban\tests\test_models.py
- `C 6:0 RegistroModelTest` - A (2)
- `M 8:4 RegistroModelTest.setUp` - A (1)
- `M 13:4 RegistroModelTest.test_registro_creation` - A (1)
- `M 28:4 RegistroModelTest.test_str_method` - A (1)

### proyecto_is2\kanban\tests\test_urls.py
- `C 5:0 KanvanURLsTestCase` - A (2)
- `M 7:4 KanvanURLsTestCase.test_kanban_url_resolves_to_kanban_view` - A (1)
- `M 11:4 KanvanURLsTestCase.test_actualizar_url_resolves_to_actualizar_view` - A (1)
- `M 15:4 KanvanURLsTestCase.test_motivo_url_resolves_to_motivo_view` - A (1)

### proyecto_is2\login\apps.py
- `C 3:0 LoginConfig` - A (2)
- `M 7:4 LoginConfig.ready` - A (1)

### proyecto_is2\login\forms.py
- `C 21:0 FormularioActualizarPerfil` - A (3)
- `M 49:4 FormularioActualizarPerfil.__init__` - A (2)
- `C 6:0 FormularioRegistro` - A (1)

### proyecto_is2\login\models.py
- `C 5:0 Usuario` - A (2)
- `M 35:4 Usuario.__str__` - A (1)

### proyecto_is2\login\signals.py
- `F 7:0 asignar_roles` - A (3)

### proyecto_is2\login\views.py
- `F 136:0 perfil_actualizar` - B (7)
- `F 11:0 inicio_sesion` - A (4)
- `F 48:0 registro` - A (3)
- `F 176:0 cargar_imagen` - A (3)
- `F 103:0 perfil_usuario` - A (2)
- `F 85:0 cerrar_sesion` - A (1)

### proyecto_is2\login\migrations\0001_initial.py
- `C 8:0 Migration` - A (1)

### proyecto_is2\login\migrations\0002_initial.py
- `C 6:0 Migration` - A (1)

### proyecto_is2\login\tests\test_apps.py
- `C 5:0 LoginConfigTest` - A (2)
- `M 6:4 LoginConfigTest.test_apps_config` - A (1)
- `M 10:4 LoginConfigTest.test_default_auto_field` - A (1)

### proyecto_is2\login\tests\test_models.py
- `C 6:0 UsuarioModelTest` - A (2)
- `M 7:4 UsuarioModelTest.test_usuario_creation` - A (1)
- `M 19:4 UsuarioModelTest.test_str_method` - A (1)

### proyecto_is2\login\tests\test_urls.py
- `C 5:0 UrlsTests` - A (2)
- `M 6:4 UrlsTests.test_inicio_sesion_url_resuelta` - A (1)
- `M 10:4 UrlsTests.test_registro_url_resuelta` - A (1)
- `M 14:4 UrlsTests.test_cerrar_sesion_url_resuelta` - A (1)
- `M 18:4 UrlsTests.test_perfil_usuario_url_resuelta` - A (1)
- `M 22:4 UrlsTests.test_perfil_actualizar_url_resuelta` - A (1)

### proyecto_is2\login\tests\test_views.py
- `C 6:0 ViewsTests` - A (2)
- `M 7:4 ViewsTests.setUp` - A (1)
- `M 13:4 ViewsTests.test_inicio_sesion` - A (1)
- `M 18:4 ViewsTests.test_registro` - A (1)
- `M 23:4 ViewsTests.test_cerrar_sesion` - A (1)
- `M 29:4 ViewsTests.test_perfil_usuario` - A (1)
- `M 35:4 ViewsTests.test_perfil_actualizar` - A (1)
- `M 41:4 ViewsTests.test_perfil_actualizar_post` - A (1)

### proyecto_is2\poblacion\carga_categorias.py
- `F 12:0 cargar_categorias` - A (4)

### proyecto_is2\poblacion\carga_publicaciones.py
- `F 15:0 cargar_publicaciones` - B (9)

### proyecto_is2\poblacion\carga_usuarios.py
- `F 12:0 cargar_usuarios` - B (6)

### proyecto_is2\publicaciones\apps.py
- `C 4:0 PublicacionesConfig` - A (1)

### proyecto_is2\publicaciones\forms.py
- `C 6:0 PublicacionForm` - B (6)
- `M 43:4 PublicacionForm.get_categoria_choices` - A (5)
- `C 55:0 BusquedaAvanzadaForm` - A (5)
- `M 30:4 PublicacionForm.__init__` - A (4)
- `M 75:4 BusquedaAvanzadaForm.__init__` - A (4)

### proyecto_is2\publicaciones\models.py
- `M 167:4 Publicacion_solo_text.save` - B (9)
- `C 26:0 Publicacion_solo_text` - A (5)
- `C 11:0 Calificacion` - A (1)
- `M 153:4 Publicacion_solo_text.__str__` - A (1)

### proyecto_is2\publicaciones\views.py
- `F 62:0 publicar` - B (9)
- `F 31:0 home` - A (5)
- `F 97:0 buscar` - A (5)
- `F 159:0 publicaciones_buscador` - A (5)
- `F 18:0 obtener_ip_usuario` - A (3)
- `F 128:0 mis_publicaciones` - A (3)

### proyecto_is2\publicaciones\migrations\0001_initial.py
- `C 8:0 Migration` - A (1)

### proyecto_is2\publicaciones\migrations\0002_initial.py
- `C 8:0 Migration` - A (1)

### proyecto_is2\roles\apps.py
- `C 4:0 RolesConfig` - A (1)

### proyecto_is2\roles\models.py
- `C 6:0 Rol` - A (1)
- `M 17:4 Rol.__str__` - A (1)

## Análisis líneas de código

LOC: 3713 

LLOC: 1893 

SLOC: 2268 

Comments: 184 

Single comments: 152 

Multi: 612 

Blank: 681 

- Comment Stats
    - (C % L): 5%
    - (C % S): 8%
    - (C + M % L): 21%

## Pylint
Errores: 70

Convenciones de código: 466

Advertencia: 40

Refactorización: 46

![image](https://github.com/CamiMaidana/IS3/assets/76019683/03628a7d-9f0c-4eb7-8534-653d0b4289d2)


![image](https://github.com/IvanWeissVanDerPol/IS3/assets/76019683/5f514f2c-0eeb-4dfa-ba35-84c24fe0b37b)

