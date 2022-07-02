- 👋 Hi, I’m @tiagodaru
- 👀 I’m interested in HomeLab & self hosting
- 🌱 I'm learning about Proxmox and creating and virtualizing some servers and some applications and services running in docker.
I'm in Brazil and around here self hosting and homelab are difficulties, because providers block ports like 80, 443, 21, 22, among others.
And for this reason I am creating an Infrastructure that costs as little as possible.
- ✨ Collaboration on this project is welcome and I will share here what I have studied and used to help the community ...

🇺🇸 This command is used to generate an encrypted username and password to put in the docker-compose.yml

🇧🇷 Este comando serve para gerar um usuário e senha criptografados para colocar no docker-compose.yml

```
echo $(htpasswd -nb <username> <password>) | sed -e s/\\$/\\$\\$/g
```

<!---
tiagodaru/tiagodaru is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
