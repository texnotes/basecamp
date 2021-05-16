# DevOps GL Basecamp - Lab Work #1
## IaaC Ansible
It is not clear in the assignment that only two groups entered to the iaac- group, i.e. the third of the four virtual machines was for tests.

![Screenshot](https://github.com/texnotes/basecamp/blob/main/img/Screenshot%202021-05-16%20232830.png "Screenshot")

Then I made a passwordless login for three instances, but for the sudo team, I think it would be more correct to pass the password through the Ansible command or use a vault. (Updated: I was wrong, it turns out that all groups should have one password, or vice versa - many passwords. I made a shudo without entering a password: echo "$USER ALL=(ALL:ALL) NOPASSWD: ALL" | sudo tee /etc/sudoers.d/$USER. But the screenshot did not change anymore).

![Screenshot](https://github.com/texnotes/basecamp/blob/main/img/Screenshot%202021-05-16%20231555.png "Screenshot")

### Useful links:
1. How to Setup Passwordless SSH Login - [Linuxize](https://linuxize.com/post/how-to-setup-passwordless-ssh-login/)
2. Обзор Ansible - [Platon Korzh](https://medium.com/@platon_korzh/%D0%BE%D0%B1%D0%B7%D0%BE%D1%80-ansible-38a794937a3c)
3. Автоматизируем и ускоряем процесс настройки облачных серверов с Ansible -[Сообщество InfoboxCloud](https://infoboxcloud.ru/community/blog/infoboxcloud/226.html)
4. How to Use Ansible: A Reference Guide - [DigitalOcean](https://www.digitalocean.com/community/cheatsheets/how-to-use-ansible-cheat-sheet-guide)
5. Создание файла инвентаря Ansible - [8host](https://www.8host.com/blog/sozdanie-fajla-inventarya-ansible/)
6. Ansible playbook to determine OS release - [Stack Exchange Network](https://superuser.com/questions/1395954/ansible-playbook-to-determine-os-release)
7. How to Create a File in Ansible - [phoenixNAP](https://phoenixnap.com/kb/ansible-create-file)
8. How to Use Ansible Roles to Abstract your Infrastructure Environment - [DigitalOcean](https://www.digitalocean.com/community/tutorials/how-to-use-ansible-roles-to-abstract-your-infrastructure-environment)
9. Missing sudo password in Ansible - [Stack Overflow](https://stackoverflow.com/questions/25582740/missing-sudo-password-in-ansible)
10. IaaC (Ansible) module of DevOsp Basecamp for Telco - [GL Basecamp](https://github.com/yurnov/IaC_Ansible_basecamp)

