# hello-actions

hello github actions (beta)

## Run

### Set token

```bash
TOKEN=`your token`
```

### greet_dispatch
```
curl -X POST \
 -H "Accespt: application/vnd.github.v3+json" \
 -H "Authorization: token ${TOKEN}" \
 https://api.github.com/repos/blck-snwmn/hello-actions/actions/workflows/greet_dispatch.yml/dispatches \
 -d '{"ref":"master", "inputs":{"name":"bob","email":"test@gmail.com","location":"space"}}'
```
