# CHANGELOG
 
Registro de cambios del proyecto terraform-s3-04.
Formato basado en https://keepachangelog.com
 
## [v1.1] - 2025-06-01
 
### Added
- Modulo reutilizable modules/mi-recurso para crear buckets S3
- Archivo REBASE.md con documentación del proceso de limpieza de commits
- Archivo CHANGELOG.md con registro de versiones
 
### Changed
- Historial de commits limpiado con git rebase -i
- README.md actualizado con notas del proyecto
 
## [v1.0] - 2025-05-01
 
### Added
- Configuración inicial de Terraform con provider AWS apuntando a LocalStack
- Recurso aws_s3_bucket para crear un bucket S3 simulado
- Recurso aws_instance para crear una instancia EC2 simulada
- Workflow validate.yml para validar el código Terraform en cada push
- Workflow deploy.yml para ejecutar init, plan y apply contra LocalStack
- Badge de estado en README.md
- Archivo .gitignore para excluir archivos generados por Terraform

