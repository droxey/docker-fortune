
# 🔮 docker-fortune

**Execute Unix `fortune` on any OS using Docker!**

> `fortune` is a program that displays a pseudorandom message from a database of quotations that first appeared in Version 7 Unix. Distributions of `fortune` are usually bundled with a collection of themed files, containing sayings like those found on fortune cookies (hence the name), quotations from famous people, jokes, or poetry. -[fortune (Unix) @ Wikipedia](https://en.wikipedia.org/wiki/Fortune_(Unix))

---

## 📦 Building & Running

| Variable | Description |
| -------- | ----------- |
| `USERNAME` | Your DockerHub username. |
| `IMAGE_NAME` | Name of the repository created above. |
| `CONTAINER_NAME` | Choose a name for this container.<br>Can be the same as `IMAGE_NAME`. |

### 1️⃣ Build

_Builds the `Dockerfile` found at the current path (`.`)._

```bash
$ docker build -t USERNAME/IMAGE_NAME .
```

### 2️⃣ Run & Test

_Runs the `IMAGE_NAME` image. Deletes the container after executing the `CMD`_.

```bash
$ docker run --rm --name CONTAINER_NAME IMAGE_NAME
```
