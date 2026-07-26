# Aprender Juntos — Plataforma Django (PT)

Projeto criado a partir do seu arquivo ZIP (copiado em `static/vendor/`) e convertido para páginas dinâmicas.

## Como rodar
```bash
python -m venv .venv
source .venv/bin/activate  # Windows: .venv\Scripts\activate
pip install -r requirements.txt
python manage.py migrate
python manage.py loaddata fixtures/initial_data.json
python manage.py runserver
```
Acesse: http://127.0.0.1:8000/

## Onde colocar conteúdos
- **Cursos/Aulas**: via painel Admin (`/admin/`) ou via shell.
- **Professores**: via Admin.
- **Home/Sobre/Contacto**: em **Admin > HomeConfig / Página**.
- **Assets do site original**: copiados do ZIP para `static/vendor/`. Ajuste seus `templates` para usar o CSS/JS original se desejar.

## Estrutura
```
aprender_juntos/
  manage.py
  aprender_juntos/
  paginas/         # Home e páginas institucionais
  cursos/          # Cursos e aulas
  professores/     # Equipe
  templates/       # Templates Django (PT)
  static/
    site.css       # Estilo base
    vendor/        # Conteúdo extraído do ZIP enviado
  fixtures/
    initial_data.json
```
