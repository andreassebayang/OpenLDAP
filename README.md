# Openldap with Phpopenldapadmin

## Structure DIT Recomendations:
![image](https://github.com/user-attachments/assets/6e8eda68-da98-4b6f-bbdf-33a021387f40)

### 1. Template LDIF - Create New User
Using this [file](https://github.com/andreassebayang/OpenLDAP/blob/main/template_add_new_User.ldif)

> [!Note]
> - Ganti USERNAME, Nama Lengkap, email@example.com, dll sesuai kebutuhan
> - Untuk userPassword, kamu bisa pakai {SSHA} dengan hash dari slappasswd, contoh:
>  `slappasswd -h {SSHA} -s YourPasswordHere`


### 2.  Tempate LDIF - Create New OU
Using this [file](https://github.com/andreassebayang/OpenLDAP/blob/main/Template_Add_New_OU.ldif)
> [!Note]
> - Contoh: `ou=People`, `ou=Groups`, `ou=IT, ou=HR`, dsb

### 3.  Tempate LDIF - Create New Grop
Using this [file](https://github.com/andreassebayang/OpenLDAP/blob/main/Template_add_new_group.ldif)
> [!Note]
> - Tambahkan lebih banyak `member:` jika anggotanya lebih dari  dua




This project leverages the powerful [Osixia/docker-openldap](https://github.com/osixia/docker-openldap) image.
Special thanks to the Osixia team for providing a robust and well-documented OpenLDAP container solution that serves as the core of this implementation.
