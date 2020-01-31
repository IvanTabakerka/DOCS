# Dockerfile

## Описание

Простой текстовый файл, в котором содержится список команд Докер-клиента. Это простой способ автоматизировать процесс создания образа.

---

# Команды

```shell
$ docker build -t [dockerhubid]/[image] . # Сборка образа по dockerfile
```

---

## Синтаксис

```dockerfile
# our base image
FROM python:3-onbuild

# specify the port number the container should expose
EXPOSE 5000

# run the application
CMD ["python", "./app.py"]
```

---
