# Развертывание go-функции в через Github Actions

## особенность

Почему-то яндекс облако не принимает новый формат версии go, поэтому в `go.mod` я указываю так

```bash
module github-actions

go 1.21
```

Если указать `1.21.1` возникает ошибка:

```json
{"errorMessage":"plugin.Open(\"/function/code/main\"): plugin was built with a different version of package internal/godebugs","errorType":"LoadPluginError"}
```
