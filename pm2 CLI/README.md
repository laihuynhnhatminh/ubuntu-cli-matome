# Ubuntu interaction with PM2

## Run pm2 with config file (js, cjs)

```bash
pm2 start ecosystem.config.js
```

## Kill pm2 process

```bash
pm2 kill
```

## pm2 delete process

```bash
pm2 delete <app-name | id>
```

## pm2 save process list so that it will auto resurrect (restart) even after ubuntu restart

```bash
pm2 save
```
