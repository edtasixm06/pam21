# LDAP server
## @edt ASIX M06-ASO Curs 2021-2022

### PAM Containers:


Exemples d'imatges per practicar PAM individualment i per practicar autnticació PAM amb ldap.


 * **edtasixm06/pam21:base** Container PAM base per practicar regles PAM. Utilitza chfn per practicar els
   exmples del HowTo per aprendre el funcionament dels *type* (*auth*,*account*,*session* i*password*) i 
   dels *control* bàsics (*sufficient*, *required*,*requisite* i *optional*) i avançats (*die*, *ok*).
   També permet practicar *pam_mount.so* per muntar unitats de *tmpfs* o *NFS* als usuaris.

* **edtasixm06/pam21:ldap** Container PAM per practicar l'autenticació PAM unix i PAM ldap. Utilitza els paquets
  *libpam-ldap*, *libnss-ldap*, *nscd* i *nslcd* per configurar l'accés al servei ldap i configura les regles PAM 
  per permetre tant usuaris unix com usuaris LDAP. En tots dos casos es munta en el home un recurs *tmpfs*
  temporal. En el cs dels usuaris LDAP si el seu home no existeix es crea usant *pam_mkhomedir.so*.




``` 
docker run --rm --name pam.edt.org -h pam.edt.prg --net 2hisix -it pam21:base

docker run --rm --name pam.edt.org -h pam.edt.prg --net 2hisix --privileged -it pam21:base

```
