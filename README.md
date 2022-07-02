- 👋 Hi, I’m @tiagodaru
- 👀 I’m interested in HomeLab & self hosting
- 🌱 I'm learning about Proxmox and creating and virtualizing some servers and some applications and services running in docker.
I'm in Brazil and around here self hosting and homelab are difficulties, because providers block ports like 80, 443, 21, 22, among others.
And for this reason I am creating an Infrastructure that costs as little as possible.
- ✨ Collaboration on this project is welcome and I will share here what I have studied and used to help the community ...

🇺🇸 🏁 To start, let's create a reverse proxy in order to make our public server in this scenario a low cost VPS with Linux Ubuntu Server just to redirect and bypass the blocking of ports of Brazilian internet providers.

🇧🇷 🏁 Para começar vamos criar um proxy reverso a fim de fazer com que o nosso servidor público neste cenário é uma VPS com Linux Ubuntu Server de baixo custo só para redirecionar e contornar o bloqueio de portas dos provedores de internet brasileiros.


🇺🇸 Our working folder will be /portiner/traefik

🇧🇷 Nossa pasta de trabalho será a /portainer/traefik

```
sudo mkdir -p /portiner/traefik
```

🇺🇸 This command is used to generate an encrypted username and password to put in the docker-compose.yml

🇧🇷 Este comando serve para gerar um usuário e senha criptografados para colocar no docker-compose.yml

```
echo $(htpasswd -nb <username> <password>) | sed -e s/\\$/\\$\\$/g
```

🇺🇸 Create the acme.json file and then we will make the permissions read-only.

🇧🇷 Crie o arquivo acme.json e em seguida deixaremos as permissões somente como leitura.

```
touch /portainer/traefik/acme.json ; chmod 600 /portainer/traefik/acme.json
```
<!---
tiagodaru/tiagodaru is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
