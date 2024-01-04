## Production Setup (tested)

### Local (Linux & Windows)

#### Backend

Move to **./server/** and set the correct value for **HOME_CLOUD_STORAGE** in
**.env** (see examples in **sample.env**), and then
run npm start:
```bash
npm start
```

#### Frontend
Move to **./client/** and create a file named **.env.production**, set the
correct value for **REACT_APP_API_URL** (see examples in **sample.env**). Then,
install serve globaly:
```bash
npm i -g serve
```

Build the app:

```bash
npm run build # Or yarn build
```

Start the server:

```bash
serve -s build -l 3000 # Or another port of your choice
```
