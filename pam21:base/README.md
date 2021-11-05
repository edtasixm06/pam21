# LDAP server
## @edt ASIX M06-ASO Curs 2021-2022

### PAM Containers:

 * **edtasixm06/pam21:base** Container PAM base per practicar regles PAM. Utilitza chfn per practicar els
   exmples del HowTo per aprendre el funcionament dels *type* (*auth*,*account*,*session* i*password*) i
   dels *control* bàsics (*sufficient*, *required*,*requisite* i *optional*) i avançats (*die*, *ok*).
   També permet practicar *pam_mount.so* per muntar unitats de *tmpfs* o *NFS* als usuaris.

``` 
docker run --rm --name pam.edt.org -h pam.edt.prg --net 2hisix --privileged -it pam21:base

```
