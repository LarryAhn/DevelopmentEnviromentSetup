# Redis
> Redis 설치하기

```
$ wget http://download.redis.io/releases/redis-3.2.4.tar.gz
$ tar xzf redis-3.2.4.tar.gz
$ cd redis-3.2.4
$ make
```
> Run
```
$ src/redis-server
```

---
### Homebrew 를 통한 Redis 설치
> [Homebrew 설치바로가기](../Homebrew/Homebrew.md)
```
$ brew install redis
$ redis-server
```
Launch Redis on computer starts.
```
$ ln -sfv /usr/local/opt/redis/*.plist ~/Library/LaunchAgents
```

Start Redis server via “launchctl”.
```
$ launchctl load ~/Library/LaunchAgents/homebrew.mxcl.redis.plist
```

Start Redis server using configuration file.
```
$ redis-server /usr/local/etc/redis.conf
```

Stop Redis on autostart on computer start.
```
$ launchctl unload ~/Library/LaunchAgents/homebrew.mxcl.redis.plist
```

Location of Redis configuration file.
```
/usr/local/etc/redis.conf
```

Uninstall Redis and its files.
```
$ brew uninstall redis
$ rm ~/Library/LaunchAgents/homebrew.mxcl.redis.plist
```

Get Redis package information.
```
$ brew info redis
```
Test if Redis server is running.
```
$ redis-cli ping
```

---
### Reference
- http://redis.io/download  
- https://medium.com/petehouston/install-and-config-redis-on-mac-os-x-via-homebrew-eb8df9a4f298#.s47w2ybbm