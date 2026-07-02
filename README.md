# FreeTime — Gestor de Lembretes

App Android de gestão de lembretes, tarefas, hábitos, medicamentos, compras e notas. Funciona completamente offline, com sincronização opcional via Google Drive.

## Download

[**Descarregar APK mais recente**](https://github.com/JFernandooo/FreeTime/releases/latest)

> Instalação manual: Definições → Segurança → Permitir fontes desconhecidas

## Funcionalidades

- **Lembretes** — 8 tipos (Geral, Medicação, Compras, Financeiro, Aniversário, Consulta, Evento, Prazo), categorias, recorrência e Modo Insistente
- **Lembretes de Localização** — notificações por geofencing ao entrar/sair de uma área; seleção no mapa (OpenStreetMap)
- **Tarefas** — com prazo, hora, prioridade, subtarefas e notificação automática
- **Gestão de Tarefas** — Matriz de Eisenhower (Fazer Já / Agendar / Delegar / Eliminar)
- **Hábitos** — frequência diária/semanal, streak e notificações
- **Medicamentos** — horários de toma com lembretes e controlo de stock
- **Lista de Compras** — por voz ou texto, quick-add por reconhecimento de voz
- **Notas** — com suporte a fixação e criação rápida de lembretes a partir de notas
- **Gestão de Tempo** — técnica Pomodoro (Foco / Pausa Curta / Pausa Longa / Livre com duração personalizada)
- **Calendário** — vista mensal com eventos, lembretes e feriados nacionais (PT e BR)
- **Dashboard** — resumo de toda a actividade, próximos lembretes, gráficos
- **Estatísticas** — produtividade semanal, tendência 7 dias, heatmap de hábitos, histórico 6 meses
- **Pesquisa Global** — pesquisa simultânea em todos os módulos
- **Export CSV/PDF** — exportação de todos os dados
- **Google Drive Sync** — backup e restauro cifrado (AES-256)
- **Suporte multilingue** — Português (PT/PT, PT/BR) e Inglês
- **Modo escuro/claro** — com cores personalizáveis
- **Widgets** — 3 tamanhos para o ecrã inicial

## Versões

| Versão | Destaques |
|--------|-----------|
| v2.1.x | Mapa picker (OpenStreetMap), Pomodoro modo Livre, Gestão de Tarefas (Eisenhower), Estatísticas, permissões revistas |
| v2.0.x | Lembretes de Localização (geofencing), Timeline, Firebase Analytics, export nativo Android |
| v1.9.x | Tags, Modo Insistente, Lixeira, Contactos, Export CSV/PDF, Google Drive, PBKDF2 |
| v1.8.x | Voz, Categorias, Calendário, Dashboard, Medicamentos |

## Privacidade

- Todos os dados ficam no dispositivo (sem servidores externos)
- Backup Google Drive cifrado com AES-256-CBC + PBKDF2-HMAC-SHA256 (100 000 iterações)
- Dados locais encriptados com AES-256 via Android Keystore
- Recolhe dados de utilização **anónimos** via Firebase Analytics (sem nome, email ou identificação pessoal)
- Sem anúncios
