# VOLT — Power Your Game

A VOLT é uma loja gamer feita em React e Capacitor para encontrar consoles, jogos e acessórios. O app reúne catálogo, busca, categorias, favoritos, carrinho e localização por GPS.

## Notificações locais

O app usa `@capacitor/local-notifications` para demonstrar alertas nativos:

- **Verificar / permitir notificações:** consulta `checkPermissions()` e solicita autorização com `requestPermissions()` quando necessário. No Android 13+, o sistema apresenta a permissão de notificações.
- **Enviar alerta agora:** dispara uma notificação promocional da VOLT.
- **Agendar lembrete:** agenda um alerta para 10 segundos depois, inclusive com o app em segundo plano.

As notificações nativas precisam ser executadas em um aparelho ou emulador com a plataforma Capacitor instalada; a versão web informa que o recurso requer o app nativo.

## Executar

```bash
npm install
npm run dev
```

Para Android, adicione a plataforma se ela ainda não existir e sincronize o plugin:

```bash
npx cap add android
npx cap sync android
npx cap open android
```

Compile e execute pelo Android Studio em um aparelho ou emulador. Conceda a permissão de notificações quando solicitada e teste os botões na seção **VOLT / ALERT SYSTEM**.

## Tecnologias

React, Vite, Capacitor, Supabase, Geolocation e Local Notifications.

## Evidências da atividade

Adicione aqui capturas de tela e um GIF/vídeo gravado no aparelho após executar o app nativo. A gravação deve mostrar a concessão da permissão, o alerta imediato e o lembrete agendado.

<img width="383" height="854" alt="Captura de tela 2026-11-13 105322" src="https://github.com/user-attachments/assets/af120958-e8b9-49c2-9829-46bd6b34b991" />
<img width="382" height="832" alt="Captura de tela 2026-11-13 102504" src="https://github.com/user-attachments/assets/c1d863a2-3a7f-4487-967b-5a4bc40e61e7" />
<img width="1222" height="653" alt="Captura de tela 2026-11-13 105555" src="https://github.com/user-attachments/assets/f886a661-15ca-48ab-9e39-b221d3300832" />


