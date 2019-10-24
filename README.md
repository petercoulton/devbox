# devbox

## TL;DR

1. Use Docker Compose to manage everything cleanly
2. Run Traefik in Docker configured to use Docker as a backend
3. Run dnsmasq in Docker to resolve a nice tld to a local ip
4. Configure MacOS to use dnsmasq for DNS lookup
    + Don't forget to add a fallback dns in the Mac system preferences, 
      otherwise when docker restarts you won't be able to access the internet
5. (Optional) Run Portainer to make inspecting Docker easier

## TODO

+ [x] Add todo list
+ [ ] Add ssl
+ [ ] Capture access logs

## Bibliography

+ https://medium.com/@williamhayes/local-dev-on-docker-fun-with-dns-85ca7d701f0a
+ https://www.stevenrombauts.be/2018/01/use-dnsmasq-instead-of-etc-hosts/
+ https://github.com/portainer/portainer-compose/
+ https://github.com/jpillora/docker-dnsmasq
  + Uses [webproc](https://github.com/jpillora/webproc) to make 
    the `dnsmasq` config editable via a web app.
+ https://blog.agchapman.com/using-variables-in-docker-compose-files/

### Other interesting links

+ [Dinghy](https://github.com/codekitchen/dinghy)
  + An older project with a cli tool for managing project

