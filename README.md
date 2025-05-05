# 🧑‍💻 Backend-Übung: Benutzer-API mit Express & TypeScript

## 📝 Ziel der Aufgabe

Erstelle einen kleinen Server mit **Express** und **JavaScript/TypeScript**:
- Neuer Benutzer  anlegen (**POST**)
   ```bash
   http://localhost:3000/users
   ```
- Alle Benutzer anzuzeigen (**GET**)
  ```bash
   http://localhost:3000/users
   ```

- Einen bestimmten Benutzer per **ID** abzurufen (**GET /users/:id**)
  ```bash
   http://localhost:3000/users/id
   ```

- Teste alles mit **Postman**

---

## Schritten für dein Projekt

### 1. Neues Projekt erstellen & `.gitignore` anlegen
  ```bash
npm init -y

 ```
```bash
echo "node_modules>.gitignore
```
### 2. Module installiere
```
npm install express uuid
npm install -D  npm install -D typescript ts-node @types/node  concurrently @types/express 

```
### 3. TypeScript `tsconfig.ts` konfigurieren und anpassen
```
npx tsc --init
```
```ts
{
  "compilerOptions": {
    "target": "ESNext",
    "module": "ESNext",
    "moduleResolution": "node",
    "outDir": "./dist",
    "rootDir": "./src",
    "strict": true,
    "esModuleInterop": true,
    "resolveJsonModule": true
  },
  "include": ["src/**/*", "types.ts"]
}
```
### 4.  Dein Script für Projekt in `package.json` anpassen.
```json
"type":"module",
"scripts": {
    "build": "tsc ",
    "watch": "tsc --watch",
    "start": "node --watch dist/index.js",
    "dev": "concurrently \"npm run watch\" \"npm run start\""
}
```

### 5. Erstelle deinen Ordner und darin deine `index.ts`-Datei erstellen
```bash
mkdir src
touch src/index.ts
```

** 😎👷‍♀️Viel Spaß 😎👷‍♀️ **
