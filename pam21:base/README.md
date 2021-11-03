# LDAP server
## @edt ASIX M06-ASO Curs 2021-2022

### PAM Containers:

 * **edtasixm06/pam:base** Container PAM base per practicar regles PAM.

``` 
docker run --rm --name pam.edt.org -h pam.edt.prg --net 2hisix -it pam21:base

docker run --rm --name pam.edt.org -h pam.edt.prg --net 2hisix --privileged -it pam21:base

```
