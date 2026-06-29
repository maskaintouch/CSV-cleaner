# Čistič CSV — Gubi

Webová aplikace pro opravu CSV exportů z databáze Gubi.

## Funkce
- Oprava telefonních čísel (odstranění textu)
- Odstranění přesných duplikátů
- Upozornění na sdílené e-maily, chybějící údaje, neznámého plátce
- Přihlášení přes Google účet
- Nahrání opraveného souboru přímo na Google Drive
- Historie zpracovaných souborů

## Nasazení na Vercel

1. Nahrajte tento repozitář na GitHub
2. Jděte na [vercel.com](https://vercel.com) → **Add New Project**
3. Importujte repozitář → **Deploy**
4. Zkopírujte výslednou URL (např. `https://csv-cleaner-xxx.vercel.app`)

## Nastavení Google OAuth

V [Google Cloud Console](https://console.cloud.google.com):

1. **APIs & Services → Credentials → váš OAuth Client ID → Edit**
2. Do **Authorized JavaScript origins** přidejte:
   - `https://csv-cleaner-xxx.vercel.app` (vaše Vercel URL)
3. Uložte

## Lokální spuštění

```bash
npx serve .
```

Aplikace poběží na `http://localhost:3000`.
Pro OAuth lokálně přidejte `http://localhost:3000` do Authorized JavaScript origins.
