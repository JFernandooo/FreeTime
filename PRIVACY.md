# Política de Privacidade — FreeTime

_Última atualização: 3 de julho de 2026_

**Idiomas:** [Português](#português) | [English](#english)

---

## Português

### Quem somos

O FreeTime é uma app de gestão pessoal (lembretes, tarefas, hábitos, medicação, listas de compras e notas) desenvolvida por um programador independente. A FreeTime não opera servidores próprios de armazenamento de dados dos utilizadores — os teus dados ficam no teu dispositivo e, opcionalmente, na tua própria conta Google Drive.

### Que dados a app recolhe e porquê

| Dado | Para quê | Onde fica guardado |
|---|---|---|
| Lembretes, tarefas, hábitos, medicação, listas de compras, notas, categorias | Funcionalidade principal da app | Localmente, no dispositivo, numa base de dados Hive **encriptada com AES-256** (chave gerada aleatoriamente e guardada no Android Keystore) |
| Localização (GPS) | Lembretes por localização — disparar uma notificação ao entrar/sair de uma zona geográfica que definas (ex.: "lembrar de comprar leite ao chegar ao supermercado") | Não sai do dispositivo; usada apenas em memória para registar geofences junto do Google Play Services |
| Contacto (nome/número) | Associar um contacto a um lembrete, escolhido através do seletor de contactos do próprio sistema Android | Guardado localmente, encriptado, tal como os restantes dados do lembrete |
| Áudio (voz) | Ditado por voz para criação rápida de itens em listas de compras (reconhecimento de voz processado pelo sistema operativo, o áudio não é gravado nem enviado pela FreeTime) | Não guardado pela app |
| Eventos de uso anónimos (ex.: "lembrete criado", "hábito concluído") | Perceber que funcionalidades são usadas, para priorizar melhorias | Firebase Analytics (Google) — eventos anónimos, sem nome, email, conteúdo dos lembretes ou qualquer identificador pessoal |

A app **não recolhe** nome, email, número de telefone (salvo o que escolheres associar a um lembrete específico), nem qualquer identificador de publicidade.

### Permissões pedidas

- **Localização em segundo plano (`ACCESS_BACKGROUND_LOCATION`)**: necessária para que os lembretes por localização disparem mesmo com a app fechada — é o mecanismo de geofencing do Android/Google Play Services. Só é usada se criares um lembrete por localização; se não usares essa funcionalidade, a permissão nunca é solicitada.
- **Contactos (`READ_CONTACTS`)**: usada apenas quando escolhes explicitamente "associar contacto" num lembrete, através do seletor nativo de contactos do Android. A app não lê nem sincroniza a tua agenda em bloco.
- **Microfone (`RECORD_AUDIO`)**: usada apenas quando ativas o ditado por voz para adicionar itens às listas de compras.
- **Notificações, alarmes exatos, otimização de bateria**: necessárias para que os lembretes e alarmes agendados disparem à hora certa.

### Google Drive (backup/sincronização)

Se ativares a sincronização com o Google Drive, os teus dados são exportados, **encriptados no dispositivo com AES-256-GCM** (chave derivada por PBKDF2, específica da tua conta), e guardados na pasta privada da app dentro da tua própria conta Google Drive (`appDataFolder` — um espaço que só a app FreeTime consegue aceder, invisível noutras apps do Drive e não navegável manualmente por ti nem por nós). A FreeTime **não tem acesso** a este ficheiro nem à tua conta Google — apenas tu, através da tua conta.

### Partilha de dados com terceiros

A FreeTime **não vende, aluga nem partilha** os teus dados pessoais com terceiros. Os únicos serviços de terceiros envolvidos são:
- **Google Play Services** (geofencing, localização) — processa localização localmente no dispositivo.
- **Google Drive** — armazenamento do teu backup encriptado, na tua própria conta.
- **Firebase Analytics (Google)** — eventos de uso anónimos, sem dados pessoais.

Nenhum destes serviços recebe o conteúdo dos teus lembretes, tarefas, notas ou dados de saúde/medicação.

### Os teus dados, o teu controlo

Podes exportar ou desativar a sincronização a qualquer momento nas definições da app (opção "Sair da conta"). Desinstalar a app apaga todos os dados locais. A app não tem ainda um botão dedicado para apagar o backup no Drive — para remover esse ficheiro, revoga o acesso da FreeTime à tua conta Google em [myaccount.google.com/permissions](https://myaccount.google.com/permissions), o que remove os dados associados a essa autorização.

### Contacto

Para questões sobre esta política, contacta: **josefernando670@gmail.com**

---

## English

### Who we are

FreeTime is a personal organization app (reminders, tasks, habits, medication, shopping lists and notes) developed by an independent developer. FreeTime does not operate its own servers for storing user data — your data stays on your device and, optionally, in your own Google Drive account.

### What data the app collects and why

| Data | Purpose | Where it's stored |
|---|---|---|
| Reminders, tasks, habits, medication, shopping lists, notes, categories | Core app functionality | Locally on the device, in a Hive database **encrypted with AES-256** (randomly generated key stored in the Android Keystore) |
| Location (GPS) | Location-based reminders — trigger a notification when entering/leaving a geographic zone you define (e.g. "remind me to buy milk when I arrive at the supermarket") | Never leaves the device; used only in memory to register geofences with Google Play Services |
| Contact (name/number) | Linking a contact to a reminder, chosen via Android's native contact picker | Stored locally, encrypted, like the rest of the reminder data |
| Audio (voice) | Voice dictation for quickly adding shopping list items (speech recognition handled by the OS; FreeTime does not record or transmit audio) | Not stored by the app |
| Anonymous usage events (e.g. "reminder created", "habit completed") | Understand which features are used, to prioritize improvements | Firebase Analytics (Google) — anonymous events, no name, email, reminder content or any personal identifier |

The app **does not collect** name, email, phone number (other than what you choose to link to a specific reminder), or any advertising identifier.

### Permissions requested

- **Background location (`ACCESS_BACKGROUND_LOCATION`)**: required so location-based reminders trigger even when the app is closed — this is the Android/Google Play Services geofencing mechanism. It's only used if you create a location-based reminder; if you never use that feature, the permission is never requested.
- **Contacts (`READ_CONTACTS`)**: used only when you explicitly choose to "link a contact" to a reminder, via Android's native contact picker. The app does not read or bulk-sync your address book.
- **Microphone (`RECORD_AUDIO`)**: used only when you enable voice dictation to add shopping list items.
- **Notifications, exact alarms, battery optimization**: required so scheduled reminders and alarms fire at the right time.

### Google Drive (backup/sync)

If you enable Google Drive sync, your data is exported, **encrypted on-device with AES-256-GCM** (key derived via PBKDF2, specific to your account), and stored in the app's private folder within your own Google Drive account (`appDataFolder` — a space only the FreeTime app can access, invisible in the regular Drive UI and not browsable by you or by us). FreeTime **has no access** to this file or your Google account — only you, through your own account.

### Sharing data with third parties

FreeTime does **not sell, rent, or share** your personal data with third parties. The only third-party services involved are:
- **Google Play Services** (geofencing, location) — processes location locally on the device.
- **Google Drive** — storage of your encrypted backup, in your own account.
- **Firebase Analytics (Google)** — anonymous usage events, no personal data.

None of these services receive the content of your reminders, tasks, notes, or medication/health data.

### Your data, your control

You can export data or disable sync at any time from the app's settings ("Sign out" option). Uninstalling the app deletes all local data. The app does not yet have a dedicated button to delete the Drive backup — to remove that file, revoke FreeTime's access to your Google account at [myaccount.google.com/permissions](https://myaccount.google.com/permissions), which removes the data associated with that authorization.

### Contact

For questions about this policy, contact: **josefernando670@gmail.com**
